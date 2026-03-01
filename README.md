🚗 Car Price Prediction
Project Goal

Predict the selling price of used cars based on features like:

Present Price

Car Age

Kms Driven

Fuel Type

Seller Type

Transmission

Owner

The project uses machine learning regression models to provide accurate price predictions and insights into the most important features affecting car resale value.

Tools & Libraries

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-Learn

Project Workflow
1️⃣ Data Loading & Cleaning

Load dataset from CSV file

Checked for missing values

Created new feature: Car_Age = 2026 - Year

Dropped irrelevant columns: Car_Name and Year

Filled missing values:

Numerical columns → median

Categorical columns → mode

2️⃣ Feature Engineering

Encoded categorical variables (Fuel_Type, Seller_Type, Transmission) using OneHotEncoder

Combined with numerical features using ColumnTransformer

3️⃣ Exploratory Data Analysis (EDA)

Histogram of Selling Price

Scatterplot: Present Price vs Selling Price

Correlation Heatmap

4️⃣ Modeling

Linear Regression

Polynomial Regression (degree=2)

Decision Tree Regression

Random Forest Regression

5️⃣ Model Evaluation

R² Score, RMSE, MAE

Cross-validation for Random Forest

Hyperparameter tuning with GridSearchCV

Model Performance
Model	R2 Score	RMSE	MAE
Linear Regression	0.850	1.658	1.245
Polynomial Regression	0.955	0.905	0.566
Decision Tree	0.929	1.143	0.624
Random Forest	0.962	0.841	0.489
🔎 Feature Importance (Random Forest)

Top 3 Features:

Present Price – strongest predictor

Car Age – older cars sell for less

Kms Driven – smaller effect

📈 Visualizations

Histogram of Selling Price

Scatterplot: Present Price vs Selling Price

Correlation Heatmap

Actual vs Predicted Prices (Random Forest)

Feature Importance Bar Chart
