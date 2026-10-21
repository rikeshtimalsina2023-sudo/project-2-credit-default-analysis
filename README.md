# Project 2 — Credit Default Analysis

## Overview

This notebook explores and models credit-card payment default using the UCI **Default of Credit Card Clients** dataset. It follows an end-to-end, educational machine-learning workflow: loading and validating the data, exploratory analysis, feature engineering, model comparison, evaluation, and interpretation.

## Models

- Logistic Regression
- Decision Tree
- Random Forest

The models are evaluated with accuracy, precision, recall, F1 score, ROC-AUC, a confusion matrix, and ROC curves. Recent payment-status features, credit limit, payment amounts, and bill amounts are examined as potential signals.

## Repository contents

- `credit_default_analysis_final.ipynb` — complete analysis and model-comparison workflow
- `default of credit card clients.xls` — original dataset file required by the notebook
- `requirements.txt` — Python dependencies

## Run locally

1. Create and activate a Python 3.10+ virtual environment.
2. Install dependencies: `python -m pip install -r requirements.txt`
3. Launch Jupyter: `jupyter notebook credit_default_analysis_final.ipynb`
4. Run all cells from top to bottom.

For a non-interactive reproducibility check:

```bash
MPLBACKEND=Agg jupyter nbconvert --to notebook --execute --stdout credit_default_analysis_final.ipynb > /dev/null
```

## Data source and attribution

The included data is the **Default of Credit Card Clients** dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients), donated in 2016 and credited to I-Cheng Yeh (2009). UCI licenses this dataset under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); it is included here with attribution for educational and portfolio use.

## Important limitations

This is an educational analysis, not a credit-decisioning system. It uses historical data from Taiwan, reflects an imbalanced target, and has not been validated for production or for fairness, regulatory compliance, or other populations. Predictions should never be used by themselves to approve, deny, or price credit.

## Skills demonstrated

Python, Pandas, NumPy, exploratory data analysis, feature engineering, train/test splitting, scaling, classification, model evaluation, feature importance, and responsible-modeling considerations.
