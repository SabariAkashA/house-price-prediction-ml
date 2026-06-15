# House Price Prediction using Machine Learning

## Overview
This project predicts house prices using machine learning regression models. The goal was to compare multiple algorithms and understand how different models perform on structured tabular data.

## Dataset
[House Prices: Advanced Regression Techniques](https://www.kaggle.com/datasets/rishitaverma02/house-prices-advanced-regression-techniques/data)

Target Variable:
- SalePrice

Features:
- Lot size
- Neighborhood
- Garage details
- Basement details
- Construction year
- House quality

 ## Data Preprocessing
- Handled missing values using domain-specific strategies
- Filled structural missing values with "None"
- Used median imputation for numerical features
- Used mode imputation for rare categorical missing values
- Applied One-Hot Encoding to categorical variables

## Models Evaluated

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. XGBoost Regressor

## Result
| Model             | MAE   | RMSE  | R²    |
| ----------------- | ----- | ----- | ----- |
| Linear Regression | 23922 | 83010 | 0.10  |
| Decision Tree     | 27008 | 83010 | 0.77  |
| Random Forest     | 17696 | 29186 | 0.889 |
| XGBoost           | 15972 | 25816 | 0.913 |

## Key Learnings

- Linear Regression struggled to capture complex housing patterns.
- Decision Trees improved performance but were prone to overfitting.
- Random Forest significantly improved generalization.
- XGBoost achieved the best overall performance.
- Proper preprocessing had a major impact on model quality.

## Tech Stack
- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- Jupyter Notebook
