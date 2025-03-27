# Contributing to {{ cookiecutter.project_name }}

Thank you for considering contributing to this research! This document outlines the process for contributing to both the paper manuscript and the code.

## Code of Conduct

By participating in this project, you agree to maintain a respectful and constructive environment for everyone involved.

## How to Contribute

### Types of Contributions

We welcome several types of contributions:

1. **Paper feedback**: Suggestions for improving clarity, identifying errors, or proposing extensions
2. **Code improvements**: Bug fixes, performance improvements, or better documentation
3. **Alternative analyses**: New ways to analyze the data or additional experiments
4. **Theoretical extensions**: Ideas that build upon the concepts in the paper

### Process for Contributing

#### For Paper Contributions

1. **Open an issue** describing the change you'd like to see
2. **Discuss** the potential change with the authors
3. **Submit a pull request** with the proposed changes to the paper markdown file
   - Make focused changes that address a specific issue
   - Maintain the existing style and formatting
   - Add yourself to the acknowledgments section if appropriate

#### For Code Contributions

1. **Open an issue** describing the bug or feature
2. **Fork the repository**
3. **Create a branch** with a descriptive name
4. **Make your changes**, adhering to the code style
5. **Add or update tests** as needed
6. **Ensure all tests pass**
7. **Submit a pull request**

### Pull Request Process

1. Update the README.md or documentation with details of changes if appropriate
2. The authors will review your changes and may request additional changes
3. Once approved, your changes will be merged

## Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/{{ cookiecutter.project_slug }}.git
cd {{ cookiecutter.project_slug }}

# Install development dependencies
pip install -e ".[dev]"

# Run tests
pytest
```

## Style Guidelines

### For Paper

- Use clear, concise language
- Support claims with citations or evidence
- Follow consistent formatting for equations, figures, and tables

### For Code

- Follow PEP 8 style guidelines
- Write docstrings for all functions, classes, and modules
- Include comments for complex code sections
- Write tests for new functionality

## Recognition

All contributors will be acknowledged in the paper. Significant contributions may warrant authorship, which will be discussed on a case-by-case basis.

## Questions?

If you have any questions about contributing, please open an issue labeled "question".
