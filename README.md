# Rain Prediction in Australia — Learning Notebook (scikit-learn)

This repository contains **my learning notebook** for predicting next-day rain in the Melbourne region, using
`pandas` and `scikit-learn`. The notebook **intentionally keeps course-style prompts + my answers** as proof of learning.

> **Provenance:** Inspired by coursework on Coursera. This repo includes **my own run and code** only.
> Course content and datasets are **not** redistributed. See `NOTICE.md`.

## Setup
```bash
pip install -r requirements.txt
jupyter notebook
```
Open `notebooks/Project Predicting Weather machine learning.ipynb` and run all cells top-to-bottom.

## Data
Use the public *Rain in Australia* dataset (e.g., Kaggle / UCI). Place the CSV locally and follow the notebook steps.
**Always check the dataset's license** at the source.

## What the notebook covers
- Feature engineering (`Season` from `Date`), cleaning, train/test split with stratification
- Preprocessing via `ColumnTransformer` (scaling numeric, One-Hot encoding categoricals)
- Two models: **RandomForest** and **Logistic Regression** tuned with **GridSearchCV**
- Evaluation: accuracy, classification report, confusion matrix, feature importances

## Example result (from my run)
- RandomForest test accuracy ≈ **84%**, TPR (Rain=Yes) ≈ **51%**
> Numbers vary by data slice and seeds.

## License
Code: **MIT** (see `LICENSE`). Data: under its **original source license**.
