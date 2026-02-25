# Contributing to Webex Samples Template

Thank you for your interest in contributing to the Webex Samples Template! We appreciate your help in maintaining and improving this framework for the Webex Samples organization.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
- [Development Setup](#development-setup)
- [Pull Request Process](#pull-request-process)
- [Style Guide](#style-guide)
- [Getting Help](#getting-help)

## Code of Conduct

This project follows the Webex Samples organization standards. Please be respectful and constructive in all interactions.

## How to Contribute

We welcome several types of contributions:

- **Bug reports**: Found something broken? Open an issue using the bug report template
- **Feature requests**: Have an idea to improve the template? Use the feature request template
- **Documentation**: Improvements to README, this guide, or other docs
- **Code**: Fixes, enhancements, or new features via pull requests

## Development Setup

1. **Clone the repository**:

   ```bash
   git clone <your-repo-url>
   cd Webex-Samples-Template
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Install Ruff** (for Python linting):

   ```bash
   pip install ruff
   ```

4. **Enable pre-commit hooks** (optional but recommended): Uncomment the lines in [.husky/pre-commit](.husky/pre-commit) to run Prettier and Ruff automatically before each commit.

## Pull Request Process

1. **Create a branch** from `main` for your changes
2. **Ensure code compiles and passes all linters** before committing. Run:
   - `npx prettier . --check` and `npx prettier . --write` if needed
   - `ruff check .` and `ruff check --fix .` for Python files
3. **Commit your changes** with clear, descriptive messages
4. **Open a pull request** using the PR template
5. **Address review feedback** promptly
6. **Wait for CI**—all GitHub Actions (Prettier, Ruff) must pass before merging

**Important**: Code must compile and pass all linters before committing. Do not push code that fails the Prettier or Ruff checks.

## Style Guide

- **JavaScript, JSON, Markdown, YAML**: Use [Prettier](https://prettier.io) for formatting
- **Python**: Use [Ruff](https://docs.astral.sh/ruff/linter/) for linting

See the [README](README.md) for detailed instructions on running Prettier and Ruff locally.

## Getting Help

- **Adam Weeks** (adweeks)
- **Ashton Jordan** (ashjorda)

Reach out to Adam or Ashton for questions about the template, adding repos to the organization, or making repos public.
