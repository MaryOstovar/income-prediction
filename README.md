# Income Prediction Project

## Overview
This project aims to predict income levels using the UCI Adult dataset. It leverages data science and machine learning techniques to preprocess data, build predictive models, and evaluate their performance. The project is structured for clarity and reproducibility, supporting notebook-based workflows.

## Directory Structure
```
income-prediction/
├── main.py                  # Entry point for running scripts
├── income-prediction/
│   ├── Makefile             # Automation commands
│   ├── pyproject.toml       # Project metadata and dependencies
│   ├── README.md            # Project documentation
│   ├── requirements.txt     # Python dependencies
│   ├── data/
│   │   ├── interim/         # Intermediate data (train/test/val splits)
│   │   ├── processed/       # Preprocessed data and artifacts
│   │   └── raw/             # Raw data (e.g., adult.csv)
│   └── notebooks/
│       ├── business-understanding.ipynb
│       ├── data-prepration.ipynb
│       ├── data-understanding.ipynb
│       └── modeling.ipynb
```

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd income-prediction
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Data Description
- **raw/adult.csv**: Original UCI Adult dataset. The user should manually place the adult.csv file in this directory before starting.
- **interim/**: Contains train.csv, test.csv, val.csv (split datasets). This folder is populated during the data preparation phase, but must exist prior to running scripts or notebooks.
- **processed/**: Preprocessed features and targets, including joblib and npz files. This folder is also filled during data preparation, but must exist before execution.

## Usage
- Explore and run Jupyter notebooks in the `notebooks/` directory for step-by-step analysis:
  - business-understanding.ipynb
  - data-prepration.ipynb
  - data-understanding.ipynb
  - modeling.ipynb

## Notes
- Ensure data files are present in the appropriate directories before running scripts or notebooks.

## CRISP-DM Methodology
This project follows the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology, which is a structured approach to data science and machine learning projects. The workflow is organized into the following phases, each supported by dedicated Jupyter notebooks:

- **Business Understanding**: Identifying the project objectives and requirements from a business perspective. See `notebooks/business-understanding.ipynb`.
- **Data Understanding**: Collecting, describing, and exploring the data to gain insights. See `notebooks/data-understanding.ipynb`.
- **Data Preparation**: Cleaning, transforming, and organizing data for modeling. See `notebooks/data-prepration.ipynb`.
- **Modeling & Validation**: Building machine learning models, tuning parameters, and validating performance. Both modeling and validation are covered in `notebooks/modeling.ipynb`.

## References
- [UCI Adult Dataset](https://www.kaggle.com/datasets/uciml/adult-census-income)
