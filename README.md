# tartufo-action

> ⚠️ **DEPRECATED**: This GitHub Action has been deprecated and archived. We recommend using alternative secret scanning solutions like [GitHub's built-in secret scanning](https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning)

This GitHub Action scans your repository for secrets using [tartufo](https://github.com/godaddy/tartufo).

The target repository should be checked out before invoking this action. The tartufo.toml file in the checked out branch
will be used as the configuration.

## Inputs

## `entropy`

**Optional** Enable entropy checks. Default `"true"`.

## `regex`

**Optional** Enable regex checks. Default `"true"`.

## `scan-filenames`

**Optional** Enable filename checks. Default `"true"`.

## `output-format`

**Optional** The format in which the output is generated. Default `"text"`.

## `entropy-sensitivity`

**Optional** Modify entropy detection sensitivity. Default `"75"`.

## `branch`

**Optional** Scan only the specified branch. By default, all branches in the repository are scanned.

## `include-submodule`

**Optional** Scan git submodules. Default `"false"`.

## Example usage

uses: godaddy/tartufo-action@v1
