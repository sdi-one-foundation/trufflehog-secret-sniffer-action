# TruffleHog Secret Sniffer Action

A GitHub Action that uses TruffleHog to scan your repository for secrets and sensitive information. If secrets are found, it will fail the action, post annotations on the code, comment on pull requests, and notify the team via email.

## Table of Contents
- [TruffleHog Secret Sniffer Action](#trufflehog-secret-sniffer-action)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Setup](#setup)
  - [Configuration](#configuration)
    - [Inputs](#inputs)
  - [Example Email Notification](#example-email-notification)
  - [Example PR Comment](#example-pr-comment)
  - [Excluding False Positives](#excluding-false-positives)
    - [Custom Allowlist](#custom-allowlist)
  - [Allowlist Pattern Format](#allowlist-pattern-format)

## Features

- **Smart Scanning**:
  - For pull requests: Only scans files that have changed and still exist (ignores deleted files)
  - For pushes to main: Performs a comprehensive scan of the entire Git history
- **Detailed Reporting**:
  - GitHub code annotations with commit details and dates
  - Pull request comments with tabular findings
  - Email notifications with statistics and detailed findings
- **Secret Context**:
  - Shows which files contain secrets
  - Displays commit information (hash, author, date)
  - Categorizes secrets by type
- **Workflow Integration**:
  - Fails the build when secrets are detected
  - Creates clear visual indicators in GitHub UI

## Setup

1. Add the action to your workflow YAML file:

```yaml
name: Secret Sniffer - TruffleHog
description: |
  This workflow runs TruffleHog to detect secrets in the repository.
  It is triggered on every push to the main branch.

on:
  push:
    branches:
      - main
  pull_request:
    types: [opened, synchronize, reopened]
  workflow_dispatch:

jobs:
  trufflehog:
    runs-on: ubuntu-latest
    defaults:
      run:
        shell: bash

    steps:
      - name: Secret Scanning Action
        uses: sdi-one-foundation/trufflehog-secret-sniffer-action@v1
        with:
            ses-username: ${{secrets.FOUNDATION_SES_USERNAME}}
            ses-password: ${{secrets.FOUNDATION_SES_PASSWORD}}
```

## Configuration

### Inputs

| Input | Description | Required |
|-------|-------------|----------|
| `ses-username` | Username for AWS SES email notifications | Yes |
| `ses-password` | Password for AWS SES email notifications | Yes |

## Example Email Notification

When secrets are detected, the action sends an email that includes the following:

The email contains:

- A warning header identifying that secrets were detected
- Information about the repository and event type
- Links to the repository, GitHub Action run, and pull request (if applicable)
- Details about the detected secrets including file and line information, commit number, author, and date of commit
- Recommendations for remediation

## Example PR Comment

When secrets are detected in a pull request, the action adds a comment like this:

```markdown
## ⚠️ Security Alert: Secrets Detected by TruffleHog ⚠️

This pull request has been scanned for secrets using TruffleHog, and sensitive information has been detected. Please review the findings below and take appropriate action to secure your repository.

TruffleHog has detected secrets in this pull request. Please review and remove any sensitive information.

| File | Line | Secret Type |
|------|------|-------------|
| `config/settings.json` | 42 | AWS |

**Important:** Committing secrets to a repository poses significant security risks. Please remove these secrets and consider them compromised.
```

## Excluding False Positives

The action includes a built-in allowlist to ignore common false positives, such as:

- Development database URLs (localhost connections)
- Test credentials and dummy passwords
- Common development patterns that aren't actual secrets

The file works just like a .gitignore file.  Every line is a regular expression pattern that will be evaluated.  Findings will be skipped if they match

### Custom Allowlist

You can override the built-in allowlist by creating a `.trufflehog-allowlist.txt` file in your repository root. This file should contain one regular expression pattern per line:

## Allowlist Pattern Format

Each line in the `.trufflehog-allowlist.txt` file is treated as a pattern:

- **Simple strings**: `example-password` matches exactly that string
- **Wildcards**: `AKIA*` matches any string starting with "AKIA"
- **Partial matching**: `database_password` will match `my_database_password_123`

Example patterns:

```
# Default TruffleHog Allowlist for common false positives
# Each line is a string pattern that will be matched against found secrets

#AWS Keys
AKIA*

# Database connection strings
jdbc:*://localhost

# Test credentials
test_*
```
