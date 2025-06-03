# TruffleHog Secret Sniffer Action

A composite GitHub Action for running TruffleHog to detect secrets in your repository. This action scans your codebase for sensitive information such as API keys, passwords, and tokens to prevent accidental exposure of credentials.

A global tag will be created (see release.yml) on every release. This global tag will have the format of "v\<major version\>" (example: v1). This global tag will point to the most recent release. The input needs to be changed upon every major version change (v1 to v2).

## Features

- **Automated Secret Detection**: Leverages TruffleHog to find exposed secrets in your code
- **Pull Request Comments**: Automatically comments on PRs with details about detected secrets
- **Email Notifications**: Sends detailed email alerts when secrets are found
- **Configurable**: Works with both push events and pull requests

## How It Works

This action performs the following steps:

1. **Checkout Code**: Uses `actions/checkout` to get your repository code
2. **Run TruffleHog**: Scans your repository using the official TruffleHog action
3. **Process Results**: Analyzes the TruffleHog output to extract useful information
4. **Notify Developers**: Posts comments on pull requests with details about detected secrets
5. **Send Email Alert**: Sends an email notification to the security team with detailed findings
6. **Fail Build**: If secrets are detected, the workflow will fail to prevent merging code with secrets

## Usage

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
- Details about the detected secrets including file and line information
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

## Troubleshooting

If you encounter issues with this action:

1. **No Email Received**: Verify your SES credentials and ensure the email address is verified in AWS SES
2. **Action Fails**: Check the GitHub Actions logs for detailed error messages
3. **False Positives**: TruffleHog may occasionally flag non-secret values; review findings carefully
4. **
