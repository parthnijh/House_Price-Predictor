



---



\# 🏠 House Price Prediction



A machine learning project to predict house prices using regression models such as XGBoost, Linear Regression, LightGBM, and Random Forest, based on the \[Kaggle House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) dataset.



---



\## 📂 Project Structure



```

house-price-prediction/

│

├── housepricepreds.ipynb      # Main notebook with all preprocessing, modeling, tuning

├── submission.csv             # Final output file for Kaggle submission

├── train.csv                  # Training dataset

├── test.csv                   # Test dataset for prediction

├── README.md                  # Project overview and instructions

```



---



\## 📊 Models Used



\* Linear Regression

\* XGBoost Regressor

\* LightGBM Regressor

\* Random Forest Regressor



---



\## ⚙️ Preprocessing Steps



\* Split numerical and categorical features

\* Used `SimpleImputer` for missing values:



&nbsp; \* \*\*Numerical\*\*: filled with median

&nbsp; \* \*\*Categorical\*\*: filled with "missing"

\* Applied `OneHotEncoding` for categorical variables

\* Used `ColumnTransformer` to combine preprocessing

\* Built `Pipeline` for each model to simplify fitting and transforming



---



\## 🔧 Model Evaluation



\* Evaluation metric: \*\*Log RMSE\*\*

\* Used `GridSearchCV` and `RandomizedSearchCV` for tuning hyperparameters

\* Feature importance extracted for XGBoost and Random Forest



---



\## 📝 How to Run



1\. Clone the repo or download the files.

2\. Install dependencies:



```bash

pip install pandas numpy scikit-learn xgboost lightgbm

```



3\. Run the Jupyter notebook:



```bash

jupyter notebook housepricepreds.ipynb

```



4\. Once predictions are made, the `submission.csv` file is generated using:



```python

submission.to\_csv("submission.csv", index=False)

```



5\. Upload `submission.csv` to \[Kaggle Submission Page](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/submit).



---



\## ✅ Submission Format



```

Id,SalePrice

1461,169000.1

1462,187724.1233

1463,175221.0

...

```



---





