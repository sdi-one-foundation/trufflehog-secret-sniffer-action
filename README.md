# trufflehog-secret-sniffer-action
A composite Github Action for running TruffleHog to detect secrets in the repository. It is triggered on every push to the main branch and every pull request.

A global tag will be created (see release.yml) on every release.  This global tag will have the format of "v\<major version\>" (example: v1).  This global tag will point to the most recent release.  The input needs to be change upon every major version change (v1 to v2).

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
```
