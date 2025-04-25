# Retail Credit Scoring Model – Predicting Loan Defaults

## Project Overview
This project simulates the development of a consumer credit risk scoring system, closely mirroring the modeling practices of banks, credit unions, and fintech lenders.  
The model predicts the Probability of Default (PD) of retail loan applicants and segments them into actionable risk bands.

---

## Methodology
- **Data Source**:  
  [Kaggle: Give Me Some Credit Dataset](https://www.kaggle.com/datasets/brycecf/give-me-some-credit-dataset)

- **Data Preprocessing**:
  - Imputed missing values
  - Handled outliers
  - Created raw and scaled datasets

- **Exploratory Data Analysis (EDA)**:
  - Identified correlations between financial behaviors and defaults
  - Addressed class imbalance (~8% defaults)

- **Feature Engineering**:
  - Debt-to-Income Ratio (DTI)
  - Late payment flags
  - Credit activity scores
  - Age and income bands
  - Log-transformed monthly income

- **Modeling**:
  - Trained Logistic Regression and Random Forest classifiers
  - Evaluated using AUC-ROC, Confusion Matrix, Precision, Recall

- **Probability Segmentation**:
  - Grouped applicants into Risk Bands A–E based on PD

---

## Key Results

| Risk Band | Default Rate (%) |
|-----------|------------------|
| A         | ~2%               |
| E         | 50%+              |

- Models displayed strong discriminatory power (AUC well above baseline).
- Clear monotonicity observed between PD and actual default rates.

---

## Business Interpretation

| Risk Band | Recommended Action           |
|-----------|-------------------------------|
| A, B      | Auto-approval                  |
| C         | Manual review                  |
| D         | High APR or secured product    |
| E         | Decline application            |

---

## Deliverables
- **Credit Scoring Report (PDF)**:  
  Detailed methodology, visuals, and business segmentation strategy.

- **(Optional)**: Jupyter Notebook containing preprocessing, EDA, modeling, and evaluation.

---

> This final report and credit scoring system were built with support from ChatGPT (OpenAI), used as a co-pilot for idea structuring, Python logic validation, and formatting refinement. The project reflects my own analytical judgment, assumptions, and execution, but benefited from AI-based structuring and iterative feedback throughout.




