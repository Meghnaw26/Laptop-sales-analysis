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

<img width="1088" height="790" alt="Image" src="https://github.com/user-attachments/assets/329b2d12-9f6e-41f0-a833-e23905f46907" />




<img width="1126" height="703" alt="Image" src="https://github.com/user-attachments/assets/db659e85-6fc7-4a88-9522-be3a24532ff1" />





## Exploratory Data Analysis 
<img width="839" height="549" alt="Image" src="https://github.com/user-attachments/assets/35f752af-f838-4a77-b16e-176d9331fdfa" />


<img width="920" height="533" alt="Image" src="https://github.com/user-attachments/assets/f928cfa0-a1be-4bc6-b22f-27d78d6fa4cc" />


<img width="1097" height="548" alt="Image" src="https://github.com/user-attachments/assets/f116fa21-a3ba-4aff-a487-31960ba900e3" />



<img width="1102" height="585" alt="Image" src="https://github.com/user-attachments/assets/a00053d0-ce95-44e2-b221-7f818e4b056f" />


<img width="1129" height="791" alt="Image" src="https://github.com/user-attachments/assets/9b363efb-8136-4b9c-868f-c9631ca1ccbf" />



<img width="1127" height="609" alt="Image" src="https://github.com/user-attachments/assets/241e5507-7d6c-4dae-804d-b8c653fe6095" />



<img width="748" height="569" alt="Image" src="https://github.com/user-attachments/assets/5c4d505b-cbf8-4c17-801c-dfc8b4dd3d54" />



<img width="765" height="566" alt="Image" src="https://github.com/user-attachments/assets/0ec60ac2-c078-4f36-a4aa-76b4b85ef2ba" />



<img width="1041" height="575" alt="Image" src="https://github.com/user-attachments/assets/8b730f16-ff2a-4e5d-bcf1-063e102929eb" />



<img width="1105" height="656" alt="Image" src="https://github.com/user-attachments/assets/9b261e5b-69b3-46d0-924b-08fb7d560341" />



<img width="1013" height="811" alt="Image" src="https://github.com/user-attachments/assets/86185f15-5d2c-4031-ad89-38a18815cd2b" />



<img width="1089" height="451" alt="Image" src="https://github.com/user-attachments/assets/4c9b41c2-24f4-4b15-82e8-6478a4e20fd2" />



<img width="1100" height="653" alt="Image" src="https://github.com/user-attachments/assets/8634e0bb-fbaf-4b79-9b00-eb7d58204fb2" />



<img width="1108" height="701" alt="Image" src="https://github.com/user-attachments/assets/5440df20-20dd-4b8f-903c-4764cd125c30" />

