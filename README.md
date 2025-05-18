# Loan Default Prediction

This project analyzes loan default data using logistic regression and decision tree models to predict the likelihood of default. The goal is to identify key factors influencing loan defaults and compare model performances.

## Dataset

- **Source**: [Kaggle Loan Default Dataset](https://www.kaggle.com/)
- **Features**: Age, income, credit score, loan amount, etc.
- **Target**: Loan default status (0 = No, 1 = Yes)

## Models Used

1. **Logistic Regression**
   - Applied class weighting and feature scaling.
   - Suitable for probability-based credit scoring.

2. **Decision Tree**
   - Limited depth for simplicity.
   - Captures nonlinear patterns.

## Results Summary

| Model              | Precision | Recall | Accuracy |
|-------------------|-----------|--------|----------|
| Logistic Regression | 95%       | 78%    | 89%      |
| Decision Tree      | 97%       | 58%    | 90%      |

- Logistic Regression is more effective at identifying potential defaulters.
- Decision Tree is better at avoiding false positives.

## Workflow Summary

- Data preprocessing (handling missing values, encoding).
- Feature scaling and class weighting.
- Model training using scikit-learn.
- Evaluation with confusion matrices, accuracy, precision, recall, F1-score, and ROC Curve.

## Tools

- Python (3.9)
- pandas, numpy, scikit-learn, matplotlib, seaborn

## Next Steps

- Apply SMOTE to address class imbalance.
- Experiment with ensemble methods like Random Forest and XGBoost.
- Integrate model into a Streamlit app or Power BI dashboard.

## Repository Structure

- `Loan_Default_Prediction.ipynb`: Main analysis notebook.
- `README.md`: Project overview and instructions.
- `requirements.txt`: List of required Python packages.

## How to Run

1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
