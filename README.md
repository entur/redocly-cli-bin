# redocly-cli-bin
Building executables of the [redocly-cli](https://github.com/redocly/redocly-cli) OpenAPI toolset for use primarily in CI/CD workflows. Uses release-please to create Github releases, and then attaches built executables to the release.

## Why?
Entur uses [redocly-cli](https://github.com/redocly/redocly-cli) to bundle OpenAPI specs. It is used in Github reusable workflows [entur/gha-api](https://github.com/entur/gha-api). The recommended way of running Redocly is to download it from npm and run the script. However, we would like to avoid being dependent on npm during runtime execution of workflows, both for security and performance. Redocly does not provide binaries, so we build one here.
