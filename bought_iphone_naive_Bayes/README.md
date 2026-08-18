# iPhone 11 Purchase Prediction using Naive Bayes

This project is a Machine Learning classification model designed to predict whether a customer will purchase an **iPhone 11** based on personal features such as gender, age, and annual salary.

---

## 🚀 Project Pipeline
The project goes through a complete data science pipeline, including:
1. **Data Loading & Exploration:** Importing and examining the dataset using `Pandas`.
2. **Data Preprocessing:** Encoding categorical text data (Gender) into numerical values using `LabelEncoder`.
3. **Data Splitting:** Splitting the dataset into training and testing sets (80/20 ratio).
4. **Feature Scaling:** Normalizing features using `StandardScaler` to ensure optimal model performance.
5. **Model Training:** Training the classification model using the **Gaussian Naive Bayes** algorithm.
6. **Comprehensive Model Evaluation:** 
   - Calculating Model Accuracy (`Accuracy`)
   - Calculating Positive Precision (`Precision`)
   - Calculating Recall (`Recall`)
   - Generating a Confusion Matrix
7. **Prediction & Probability Scoring:** Testing the model with custom user profiles and predicting purchase probabilities using `predict_proba`.

---

## 🛠️ Tech Stack
* **Python**
* **Pandas** (for data analysis and manipulation)
* **Scikit-Learn** (for machine learning models and preprocessing)

---

## 📂 File Structure
```text
├── bought_iphone_naive_Bayes.ipynb   # Jupyter Notebook containing the complete code
├── iphone11.csv                      # Dataset used for training and testing
└── README.md                         # Project documentation
