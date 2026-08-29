# iPhone Purchase Prediction (SVM)

A machine learning project using a **Support Vector Classifier (SVC)** with a linear kernel to predict whether a customer will purchase an iPhone based on **Gender**, **Age**, and **Salary**[cite: 1, 2].

---

### 📊 Dataset & Preprocessing
* **Features**: Gender (`LabelEncoder`), Age, Salary[cite: 1, 2].
* **Target**: `purchase_iphone` (0 or 1)[cite: 1, 2].
* **Split**: 80% Train, 20% Test (`random_state=0`)[cite: 1, 2].
* **Scaling**: `StandardScaler` applied to feature inputs[cite: 1, 2].

---

### 📈 Results
* **Accuracy**: 68.75%[cite: 1, 2]
* **Precision**: 70.61%[cite: 1, 2]
* **Recall**: 82.08%[cite: 1, 2]

---

### 🚀 Quick Start
```bash
pip install pandas scikit-learn
jupyter notebook bought_iphone_svm.ipynb
