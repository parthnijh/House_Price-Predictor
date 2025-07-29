# 🏠 House Price Prediction

A machine learning project to predict house prices using regression models such as XGBoost, Linear Regression, LightGBM, and Random Forest, based on the [Kaggle House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) dataset.

---

## 📊 Models Used

- Linear Regression  
- XGBoost Regressor  
- LightGBM Regressor  
- Random Forest Regressor  

---

## ⚙️ Preprocessing Steps

- Split numerical and categorical features  
- Used `SimpleImputer` for missing values:  
  - **Numerical**: filled with median  
  - **Categorical**: filled with `"missing"`  
- Applied `OneHotEncoder` for categorical variables  
- Used `ColumnTransformer` to combine preprocessing  
- Built `Pipeline` for each model to simplify fitting and transforming  

---

## 🔧 Model Evaluation

- Evaluation metric: **Log RMSE**  
- Used `GridSearchCV` and `RandomizedSearchCV` for hyperparameter tuning  
- Feature importance extracted for XGBoost and Random Forest  

---

## 📝 How to Run

1. Clone the repo or download the files  
2. Install dependencies:

```bash
pip install pandas numpy scikit-learn xgboost lightgbm
