# House Price Prediction — ML Portfolio

Project aimed at predicting house sale prices using the Ames Housing dataset. This repository is organized as a recruiter-ready project demonstrating end-to-end data science workflow: data loading, cleaning, feature engineering, model building, evaluation, and producing a submission.

## Project Overview
- Predict sale prices for residential properties using structured tabular data (Ames Housing).

## Problem Statement
- Given historic housing features, build a regression model to estimate `SalePrice` for unseen properties.

## Dataset
- Source: local `data/` folder with `train.csv` and `test.csv`.
- Generated submissions are exported to `outputs/submission.csv`.

## Tech Stack
- Python, pandas, NumPy, scikit-learn, matplotlib, seaborn, SciPy

## Workflow
1. Import libraries
2. Load dataset
3. Data cleaning & missing-value handling
4. Exploratory Data Analysis (EDA)
5. Feature engineering (custom transformers)
6. Pipeline construction and model training (ElasticNet + GridSearchCV)
7. Evaluation and submission generation

## Model Used
- `ElasticNet` (scikit-learn) with a preprocessing pipeline including numeric/categorical handling and custom transformers.

## Results
- See the notebook for cross-validation scores and final test predictions: `notebooks/house_price_prediction_pipeline.ipynb`.

## Key Learnings
- Importance of robust preprocessing pipelines and avoiding data leakage.
- Feature engineering and regularization help generalize to unseen data.

## Future Improvements
- Try regularized linear models (Ridge/Lasso) and compare coefficients.
- Try tree-based models (Random Forest, XGBoost) for non-linear patterns.
- Deploy a simple Streamlit app to showcase predictions and model explainability.

## Files
- `data/` — dataset CSVs
- `notebooks/` — polished notebook
- `outputs/` — exports including `submission.csv` and PNG charts

## Output Preview
![Sale Price Distribution](outputs/saleprice_distribution.png)

![Top Features Correlation](outputs/top_feature_correlation.png)

---

This project demonstrates a complete machine learning workflow for house price prediction, from data preprocessing and EDA to model training, evaluation, and submission-ready outputs.