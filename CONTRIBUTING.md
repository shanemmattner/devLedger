# Contributing to DevLedger

Thank you for your interest in contributing to DevLedger! This document provides guidelines and instructions for contributing to the project.

## Development Setup

### Prerequisites
- Python 3.8 or higher
- Git 2.25 or higher
- Virtual environment management tool (venv, conda, etc.)

### Setting Up Development Environment

1. Clone the repository:
```bash
git clone https://github.com/yourusername/devledger.git
cd devledger
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install development dependencies:
```bash
pip install -e ".[dev]"
```

4. Install pre-commit hooks:
```bash
pre-commit install
```

### Optional Components
For enhanced functionality, you may want to install:
- `chromadb` for vector storage capabilities
- `transformers` for local LLM support
- Cloud LLM provider SDKs (openai, anthropic)

## Development Workflow

### Coding Standards

1. **Python Style Guide**
   - Follow PEP 8 style guide
   - Use type hints for function arguments and return values
   - Document functions and classes using docstrings
   - Maximum line length: 88 characters (Black formatter)

2. **Comment Patterns**
   - Use DevLedger's comment pattern system:
     - Information comments: `# I5-`
     - Debug comments: `# D5-`
     - Technical comments: `# T5-`
   - Include rationale for non-obvious implementation decisions

3. **Testing**
   - Write unit tests for new functionality
   - Maintain or improve test coverage
   - Include integration tests for complex features
   - Test both local and cloud LLM scenarios

4. **Documentation**
   - Update relevant documentation for new features
   - Include docstrings for public APIs
   - Add examples for new functionality
   - Update type hints when modifying interfaces

### Git Workflow

1. **Branch Naming**
   - Feature branches: `feature/description`
   - Bug fixes: `fix/description`
   - Documentation: `docs/description`
   - Performance improvements: `perf/description`

2. **Commit Messages**
   - Use clear, descriptive commit messages
   - Follow conventional commits format:
     ```
     type(scope): description
     
     [optional body]
     [optional footer]
     ```
   - Types: feat, fix, docs, style, refactor, perf, test, chore

## Pull Request Process

1. **Before Submitting**
   - Create a feature branch from `main`
   - Ensure all tests pass locally
   - Run pre-commit hooks
   - Update documentation if needed
   - Add tests for new functionality

2. **PR Description**
   - Clearly describe the changes
   - Reference any related issues
   - Include screenshots for UI changes
   - List any breaking changes
   - Mention any new dependencies

3. **Review Process**
   - PRs require at least one reviewer approval
   - Address review comments promptly
   - Keep PRs focused and reasonably sized
   - Ensure CI checks pass

4. **After Merge**
   - Delete the feature branch
   - Update relevant documentation
   - Monitor CI/CD pipeline

## Development Tools

### Recommended IDE Setup
- VSCode with Python extension
- Recommended extensions:
  - Python
  - Pylance
  - Python Test Explorer
  - GitLens
  - Python Docstring Generator

### Code Quality Tools
- Black for code formatting
- isort for import sorting
- flake8 for linting
- mypy for type checking
- pytest for testing

## Getting Help

- Create an issue for bugs or feature requests
- Join our community discussions
- Check existing documentation and issues
- Reach out to maintainers if stuck

## License

By contributing to DevLedger, you agree that your contributions will be licensed under the MIT License.