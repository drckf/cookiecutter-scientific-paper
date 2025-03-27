# Analysis Code

This directory contains the code used to analyze data and generate results for the paper.

## Directory Structure

- `analysis/` - Scripts for data analysis and figure generation
- `experiments/` - Code to run experiments described in the paper
- `notebooks/` - Jupyter notebooks for exploration and visualization

## Getting Started

### Prerequisites

- Python 3.7+
- Dependencies listed in `requirements.txt`

### Installation

```bash
# Install dependencies
pip install -r requirements.txt

# Install the package from the parent directory
pip install -e ../src
```

## Running the Analysis

To reproduce all results and figures in the paper:

```bash
python -m analysis.run_all
```

To run specific analyses:

```bash
python -m analysis.figure1
python -m analysis.table1
# etc.
```

## Experiments

Each experiment can be run individually:

```bash
python -m experiments.experiment1 --param1=value1 --param2=value2
```

See the docstrings in each experiment file for specific parameters and options.

## Results

Analysis results are saved to:

- Figures: `../paper/figures/`
- Tables: `../paper/tables/`
- Processed data: `../data/processed/`

## Adding New Analyses

To add a new analysis:

1. Create a new script in the `analysis/` directory
2. Add your analysis function
3. Add it to the imports in `analysis/run_all.py`
