# {{ cookiecutter.paper_title }}

[![Build Status](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/workflows/Build%20Paper/badge.svg)](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/actions)
[![Tests](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/workflows/Test%20Package/badge.svg)](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/actions)
[![Paper](https://img.shields.io/badge/paper-GitHub%20Pages-blue)](https://{{ cookiecutter.github_username }}.github.io/{{ cookiecutter.project_slug }})
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)
[![License](https://img.shields.io/badge/License-{{ cookiecutter.open_source_license | replace("-", "--") }}-blue.svg)](https://opensource.org/licenses/{{ cookiecutter.open_source_license }})

## About

{{ cookiecutter.project_short_description }}

This repository contains the full manuscript, code, and data to reproduce the research presented in our paper.

## Paper

The paper is available in multiple formats:

- [Read online (GitHub Pages)](https://{{ cookiecutter.github_username }}.github.io/{{ cookiecutter.project_slug }})
- [Markdown source (paper.md)](paper/paper.md)
- [PDF version](https://{{ cookiecutter.github_username }}.github.io/{{ cookiecutter.project_slug }}/paper.pdf)

## Code

This repository includes:

1. A Python package (`src/{{ cookiecutter.package_name }}`) implementing the core methods described in the paper
2. Analysis scripts and experiments (`code/`) that use this package to generate the results in the paper

### Installation

```bash
# Install the package in development mode
pip install -e .

# Install analysis requirements
pip install -r code/requirements.txt
```

### Reproducing Results

```bash
# Run the analysis pipeline
cd code
python -m analysis.run_all
```

## Data

- `data/raw/`: Original, unmodified data
- `data/processed/`: Processed data ready for analysis

See the [data README](data/README.md) for details on data sources and processing steps.

## Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

The following types of contributions are especially valuable:
- Bug fixes in code or analysis
- Alternative analyses of our data
- Suggestions for improving clarity in the paper
- Extensions to our methods

## Citation

If you use this work in your research, please cite:

```bibtex
{% raw %}
@article{author-year,
  title     = "{{ cookiecutter.paper_title }}",
  author    = "{{ cookiecutter.author_name }}",
  journal   = "",
  year      = {{ cookiecutter.year }},
  doi       = "10.5281/zenodo.XXXXXXX"
}
{% endraw %}
```

## License

This project is licensed under the {{ cookiecutter.open_source_license }} License - see the [LICENSE](LICENSE) file for details.
