# 🏠 Housing Price Prediction using Advanced Regression Techniques

This repository contains a machine learning project aimed at predicting house sale prices using the Ames Housing Dataset. This project was developed as part of my participation in the [Kaggle House Prices Competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques), and is implemented in Python using popular ML libraries.

---

## 🎯 Project Goal

To build a regression model that can accurately predict the sale prices of homes in Ames, Iowa using 79 explanatory variables describing every aspect of residential homes.

---
## 📊 Workflow Summary

### 📌 1. Data Loading and Initial Exploration
- Loaded training and test datasets
- Visualized missing values using heatmaps
- Displayed data types and initial statistics

### 📌 2. Data Preprocessing
- Imputed missing values using mean/mode or labeled as "None"
- Applied one-hot encoding to categorical features
- Performed log transformation on skewed numerical features
- Normalized data using standard scaling

### 📌 3. Feature Engineering
- Created new features (`TotalSF`, `TotalBathrooms`, etc.)
- Removed redundant or highly correlated features
- Combined and grouped features for better predictive power

### 📌 4. Model Training
Trained and evaluated the following models:
- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **ElasticNet**
- **XGBoost Regressor**
- **LightGBM Regressor**

### 📌 5. Model Evaluation
- Used **Root Mean Squared Error (RMSE)** on log-transformed SalePrice
- Cross-validated each model to avoid overfitting
- Compared scores and performance for each model

### 📌 6. Ensembling
- Combined multiple models using simple averaging and stacking
- Improved generalization and reduced variance

### 📌 7. Submission
- Generated `submission.csv` with final predictions
- Ready to be uploaded to the Kaggle competition portal

---

## 📈 Metric Used

Evaluation is based on RMSE of the log of predicted SalePrice values:

\[
\text{RMSE} = \sqrt{\frac{1}{n} \sum (\log(\hat{y}) - \log(y))^2}
\]

---

## 🛠 Tools & Technologies

- Python
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- LightGBM
- Jupyter Notebook

---
## 🧠 Key Learnings

- Importance of handling missing values carefully
- Impact of log transformation and scaling on regression models
- Feature engineering and ensembling can significantly improve accuracy
- Cross-validation is crucial to avoid overfitting

---

## 📌 Future Work

- Use SHAP values for interpretability
- Deploy the model using Flask or Streamlit
- Automate the pipeline with `scikit-learn` Pipelines

---

## 🙋‍♂️ Author

**Kaarthikeyan SS**  
📍 Bengaluru, India  
🧑‍🎓 Post Graduate in Data Science & Engineering  
✉️ kaarthikeyan0909@gmail.com


