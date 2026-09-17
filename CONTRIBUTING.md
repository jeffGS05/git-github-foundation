# Contributing Guidelines

Thank you for contributing to this project.

This repository is used to demonstrate professional Git and GitHub practices as part of an engineering portfolio.

## Development Workflow

### 1. Create a Feature Branch

Create a dedicated branch for each change:

```bash
git checkout -b feature/<short-description>
```

Example:

```bash
git checkout -b feature/update-documentation
```

### 2. Make Changes

Keep changes focused and avoid mixing unrelated modifications in the same branch.

### 3. Review Changes

Before committing, review the working tree:

```bash
git status
git diff
```

Stage the intended files:

```bash
git add <file>
```

Review the staged changes:

```bash
git diff --cached
```

### 4. Commit Changes

Use clear and descriptive commit messages.

This repository follows a Conventional Commits style:

```text
feat: add new functionality
fix: correct an issue
docs: update documentation
chore: maintenance changes
ci: update CI configuration
security: improve security controls
refactor: restructure existing code
```

Example:

```bash
git commit -m "docs: improve branching documentation"
```

### 5. Push the Branch

```bash
git push -u origin feature/<short-description>
```

### 6. Pull Request

Open a Pull Request on GitHub.

The Pull Request should:

* Clearly describe the change
* Explain why the change was necessary
* Identify any relevant testing performed
* Avoid unrelated changes

### 7. Merge

After reviewing the Pull Request, merge the branch into `main`.

Delete the feature branch after it is no longer required.

## Documentation Standards

Documentation should be:

* Clear
* Concise
* Technically accurate
* Reproducible
* Written using Markdown where appropriate

Commands should include enough context for another engineer to reproduce the documented procedure.

## Security

Never commit:

* Passwords
* API keys
* Private SSH keys
* Cloud credentials
* Certificates containing private keys
* `.env` files containing secrets
* Other sensitive credentials

Use placeholders or example configuration files instead.

## Code Quality

Changes should prioritize:

* Readability
* Maintainability
* Simplicity
* Reproducibility
* Security

Automated validation should be used where practical.

## Issues

Issues should contain enough information to understand the problem or proposed improvement.

Include, when applicable:

* Description
* Expected behavior
* Actual behavior
* Steps to reproduce
* Relevant logs or error messages
* Environment information

