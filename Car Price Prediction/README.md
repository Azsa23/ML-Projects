# Car Price Prediction using Multiple Linear Regression

Welcome to this Machine Learning project! This project focuses on predicting used car prices based on multiple features using real-world data.

## 📌 Project Overview
The objective of this project is to build a Multiple Linear Regression model to estimate the price of a car (`Price`) by analyzing various numerical and categorical attributes such as manufacturing year, mileage, engine volume, brand, and body type.

---

## 🛠️ Technologies & Libraries Used
* **Python 3.x**
* **Pandas & NumPy** (Data manipulation, missing value imputation, and numerical operations)
* **Scikit-Learn** (Label Encoding, data splitting, linear regression model, and performance metrics)
* **Matplotlib & Seaborn** (Data visualization and Pearson correlation heatmap)

---

## 📊 Workflow & Steps
1. **Data Loading & Exploration:** Inspecting the dataset and identifying categorical and missing values.
2. **Data Preprocessing & Encoding:** 
   * Converting categorical text columns (`Brand`, `Body`, `Engine Type`, `Registration`, `Model`) into numerical values using `LabelEncoder`.
   * Handling missing/null values in `Price` and `EngineV` by filling them with column means.
3. **Correlation Analysis:** Generating a Pearson correlation matrix heatmap to understand feature relationships.
4. **Data Splitting:** Splitting the dataset into training and testing sets (80/20 split).
5. **Model Training:** Training a `LinearRegression` model using selected features (`Year`, `Mileage`, `Brand_num`, `Body_num`).
6. **Model Evaluation:** Evaluating prediction performance using:
   * **MAE** (Mean Absolute Error)
   * **MSE** (Mean Squared Error)
   * **RMSE** (Root Mean Squared Error)
7. **Real-World Prediction:** Testing the trained model by predicting the price of a custom-specified car profile.

---

## 🚀 Key Takeaway
This project demonstrates end-to-end data preprocessing pipelines—from handling raw text and missing data to training a multi-variable regression model and generating real-world business insights.
