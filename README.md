# Fetch Latest Release Version

A Github Action to fetch the latest release version for the current repository.

## Usage

```
jobs:
  job-name:
    runs-on: ubuntu-latest
    steps:

      - uses: actions/checkout@v3

      - name: Fetch latest release version
        id: fetch-latest-release
        uses: reloc8/action-latest-release-version@1.0.1

      - name: Test
        run: echo ${{ steps.fetch-latest-release.outputs.latest-release }}
``` 
