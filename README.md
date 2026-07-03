# Laptop Prices Analysis

This project explores and prepares a laptop pricing dataset for analysis. It includes the original laptop data, a feature-engineered dataset, and a Jupyter notebook used to create derived features.

## Project Structure

```text
.
|-- pyproject.toml
|-- README.md
`-- src
    |-- requirements.txt
    |-- data
    |   |-- raw
    |   |   `-- laptop_data.csv
    |   `-- feature_engineered
    |       `-- feature_engineered_data.csv
    `-- notebooks
        `-- feature_engineered.ipynb
```

## Data

- `src/data/raw/laptop_data.csv`: original laptop dataset.
- `src/data/feature_engineered/feature_engineered_data.csv`: processed dataset with extracted features such as screen width, screen height, CPU speed, CPU core type, storage size, and GPU type.

## Setup

Create and activate a virtual environment, then install the notebook dependencies:

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r src/requirements.txt
```

## Usage

Open the feature engineering notebook:

```bash
jupyter notebook src/notebooks/feature_engineered.ipynb
```

The notebook reads the raw laptop dataset, creates additional columns, and saves the processed data to `src/data/feature_engineered/feature_engineered_data.csv`.

## Requirements

Main Python packages:

- `pandas`
- `ipykernel`
- `ipywidgets`

See `src/requirements.txt` for pinned versions.
