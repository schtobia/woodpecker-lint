<!--
SPDX-FileCopyrightText: 2023 Tobias Schmidl

SPDX-License-Identifier: AGPL-3.0-or-later
-->

# woodpecker-lint

This repository is intended to be used as a [pre-commit hook](https://pre-commit.com/#install).

## Versioning

This repository adheres to [SemVer](https://semver.org/lang/de/) and [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## Usage

Simple, add the second option to your `.pre-commit-config.yaml`.

<!-- editorconfig-checker-disable -->

```yaml
---
repos:
- repo: https://github.com/pre-commit/pre-commit-hooks
  rev: v4.4.0
  hooks:
  - id: check-yaml
  - id: end-of-file-fixer
  - id: trailing-whitespace
  - id: check-merge-conflict
- repo: https://git.schmidl.dev/schtobia/woodpecker-lint
  rev: 1.0.0
  hooks:
  - id: woodpecker-lint
...
```
<!--// editorconfig-checker-enable -->

## Alternative Repos

The base URL for this repository is and will always be on [git.schmidl.dev](https://git.schmidl.dev/schtobia/woodpecker-lint). However, I've enabled a push mirror to [Github](https://github.com/schtobia/woodpecker-lint).
