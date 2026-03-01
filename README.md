# 🚗 Car Price Prediction

Predict the **selling price of used cars** using machine learning regression models, based on features like Present Price, Car Age, Kms Driven, Fuel Type, Seller Type, Transmission, and Owner.

---

## 🎯 Project Goal
- Build predictive models to estimate **used car selling prices**.  
- Extract **insights about feature importance** affecting car resale value.  
- Showcase a complete **data science workflow** from cleaning to modeling.

---

## 🛠 Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-Learn  

---

## 📌 Workflow

### 1️⃣ Data Loading & Cleaning
- Load dataset from CSV  
- Check for missing values  
- Created `Car_Age = 2026 - Year`  
- Dropped irrelevant columns: `Car_Name`, `Year`  
- Filled missing values:
  - Numerical → median  
  - Categorical → mode  

### 2️⃣ Feature Engineering
- Encoded categorical variables (`Fuel_Type`, `Seller_Type`, `Transmission`) using **OneHotEncoder**  
- Combined encoded features with numerical features using **ColumnTransformer**  

### 3️⃣ Exploratory Data Analysis (EDA)
- Histogram of Selling Price  
- Scatterplot: Present Price vs Selling Price  
- Correlation Heatmap  

### 4️⃣ Modeling
- Linear Regression  
- Polynomial Regression (degree=2)  
- Decision Tree Regression  
- Random Forest Regression  

### 5️⃣ Model Evaluation
Metrics used:
- R² Score  
- RMSE  
- MAE  

#### Model Performance

| Model | R2 Score | RMSE | MAE |
|-------|----------|------|-----|
| Linear Regression | 0.850 | 1.658 | 1.245 |
| Polynomial Regression | 0.955 | 0.905 | 0.566 |
| Decision Tree | 0.929 | 1.143 | 0.624 |
| **Random Forest** | **0.962** | **0.841** | **0.489** |

#### Random Forest Cross-Validation
- CV Scores: `[0.960, 0.906, 0.895, 0.901, 0.948]`  
- Mean R² = 0.922 ± 0.027  

---

## 🔎 Feature Importance (Random Forest)
Top 3 Features:
1. **Present Price** – strongest predictor  
2. **Car Age** – older cars sell for less  
3. **Kms Driven** – smaller effect  

---

## 📈 Visualizations
- Histogram of Selling Price  
- Scatterplot: Present Price vs Selling Price  
- Correlation Heatmap  
- Actual vs Predicted Prices (Random Forest)  
- Feature Importance Bar Chart  

---

## 🚀 How to Run
1. Clone the repository  
2. Place `car data.csv` in the project folder  
3. Open `Car_Price_Prediction.ipynb` in Jupyter Notebook  
4. Run all cells to reproduce analysis and results  

---

## ✅ Conclusion
- Random Forest achieved the **best performance** with highest R² and lowest RMSE/MAE  
- Polynomial Regression captured non-linear relationships better than Linear Regression  
- Present Price and Car Age are the **most important features**  
- Full workflow demonstrates **data cleaning, feature engineering, modeling, evaluation, and insights extraction**  
- Ideal project for a **Data Science portfolio**

---

## 📄 License
Open source for educational purposes.
