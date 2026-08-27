# Fruit Classification using Support Vector Machine (SVM) 🍎🍊

A simple yet effective machine learning project that uses a **Support Vector Classifier (SVC)** to classify fruits (Apples vs. Oranges) based on their physical features such as **Weight** and **Size**.

---

## 📊 Dataset Features
- **Weight:** The weight of the fruit.
- **Size:** The size/dimensions of the fruit.
- **Class:** The target label (`apple` or `orange`).

---

## 🛠️ Tech Stack & Libraries
- **Python** 
- **Pandas** (Data manipulation and reading datasets)
- **Matplotlib** (Data visualization and plotting decision boundaries)
- **Scikit-Learn** (`SVC`, `LabelEncoder`, `train_test_split`, and performance metrics like accuracy, precision, recall, f1-score, and confusion matrix)

---

## ⚙️ Project Workflow
1. **Data Loading:** Read the dataset (`apples_and_oranges.csv`) using Pandas.
2. **Exploratory Data Analysis (EDA):** Visualize the data points using scatter plots to check for linear separability between classes.
3. **Data Preprocessing:** Encode categorical target labels (`Class`) into numerical values using `LabelEncoder`.
4. **Data Splitting:** Divide the dataset into training and testing sets (80/20 split).
5. **Model Training:** Train a Support Vector Classifier (`SVC`) model on the training data.
6. **Evaluation:** Assess model performance using Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix.
7. **Prediction:** Test the trained model with custom physical measurements to predict the fruit type.

---

