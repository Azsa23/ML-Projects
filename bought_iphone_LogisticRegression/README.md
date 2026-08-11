iPhone Purchase Prediction (Logistic Regression)
This project is a complete end-to-end Machine Learning pipeline that predicts whether a customer is likely to purchase an iPhone based on their demographic and financial data (Age, Salary, and Gender). It serves as a practical implementation of Logistic Regression for binary classification.

🚀 Project Pipeline
The implementation follows the standard machine learning workflow:

Data Preprocessing:

Handling categorical variables using LabelEncoder.

Feature scaling using StandardScaler to ensure optimal model performance.

Data Splitting: Training and testing the model with a 75/25 split.

Model Training: Implementing LogisticRegression with the 'liblinear' solver for robust classification.

Model Evaluation: Measuring performance using:

Confusion Matrix

Accuracy Score

Precision & Recall

Inference: Predicting purchase outcomes for new individual profiles and interpreting results using probability scores (predict_proba).

🛠 Tech Stack
Python

Pandas: Data loading and exploration.

Scikit-learn: Implementation of the classifier, preprocessing, and evaluation metrics.

📁 Repository Structure
bought_iphone_LogisticRegression.ipynb: The notebook containing the full code, evaluation metrics, and prediction examples.

iphone.csv: The dataset containing client information (Gender, Age, Salary, Purchase History).

📥 How to Run
Install the required dependencies:

Bash
pip install pandas scikit-learn
Clone the repository and open the Jupyter Notebook to explore the model's performance and prediction logic.

💡 Key Takeaway
This project demonstrates the importance of Feature Scaling and Data Encoding in building reliable classification models. It shows how probability-based models can provide deeper insights beyond a simple "Yes/No" output.
