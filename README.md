# **Car Price Prediction**

## **Project Goal**
**Predict the selling price of cars** based on features like **Present Price, Car Age, Fuel Type, Seller Type, and Transmission**.

## **Tools Used**
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-Learn**

## **Steps**

### **1. Data Loading & Cleaning**
- Loaded dataset from CSV
- Checked **missing values**
- Created **`Car_Age`** feature
- Dropped irrelevant columns: **`Car_Name`, `Year`**

### **2. Feature Engineering**
- Created **Car Age = 2026 - Year**
- Encoded categorical variables (**Fuel_Type, Seller_Type, Transmission**) using **OneHotEncoder**

### **3. Exploratory Data Analysis (EDA)**
- **Histogram** of Selling Price
- **Scatterplot:** Present Price vs Selling Price
- **Correlation Heatmap**

### **4. Modeling**
- **Linear Regression**
- **Polynomial Regression (degree=2)**
- **Decision Tree Regression**
- **Random Forest Regression**

### **5. Evaluation**

#### **Model Performance**

| **Model**              | **R2 Score** | **RMSE** | **MAE** |
|------------------------|--------------|----------|---------|
| Linear Regression      | 0.850        | 1.658    | 1.245   |
| Polynomial Regression  | 0.955        | 0.905    | 0.566   |
| Decision Tree          | 0.929        | 1.143    | 0.624   |
| Random Forest          | 0.962        | 0.841    | 0.489   |

#### **Random Forest Cross-Validation**
- **CV Scores:** [0.960, 0.906, 0.895, 0.901, 0.948]  
- **Mean R2:** 0.922 ± 0.027

### **6. Visualization**
- **Histogram of Selling Price**
- **Scatterplot:** Present Price vs Selling Price
- **Correlation Heatmap**
- **Actual vs Predicted Prices** for all models
- **Feature Importance** (Random Forest)

## **How to Run**
1. Clone the repository
2. Ensure **`car data.csv`** is in the same folder as the notebook
3. Open **`Car_Price_Prediction.ipynb`** in Jupyter Notebook
4. Run all cells to reproduce the analysis and results

## **Notes**
- **Polynomial Regression (degree=2)** gives higher **R2** than Linear Regression
- **Random Forest** performs the best overall with the lowest **RMSE** and **MAE**
- **CV Scores** show Random Forest is stable across folds
