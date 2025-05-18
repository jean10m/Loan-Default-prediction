# 💳 Loan Default Prediction – Logistic Regression vs Decision Tree

This machine learning project predicts whether a borrower will default on a loan using credit and demographic data. It compares **Logistic Regression** and a **Decision Tree Classifier** to evaluate how well each model balances between **recall** (identifying defaulters) and **precision** (avoiding false positives).

---

## 📊 Dataset

- 32,000+ records with borrower features:
  - Age, income, credit score, job type, loan amount, tenure, etc.
- Target: `Default` (0 = No, 1 = Yes)

---

## 🧠 Models Compared

1. **Logistic Regression**
   - Includes class weighting and feature scaling
   - More interpretable and suitable for probability-based credit scoring

2. **Decision Tree**
   - Limited max depth for simplicity
   - Better at capturing nonlinear patterns

---

## ✅ Results Summary (Why It Matters for Banks)

| Model              | Precision | Recall (Defaults) | Accuracy |
|-------------------|-----------|-------------------|----------|
| Logistic Regression | 95%       | **78%**           | 89%      |
| Decision Tree      | **97%**   | 58%               | 90%      |

- **Logistic Regression** is more effective at catching potential defaulters, making it valuable for banks aiming to **minimize loan loss** and improve **risk classification**.
- **Decision Tree** is better at avoiding false positives, which helps prevent **unnecessary credit rejections** — key for **customer retention and lending revenue**.

> Banks face a critical trade-off:
> - **Catch more risky borrowers** (maximize recall)
> - **Avoid false alarms** and retain good customers (maximize precision)

This model comparison supports credit teams in balancing risk exposure, profitability, and customer satisfaction — especially in light of **Basel III compliance** and **automated loan approvals**.

---

## 📌 Workflow Summary

- Data preprocessing (handling missing values, encoding)
- Feature scaling and class weighting
- Model training using scikit-learn
- Evaluation with:
  - Confusion matrices
  - Accuracy, Precision, Recall, F1-score
  - ROC Curve

---

## 📈 Tools

- Python (3.9)
- pandas, numpy, scikit-learn, matplotlib, seaborn

---

## 🚀 Next Steps

- Apply SMOTE to better address class imbalance
- Experiment with ensemble methods like Random Forest and XGBoost
- Integrate model into a Streamlit app or Power BI dashboard

