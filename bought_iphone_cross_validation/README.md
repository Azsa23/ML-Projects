# 📱 iPhone Purchase Prediction: Multi-Model Benchmark

An end-to-end Machine Learning benchmark comparing five classification algorithms using **K-Fold Stratified/Cross-Validation** to predict iPhone purchase behavior based on demographic and financial data.

---

## 📌 Project Overview
The objective of this project is to evaluate and compare different supervised machine learning models to determine customer purchase intention. Instead of relying on a single random train/test split, this project implements a reusable evaluation function powered by **K-Fold Cross-Validation ($k=10$)** to avoid sampling bias and achieve robust performance estimates.

---

## 📊 Dataset Features
The dataset contains customer information with the following features:
* **`gender`**: Categorical (Encoded to numeric values using `LabelEncoder`).
* **`age`**: Customer's age.
* **`salary`**: Annual estimated salary.
* **`purchase_iphone`**: Binary target variable (`1` = Purchased, `0` = Not Purchased).

---

## ⚙️ Methodology & Pipeline

1. **Preprocessing & Encoding**:
   * Label Encoding applied to categorical variables (`gender`).
   * Feature scaling using `StandardScaler` to normalize distributions across varying numerical scales (`age`, `salary`).
2. **Model Evaluation Function**:
   * Implemented a modular benchmarking utility `cv_comparison_classification()` that automates multi-model cross-validation across specified fold counts and returns comparative performance tables.
3. **Algorithms Benchmarked**:
   * **Logistic Regression**
   * **Gaussian Naive Bayes**
   * **Support Vector Classifier (SVC - RBF Kernel)**
   * **K-Nearest Neighbors (KNN)**
   * **Decision Tree Classifier (Entropy Criterion)**

---

## 📈 Benchmark Results (10-Fold Cross-Validation)

| Model | Accuracy (Mean) |
| :--- | :---: |
| **Logistic Regression** | **0.668** |
| **Gaussian Naive Bayes** | **0.667** |
| **Support Vector Classifier (SVC)** | **0.663** |
| **K-Nearest Neighbors (KNN)** | **0.632** |
| **Decision Tree Classifier** | **0.587** |

### 🔍 Key Insights:
* Linear and probabilistic models (**Logistic Regression** and **GaussianNB**) performed best on this dataset, indicating largely linear separation trends between features like age/income and purchase decisions.
* Tree-based models (single Decision Tree) suffered from lower generalization accuracy ($58.7\%$), likely due to sensitivity to feature variance without ensemble methods (such as Random Forests).

---
