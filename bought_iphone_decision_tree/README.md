# 📱 iPhone Purchase Prediction using Decision Tree

A Machine Learning project that predicts whether a customer will purchase an iPhone based on demographic and financial features (Gender, Age, Estimated Salary).

---

## 📌 Project Overview
The objective of this project is to build and evaluate a **Decision Tree Classifier** to classify user purchasing behavior. It covers the full machine learning workflow: exploratory data analysis, data preprocessing, feature scaling, model training, hyperparameter tuning, and performance evaluation.

---

## 📊 Dataset Description
The dataset contains **2,000 records** with the following features:
- **`gender`**: Gender of the customer (`Male` / `Female`).
- **`age`**: Age in years.
- **`salary`**: Estimated annual income.
- **`purchase_iphone`** *(Target)*: Binary label (`1` = Purchased, `0` = Did not purchase).

---

## ⚙️ Workflow & Preprocessing
1. **Data Preprocessing & Encoding:** Encoded categorical features (`gender`) using `LabelEncoder`.
2. **Data Splitting:** Divided the data into training (80%) and testing (20%) sets.
3. **Feature Scaling:** Applied `StandardScaler` on the feature set.
4. **Model Training:** Built a `DecisionTreeClassifier` utilizing the **Entropy** criterion.
5. **Hyperparameter Tuning:** Mitigated severe overfitting by tuning the tree depth (`max_depth`).

---

## 📈 Results & Performance Comparison

| Configuration | Hyperparameters | Test Accuracy | Observations |
| :--- | :--- | :--- | :--- |
| **Unconstrained Tree** | `max_depth=None` | **57.0%** | Severe Overfitting (100% training accuracy) |
| **Tuned Tree** | `max_depth=4` | **68.2%** | Generalized better on unseen test data |

---

## 🚀 Getting Started

### Prerequisites
Make sure you have Python installed with the required libraries:
```bash
pip install numpy pandas scikit-learn matplotlib
