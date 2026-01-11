# Predicting 30-Day Hospital Readmission Risk Using Machine Learning

## Project Overview
Unplanned hospital readmissions within 30 days of discharge are a significant challenge for healthcare systems worldwide. They are associated with increased healthcare costs, hospital congestion, and poorer patient outcomes. In the Philippine healthcare context—where public hospitals often operate under constrained resources—reducing avoidable readmissions is particularly important.

This capstone project applies an end-to-end machine learning lifecycle to predict the likelihood of 30-day hospital readmission using patient-level clinical and administrative data. The objective is to support targeted post-discharge interventions by identifying high-risk patients who may benefit from additional follow-up, education, or care coordination.

This project was completed as part of the **AI & Machine Learning (AIM) programme** and follows industry-aligned best practices in reproducibility, leakage prevention, interpretability, and responsible AI.

---

## Business Problem
Hospitals face increasing pressure to optimise bed utilisation while maintaining quality of care. High readmission rates may indicate gaps in discharge planning, medication adherence, or access to follow-up care.

From an operational and business perspective, accurately identifying patients at high risk of readmission can:
- Reduce avoidable healthcare costs
- Improve patient outcomes and continuity of care
- Support data-driven clinical and operational decision-making
- Improve hospital performance metrics and resource allocation

---

## Data Science Problem
The data science task is formulated as a supervised **binary classification problem**:

> **Can we predict whether a patient will be readmitted within 30 days of discharge based on available clinical, demographic, and healthcare utilisation data?**

Multiple machine learning models are trained and evaluated, with careful consideration of class imbalance, model explainability, and ethical implications.

---

## Repository Structure

├── notebooks/
│ ├── 01_problem_framing_data_understanding.ipynb
│ ├── 02_data_cleaning_feature_engineering.ipynb
│ ├── 03_eda_feature_selection_dimensionality_reduction.ipynb
│ ├── 04_model_development_evaluation_selection.ipynb
│ └── 05_model_explainability_fairness_interpretation.ipynb
│
├── data/
│ └── README.md
│
├── outputs/
│ └── processed/
│
├── models/
│
├── docs/
│
└── README.md

---

## Methodology & Notebook Breakdown

### Notebook 01 – Problem Framing & Data Understanding
- Business and clinical motivation
- Prediction objective and success metrics
- Dataset overview and data dictionary
- Initial assessment of missing values and feature types

### Notebook 02 – Data Cleaning & Feature Engineering
- Target engineering for 30-day readmission
- Leakage prevention and feature exclusion
- Missing value handling and encoding
- Leakage-safe stratified train/test split
- Reproducible preprocessing pipeline

### Notebook 03 – EDA, Feature Selection & Dimensionality Reduction
- Leakage-safe exploratory data analysis (training data only)
- Numeric and categorical feature diagnostics
- Correlation and redundancy analysis
- Filter-based and embedded feature selection
- PCA / TruncatedSVD diagnostics

### Notebook 04 – Model Development, Evaluation & Selection
- Baseline and candidate model implementation
- Cross-validated model comparison
- Clinically informed threshold optimisation
- Final model selection and artifact persistence

### Notebook 05 – Model Explainability & Fairness Analysis
- Model interpretability (coefficients, SHAP)
- Feature impact analysis
- Bias and fairness assessment across subgroups
- Responsible AI considerations and mitigations

---

## Evaluation Metrics
Model performance is evaluated using metrics appropriate for imbalanced healthcare data:
- ROC-AUC and PR-AUC
- Precision, Recall, and F1-score
- Confusion matrix analysis
- Threshold-based evaluation aligned with clinical priorities

Recall is prioritised due to the higher clinical and ethical cost associated with failing to identify high-risk patients.

---

## Reproducibility Notes
- Large binary artifacts (processed matrices, trained models) are not committed to GitHub.
- All results are fully reproducible by running the notebooks sequentially.
- Google Colab is used for execution, with artifacts stored in Google Drive.

---

## Ethical Considerations
Healthcare machine learning models must be interpretable, fair, and used responsibly. This project includes:
- Model explainability using feature importance and SHAP values
- Bias and fairness analysis across available demographic attributes
- Discussion of limitations, data imbalance, and deployment risks

The model is intended as a **decision-support tool** and does not replace clinical judgment.

---

## Author
**John Raffy Raymundo**  
AI & Machine Learning Student, AIM  
Capstone Project – 2025
