# Contributing

Thank you for your interest in contributing! This is the default contributing guide for every
public repository owned by [Chris-Wolfgang](https://github.com/Chris-Wolfgang). Many repositories
have their own `CONTRIBUTING.md` with project-specific build, test, and code-quality rules; when
one exists, it takes precedence over this file.

## How Can You Contribute?

You can contribute in several ways:
- Reporting bugs
- Suggesting enhancements
- Submitting pull requests for new features or bug fixes
- Improving documentation
- Writing or improving tests

**Please note:** Before coding anything, please check with me first by opening an issue and getting
approval for it. Pull requests are more likely to be merged if I have agreed to the changes.

Security vulnerabilities are the exception: do **not** open a public issue. Follow the
[security policy](https://github.com/Chris-Wolfgang/.github/blob/main/SECURITY.md) instead.

---

## Getting Started

1. **Fork the repository** and clone it locally.
2. **Enable the pre-commit secret scan**, if the repository has a `.githooks/pre-commit` file
   (once per clone). The hook runs [gitleaks](https://github.com/gitleaks/gitleaks) and blocks
   commits containing secrets (credentials, tokens, private keys):
   ```sh
   git config core.hooksPath .githooks
   ```
   Install the `gitleaks` CLI: `winget install gitleaks` (Windows), `brew install gitleaks` (macOS), or a
   binary from the [releases page](https://github.com/gitleaks/gitleaks/releases) (Linux).
3. **Create a new branch** for your feature or bug fix:
   ```sh
   git checkout -b your-feature-name
   ```
4. **Make your changes** and commit them with clear messages.
5. **Push your branch** to your fork and **open a pull request** describing your changes and
   referencing the issue it addresses.
6. **Check the PR checks.** Each repository runs its own set of checks on pull requests (for
   example builds and tests, coverage gates, secret scanning, CodeQL, and workflow linting). If a
   check fails, read its log, fix, and push.

---

## Guidelines

- Follow the coding style already used in the repository (most repositories enforce it through
  `.editorconfig` and analyzers).
- Write clear, concise commit messages.
- Add relevant tests for new features or bug fixes.
- Keep changes focused and atomic: one feature or fix per pull request.
- Update documentation when you change behavior or public APIs.
- Respond to review feedback in a timely manner.

---

## Code of Conduct

Please be respectful and considerate in all interactions. See the
[Code of Conduct](https://github.com/Chris-Wolfgang/.github/blob/main/CODE_OF_CONDUCT.md) for our
community guidelines.

---

Thank you for contributing!
