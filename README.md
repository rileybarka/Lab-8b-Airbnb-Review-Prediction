[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rileybarka/Lab-8b-Airbnb-Review-Prediction/blob/main/notebooks/Lab8b.ipynb)

# Airbnb Review Prediction - Custom Machine Learning Project

This project uses NYC Airbnb listings data to predict overall review scores based on host and listing features. The process follows the full ML lifecycle - from exploratory data analysis (EDA) through model training, tuning, and interpretation.

---

## Dataset

| Dataset               | Description                                                  |
|-----------------------|--------------------------------------------------------------|
| Airbnb Listings NYC   | Detailed NYC Airbnb data including host details, property info, and review metrics, used to predict `review_scores_rating`. |

---

## Objectives

- Select the Airbnb dataset and define the ML problem: predict review scores (regression)  
- Load and explore the data with EDA  
- Define a project plan based on insights  
- Prepare data for modeling (cleaning, feature engineering, handling missing values)  
- Fit models to training data and evaluate performance  
- Iteratively improve the model through feature engineering and hyperparameter tuning  
- Interpret feature importance and residual patterns  

---

## Methodology

1. **Data loading and exploration** — inspected missing values, feature distributions, and correlations  
2. **Problem definition and project planning** — identified features and target (`review_scores_rating`)  
3. **Data preparation and feature engineering** — handled missing values, transformed price, created missing indicators, encoded categoricals  
4. **Model selection, training, and evaluation** — tested Ridge Regression, Random Forest, and Gradient Boosting models  
5. **Model tuning and improvement** — used `RandomizedSearchCV` for Gradient Boosting, added new features, and improved RMSE/R²  
6. **Model interpretation** — analyzed feature importances to understand drivers of review scores  

---

## Results

- **Final model**: Tuned Gradient Boosting Regressor  
- **Performance**: RMSE ≈ 0.476, R² ≈ 0.111  
- **Key features**: Host’s private room listings, reviews per month, total listings count, entire homes listed, price  

---

## Setup Instructions

### Open in Google Colab  
Click the badge above.

### Run Locally

```bash
git clone https://github.com/rileybarka/Lab-8b-Airbnb-Review-Prediction.git
cd Lab-8b-Airbnb-Review-Prediction/notebooks
jupyter notebook Lab8b.ipynb
