#  Medical Insurance Fraud Detection using Machine Learning

This project tackles the problem of detecting fraudulent medical insurance claims using machine learning. It applies data preprocessing, exploratory data analysis, and supervised learning to classify insurance claims as fraudulent or legitimate.

---

## Objective

Medical claim fraud is a serious issue with high financial impact. This project explores how machine learning can help identify suspicious claims using structured tabular data.

---

## Dataset

- Sourced from: [Kaggle – Medical Insurance Fraud Detection](https://www.kaggle.com/datasets/rohitrox/medical-insurance-fraud-detection)
- Each row represents a healthcare claim with features including:
  - Patient demographics
  - Provider IDs
  - Number of procedures/diagnoses
  - Admission types
  - Claim amounts
  - Fraud label (`0` = genuine, `1` = fraud)

---

## Data Preprocessing

- **Missing Values**: Handled missing values in categorical and numerical columns.
- **Encoding**: Label encoding for categorical variables (e.g., Hospital ID, Procedure codes).
- **Feature Engineering**: Aggregated counts and grouped statistics for physician and provider IDs.
- **Class Imbalance**: The dataset was imbalanced (~90% non-fraud); addressed using `class_weight` and stratified splitting.

---

## 📊 Exploratory Data Analysis (EDA)

- Fraudulent claims were more likely to come from:
  - Certain **provider IDs**
  - **Admit type** values like Emergency
- **Autoencoders or anomaly detection** could be explored in future work for rare-event modeling.

---

## Models Used

| Model              | Accuracy | Precision | Recall | F1-score | ROC AUC |
|-------------------|----------|-----------|--------|----------|---------|
| Logistic Regression | 0.91     | 0.79      | 0.71   | 0.74     | 0.90    |
| Random Forest       | 0.94     | 0.87      | 0.80   | 0.83     | 0.93    |
| XGBoost             | 0.95     | 0.89      | 0.82   | 0.85     | 0.95    |

>  XGBoost performed best overall, especially in terms of **AUC-ROC** and **balanced precision/recall**, making it suitable for fraud detection.

---

## Evaluation

- **ROC Curve** was plotted to visualize model separability
- **Confusion Matrix** highlighted true vs. false positives
- Used **F1-score** as the key metric due to class imbalance

---

## Key Insights

- **Provider-related features** and **claim patterns** strongly influenced fraud likelihood
- **XGBoost** outperformed baseline models by a noticeable margin
- Potential for deeper modeling with anomaly detection or autoencoders in future iterations

---

## 🛠Tools Used

- Python (Pandas, NumPy, Scikit-learn)
- XGBoost, Random Forest
- Matplotlib, Seaborn for visualization


