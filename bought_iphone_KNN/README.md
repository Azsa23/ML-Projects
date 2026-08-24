# iPhone Purchase Prediction using K-Nearest Neighbors (KNN) 📱🤖

This repository contains a complete machine learning project built with Python to predict whether a customer will purchase an iPhone based on demographic features and salary using the **K-Nearest Neighbors (KNN)** classification algorithm.

---

## 📊 Dataset Overview
The dataset (`iphone11.csv`) contains **2,000 samples** with the following features:
* **Gender:** The gender of the customer (processed and encoded using `LabelEncoder`).
* **Age:** The age of the customer.
* **Salary:** The annual salary of the customer.
* **Purchase_Iphone:** The target variable (binary: `1` for bought, `0` for did not buy).

---

## 🛠️ Project Workflow & Steps

1. **Data Preprocessing:**
   * Loading the dataset using `pandas`.
   * Splitting features (`X`) and target (`y`).
   * Encoding categorical text data (`Gender`) into numerical values using `LabelEncoder`.

2. **Train-Test Split:**
   * Splitting the dataset into **80% training data** and **20% testing data** using `train_test_split`.

3. **Feature Scaling:**
   * Standardizing features (`Age` and `Salary`) using `StandardScaler` to ensure all columns contribute equally to the distance-based KNN algorithm.

4. **Model Training (KNN Classifier):**
   * Dynamically calculating the optimal $k$ value using the square root of the training set size (adjusted to the nearest odd number to avoid ties).
   * Training the `KNeighborsClassifier`.

5. **Evaluation Metrics:**
   * Evaluating the model performance using:
     * **Accuracy Score**
     * **Precision Score**
     * **Recall Score**
     * **Confusion Matrix**

6. **Inference & Probabilities:**
   * Making predictions on custom user profiles.
   * Calculating prediction probabilities (`predict_proba`) for deeper insights.

---

## 📈 Model Performance
* **Accuracy:** ~69%
* **Precision:** ~70.4%
* **Recall:** ~83.3%

---

## 🚀 Requirements & Libraries
Make sure you have the following Python libraries installed before running the notebook:

```bash
pip install pandas numpy scikit-learn
