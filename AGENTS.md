# AGENTS.md

Project context for AI coding agents (Cursor, GitHub Copilot, etc.) working on the Webex Samples Template.

## Project Overview

This is the **Webex Samples Template** repository—a standardized framework for creating code contributions to the Webex Samples organization. Projects created from this template are intended to be **open sourced and used by customers and partners**. The template provides a consistent structure, linting tools, and GitHub Actions for all new sample repositories.

## Tech Stack

- **Node.js**: Prettier, ESLint, Husky, lint-staged
- **Python**: Ruff (linter)

## Format and Lint Commands

### Prettier (JavaScript, JSON, Markdown, YAML)

```bash
npx prettier . --check    # Check formatting
npx prettier . --write     # Apply formatting
npm run format             # Same as --write
```

### Ruff (Python)

```bash
ruff check .              # Check for issues
ruff check --fix .        # Auto-fix issues
```

## Pre-Commit Hooks

Husky and lint-staged run automatically before each commit when enabled. To enable, uncomment the lines in [.husky/pre-commit](.husky/pre-commit):

```bash
npx lint-staged
ruff check --fix .
```

## Dev Environment Tips

- Use `npm run format` for Prettier formatting
- Use a Python virtual environment when running Ruff
- Run `npm ci` to install dependencies (use `npm ci` in CI, not `npm install`)

## Quality Rules

**Code must compile and pass all linters before committing.** Run Prettier and Ruff (or enable pre-commit hooks) to ensure checks pass locally before pushing. All GitHub Actions workflows must pass before a pull request can be merged.

## Pull Request Instructions

- All workflows (Prettier, Ruff) must pass before merging
- Contact Adam Weeks (adweeks) or Ashton Jordan (ashjorda) to have a new repo added to the Webex Samples organization
- New repos are private by default; contact Adam or Ashton for review to make the repo public
