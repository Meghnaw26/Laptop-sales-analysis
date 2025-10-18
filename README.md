# Laptop-Sales-Analysis

## Project Type: Data Analyst/ Data Science

## Project Overview
A comprehensive analysis of laptop specifications and pricing to understand factors that drive price, build predictive models to estimate price (in Euros), and create visual dashboards to communicate insights. The project combines exploratory data analysis (EDA), data cleaning, feature engineering, and supervised machine learning.


## Tools and Technologies
- Python (pandas, numpy)
- Jupyter Notebook
- Visualization: matplotlib, seaborn, plotly
- Machine Learning: scikit-learn (DummyRegressor, LinearRegression, RandomForestRegressor)
- Dashboarding: Tableau / static images


## Data Preprocessing and Feature Engineering
- Performed an initial data audit to check shape, data types, duplicates and missing values.
- Standardized column names and converted relevant columns to numeric types.
- Encoded categorical variables: Applied one-hot / ordinal encoding to CPU model, brand, GPU, and other categorical fields to prepare data for modelling.
- Engineered features:
  - Converted price column to a common currency Price_euros and used as the target variable.
  - Cleaned and simplified text features (e.g., RAM, storage) into numeric representations (GB values, SSD/HDD flags).
  - Created derived columns (e.g. Total_storage_GB, Weight_kg converted from strings) to better capture numeric relationships
- Scaled the numerical features using StandardScaler and MinMaxScaler to normalize data ranges and improve model performance.
- Train/test split: used train_test_split with test_size=0.2 and random_state=42.


## Predictive Modeling
- Established a baseline using DummyRegressor (mean strategy) to set an easy-to-beat benchmark.
- Trained and evaluated the following models:
   - Linear Regression — quick baseline linear approach.
   - Random Forest Regressor — captured non-linearities and interactions between specs.
- Evaluated models using MAE, RMSE and R² on the holdout test set and compared to baseline.
- Extracted feature importances from the Random Forest model to identify top predictors of price (e.g., CPU family, RAM, storage type, GPU presence).
