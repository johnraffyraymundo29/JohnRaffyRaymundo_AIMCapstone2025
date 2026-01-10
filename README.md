
# Predicting 30-Day Hospital Readmission Risk Using Machine Learning

## Project Overview
Unplanned hospital readmissions within 30 days of discharge are a significant challenge for healthcare systems worldwide. They are associated with increased healthcare costs, hospital congestion, and poorer patient outcomes. In the Philippine healthcare context, where public hospitals often operate under constrained resources, reducing avoidable readmissions is particularly important.

This capstone project applies an end-to-end machine learning lifecycle to predict the likelihood of 30-day hospital readmission using patient-level clinical and administrative data. The objective is to support targeted post-discharge interventions by identifying high-risk patients who may benefit from additional follow-up, education, or care coordination.

This project is completed as part of the AI & Machine Learning (AIM) programme and follows industry-aligned best practices in data science, reproducibility, and ethical AI.

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

## Project Structure
The repository is organised following open-source and industry best practices:

```
.
├── data/                    # Raw and processed datasets
├── notebooks/               # Exploratory analysis and development
├── src/                     # Reusable Python modules
├── models/                  # Trained model artifacts
├── results/                 # Evaluation metrics and reports
├── README.md               # This file
├── requirements.txt        # Python dependencies
└── LICENSE                 # Project license
```

---

## Methodology
The project follows the complete machine learning lifecycle:

1. Problem understanding and business framing  
2. Data collection and data understanding  
3. Data preprocessing, exploratory data analysis (EDA), and feature engineering  
4. Model training, tuning, and evaluation  
5. Model explainability, bias analysis, and ethical considerations  
6. Results communication through technical and business-facing presentations  

---

## Evaluation Metrics
Model performance is evaluated using metrics appropriate for imbalanced healthcare data:
- Area Under the ROC Curve (AUC)
- Precision, Recall, and F1-score
- Confusion Matrix analysis

Recall is prioritised due to the higher clinical and ethical cost associated with failing to identify high-risk patients.

---

## Ethical Considerations
Healthcare machine learning models must be interpretable, fair, and used responsibly. This project includes:
- Model explainability using feature importance and SHAP values
- Bias analysis across available demographic attributes
- Discussion of limitations, data imbalance, and deployment risks

The model is intended as a **decision-support tool** and does not replace clinical judgment.

---

## Author
**John Raffy Raymundo**  
AI & Machine Learning Student, AIM  
Capstone Project – 2025
