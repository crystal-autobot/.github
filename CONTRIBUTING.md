# Contributing to Autobot

We welcome contributions! Here's how to get started.

## Setup

**Prerequisites:** [Crystal](https://crystal-lang.org/install/) >= 1.10.0, Make, Docker (optional, for sandbox testing on macOS)

```bash
git clone https://github.com/YOUR_USERNAME/autobot.git
cd autobot
make deps
make build
```

## Workflow

1. Create a feature branch from `main`
2. Make your changes and add tests
3. Run checks before committing:

```bash
make format    # Auto-format code
make lint      # Ameba linter (no warnings allowed)
make test      # All tests must pass
```

4. Open a pull request with a clear description

For major features, please open an issue first to discuss the approach.

## Code quality

- All code must pass `make lint` — no exceptions
- Max cyclomatic complexity: 10. Extract methods instead of ignoring the rule
- Follow the [Crystal style guide](https://crystal-lang.org/reference/conventions/coding_style.html)
- Add tests for new functionality in `spec/`
- Update `docs/` if your changes affect user-facing behavior

## Code of conduct

This project follows the [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to abide by its terms.

## License

Contributions are licensed under the [MIT License](https://github.com/crystal-autobot/autobot/blob/main/LICENSE).
