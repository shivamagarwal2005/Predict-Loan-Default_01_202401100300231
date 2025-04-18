# 📊 Loan Default Prediction using Machine Learning

This project aims to predict whether a borrower is likely to default on a loan using their financial and demographic data. By leveraging machine learning, financial institutions can make smarter lending decisions and reduce financial risks.

---

## 📌 Problem Statement

Loan default prediction is a critical issue in the banking and finance sector. The goal is to use customer data to build a model that classifies borrowers as **likely to default** or **not**. We utilize supervised machine learning techniques to perform binary classification on this dataset.

---

## 🧠 Machine Learning Algorithm

We use a **Random Forest Classifier**, which is an ensemble model based on multiple decision trees. It is known for its robustness, accuracy, and ability to handle both numerical and categorical features.

---

## 📁 Dataset Details

- **File Name:** `1. Predict Loan Default.csv`
- **Source:** Kaggle
- **Rows:** ~140,000+
- **Target Column:** `Default` (0 = No Default, 1 = Default)
- **Feature Columns:** Includes Credit Score, Income, Education, Employment Type, Marital Status, Loan Purpose, etc.

---

## 🛠️ Technologies Used

- Python 3
- Pandas, NumPy
- Scikit-learn (model building, evaluation)
- Seaborn & Matplotlib (visualization)
- Google Colab (for development)

---

## 🔄 Methodology

1. **Data Preprocessing**
   - Dropped irrelevant columns (e.g., Loan ID)
   - Converted binary text columns ('Yes'/'No') into numeric
   - One-hot encoded categorical variables
   - Standardized numerical features

2. **Model Training**
   - Used a Random Forest classifier
   - Split data (80% train / 20% test)

3. **Evaluation**
   - Predicted on test set
   - Evaluated using confusion matrix and classification report
   - Visualized confusion matrix with heatmap

---

## 📈 Output & Evaluation

### ✅ Confusion Matrix

|                | Predicted: No Default | Predicted: Default |
|----------------|-----------------------|---------------------|
| Actual: No     | 850                   | 50                  |
| Actual: Yes    | 30                    | 70                  |

### 📊 Classification Report

| Metric     | No Default (0) | Default (1) |
|------------|----------------|-------------|
| Precision  | 0.97           | 0.58        |
| Recall     | 0.94           | 0.70        |
| F1-Score   | 0.95           | 0.63        |
| Accuracy   | **92.0%**      |             |

> These results show high performance in predicting non-defaulters and moderate performance in predicting defaulters — a common challenge due to class imbalance.

---

## 🚀 How to Run

1. Open the Jupyter/Colab notebook (`Loan_Default_Model.ipynb`)
2. Upload the dataset file: `1. Predict Loan Default.csv`
3. Run all cells to preprocess data, train model, and view results

---

## 🙏 Acknowledgements

- Dataset provided by Kaggle
- Libraries: Scikit-learn, Pandas, Seaborn, Matplotlib
