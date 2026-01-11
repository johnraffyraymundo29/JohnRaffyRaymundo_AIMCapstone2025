**Predicting 30-Day Hospital Readmission Risk Using Machine Learning**
**Project Overview**

Unplanned hospital readmissions within 30 days of discharge are a significant
challenge for healthcare systems worldwide. They are associated with increased
healthcare costs, hospital congestion, and poorer patient outcomes. In the
Philippine healthcare context, where public hospitals often operate under
constrained resources, reducing avoidable readmissions is particularly important.

This capstone project applies an end-to-end machine learning lifecycle to predict
the likelihood of 30-day hospital readmission using patient-level clinical and
administrative data. The objective is to support targeted post-discharge
interventions by identifying high-risk patients who may benefit from additional
follow-up, education, or care coordination.

This project was completed as part of the AI & Machine Learning (AIM) Programme
and follows industry-aligned best practices in data science, reproducibility, and
ethical AI.

---

**Business Problem**

Hospitals face increasing pressure to optimise bed utilisation while maintaining
quality of care. High readmission rates may indicate gaps in discharge planning,
medication adherence, or access to follow-up care.

From an operational and business perspective, accurately identifying patients at
high risk of readmission can:

- Reduce avoidable healthcare costs
- Improve patient outcomes and continuity of care
- Support data-driven clinical and operational decision-making
- Improve hospital performance metrics and resource allocation

---

**Data Science Problem**

The data science task is formulated as a supervised binary classification
problem:

**Can we predict whether a patient will be readmitted within 30 days of
discharge based on available clinical, demographic, and healthcare utilisation
data?**

Multiple machine learning models are trained and evaluated, with careful
consideration of class imbalance, model explainability, and ethical implications.
---
**Project Structure Structure**
The repository is organised following open-source and industry best practices:
├.
├── data/                      # Raw reference data and documentation
├── notebooks/                 # Step-by-step analysis notebooks (01–05)
├── src/                       # Reusable Python utilities
├── models/                    # Trained model artifacts
├── outputs/                   # Processed datasets and saved features
├── docs/                      # Explainability and fairness outputs
├── README.md                  # Project overview (this file)
├── requirements.txt           # Python dependencies
└── LICENSE


**Methodology & Notebook Guide**

The project follows the complete machine learning lifecycle:

1. Problem Framing & Data Understanding
Notebook 01 – Business context, prediction objective, dataset overview, and
data dictionary

2. Data Cleaning & Feature Engineering
Notebook 02 – Target engineering, leakage prevention, preprocessing pipeline,
and train/test split

3. Exploratory Analysis & Feature Diagnostics
Notebook 03 – Applied EDA, feature relevance screening, correlation analysis,
and dimensionality reduction

4. Model Development & Evaluation
Notebook 04 – Baseline and advanced models, performance comparison, threshold
selection, and final model selection

5. Explainability, Fairness & Ethical Analysis
Notebook 05 – Global and local explainability, fairness assessment by subgroup,
ethical risks, and mitigation strategies

**Evaluation Metrics**

Model performance is evaluated using metrics appropriate for imbalanced healthcare
data:

- Area Under the ROC Curve (AUC)
- Precision, Recall, and F1-score
- Confusion matrix analysis

Recall is prioritised due to the higher clinical and ethical cost associated with
failing to identify high-risk patients.

**Ethical Considerations**

Healthcare machine learning models must be interpretable, fair, and used
responsibly. This project explicitly addresses:

Model explainability using global and local interpretation methods

Fairness assessment across clinically meaningful subgroups

Discussion of limitations, bias risks, and ethical deployment considerations

The model is intended as a decision-support tool and does not replace clinical
judgment.

**Reproducibility Notes**

All analysis is conducted using leakage-safe train/test splits.
Each notebook can be run independently, provided required artifacts from previous
steps are available. When using Google Colab, Google Drive must be mounted to
access saved datasets and models.

**Author**

John Raffy Raymundo
AI & Machine Learning Student, AIM
Capstone Project – 2025