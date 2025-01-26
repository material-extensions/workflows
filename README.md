<!-- markdownlint-disable first-line-h1 -->

# ♻️ Reusable GitHub Workflows

A comprehensive collection of reusable GitHub Actions workflows that help standardize CI/CD practices across our organization.

## Overview

This repository contains a set of carefully crafted, reusable GitHub workflows that can be easily integrated into any our project. These workflows help maintain consistency, reduce duplication, and enforce best practices across all repositories.

## Available Workflows

### PR Title Check ([`pr-title.yml`](.github/workflows/pr-title.yml))

Validates Pull Request titles against conventional commit format.

```yaml
uses: material-extensions/workflows/.github/workflows/pr-title.yml@main
with:
  sparse-checkout: commitlint.config.js
  commitlint-help-url: https://www.conventionalcommits.org/en/v1.0.0/
```

### PR Closed ([`pr-closed.yml`](.github/workflows/pr-closed.yml))

Adds a thank you comment when PRs are closed.

```yaml
uses: material-extensions/workflows/.github/workflows/pr-closed.yml@main
with:
  comment: Thank you for your contribution! 🙏
```
