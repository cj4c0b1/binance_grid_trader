# Contributing to Binance Grid Trader

Thank you for your interest in contributing to the Binance Grid Trader project! This document outlines the process for contributing to the project.

## Git Workflow

We follow the [Git Flow](https://nvie.com/posts/a-successful-git-branching-model/) branching model with the following main branches:

- `main` - Production-ready code (protected branch)
- `develop` - Integration branch for features (protected branch)
- `feature/*` - Feature branches for new functionality
- `bugfix/*` - Bug fix branches
- `hotfix/*` - Hotfix branches for production issues
- `release/*` - Release preparation branches

## Branch Naming Conventions

- `feature/descriptive-name` - New features
- `bugfix/issue-number-description` - Bug fixes
- `hotfix/issue-number-description` - Critical production fixes
- `release/version-number` - Release preparation

## Commit Message Format

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Commit Types

- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that do not affect the meaning of the code
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `perf`: A code change that improves performance
- `test`: Adding missing tests or correcting existing tests
- `chore`: Changes to the build process or auxiliary tools

## Pull Request Process

1. Fork the repository and create your branch from `develop`
2. Make your changes following the coding standards
3. Add tests if applicable
4. Update the documentation if needed
5. Ensure all tests pass
6. Submit a pull request to the `develop` branch

## Code Style

- Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) for Python code
- Use type hints for better code documentation
- Write docstrings for all public functions and classes
- Keep functions small and focused on a single responsibility

## Development Setup

1. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

2. Install development dependencies:
   ```bash
   pip install -r requirements-dev.txt
   ```

3. Install pre-commit hooks:
   ```bash
   pre-commit install
   ```

## Testing

Run the test suite with:

```bash
pytest
```

## Code Review Process

- At least one approval is required before merging
- All CI checks must pass
- Code should be reviewed by at least one other developer
- Keep PRs small and focused on a single feature or fix

## Reporting Issues

Please use GitHub Issues to report any bugs or suggest new features. Include as much detail as possible to help us understand and reproduce the issue.

## License

By contributing, you agree that your contributions will be licensed under the project's [LICENSE](LICENSE) file.
