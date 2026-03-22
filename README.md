# House Price Prediction with Explainable AI (SHAP)

## Overview
An end-to-end machine learning project that predicts California house prices 
using XGBoost and explains every prediction using SHAP (SHapley Additive Explanations).

## Problem Statement
Given features like location, income level, house age, and number of rooms — 
predict the median house value and explain which factors drove that prediction.

## Dataset
- Source: California Housing Prices (Kaggle)
- 20,640 records, 10 features
- Target variable: median_house_value

## Tech Stack
- Python, Google Colab
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn, XGBoost
- SHAP

## Project Steps
1. Data loading and exploratory data analysis (EDA)
2. Data cleaning — handled 207 missing values
3. Feature engineering — created 3 meaningful ratio features
4. Model building — XGBoost vs Linear Regression comparison
5. Model evaluation — R², RMSE metrics
6. SHAP explainability — feature importance, beeswarm, waterfall charts
7. Model testing — actual vs predicted, custom house prediction

## Results
| Model | R² Score | RMSE |
|---|---|---|
| Linear Regression | ~0.65 | ~$53,000 |
| XGBoost | ~0.83 | ~$31,000 |

XGBoost outperformed the baseline by 18% in R² score.

## Key Insights from SHAP
- `median_income` is the strongest predictor of house price
- Ocean proximity significantly boosts predicted price
- Older houses and dense populations negatively impact price

## How to Run
1. Clone this repo or open notebook directly in Google Colab
2. Run all cells in order
3. No additional setup needed — all libraries available in Colab

## Author
Gokul Kanna S — [LinkedIn](https://www.linkedin.com/in/gokul-kanna-170b4a193/)
