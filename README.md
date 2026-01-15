# Predicting 30-Day Hospital Readmissions Using Machine Learning

**Author:** John Raffy Raymundo  
**Program:** AI & Machine Learning Capstone  
**Year:** 2025

---

## Project Overview
Hospital readmissions within 30 days of discharge are costly, disruptive, and often preventable.  
This project develops an interpretable and ethically evaluated machine learning model to predict the risk of 30-day hospital readmission at the point of discharge. The goal is to support proactive clinical interventions, improve patient outcomes, and reduce avoidable healthcare costs.

The solution follows the full machine learning lifecycle, from problem framing and data understanding to model development, explainability, fairness assessment, and responsible deployment considerations.

---

## Business Problem
Unplanned hospital readmissions increase operational costs, trigger payer penalties, and negatively impact patient outcomes and satisfaction. Many readmissions could be reduced through targeted post-discharge interventions if high-risk patients were identified earlier.

This project addresses the problem by building a predictive model that:
- Identifies patients at high risk of readmission before discharge  
- Supports clinical decision-making (not replacement)  
- Enables more efficient allocation of care resources  

---

## Dataset
The dataset consists of structured healthcare data available at or before patient discharge. It includes multiple feature categories such as:
- Patient demographics  
- Prior healthcare utilization  
- Clinical conditions and comorbidities  

The target variable indicates whether a patient is readmitted within 30 days of discharge.  
Strict care was taken to prevent data leakage by excluding any post-discharge information from model inputs.

---

## Methodology & Notebook Guide
This project follows the complete machine learning lifecycle and is organized into five structured and reproducible notebooks:

### 1. Problem Framing & Data Understanding  
**Notebook 01**  
Defines the business context and prediction objective, provides a dataset overview, and documents feature categories and the data dictionary.

### 2. Data Cleaning & Feature Engineering  
**Notebook 02**  
Covers target construction, leakage prevention strategies, preprocessing pipelines, and leakage-safe train/test splitting.

### 3. Exploratory Analysis & Feature Diagnostics  
**Notebook 03**  
Includes applied exploratory data analysis (EDA), feature relevance screening, correlation analysis, and dimensionality reduction techniques to diagnose feature quality and redundancy.

### 4. Model Development & Evaluation  
**Notebook 04**  
Implements baseline and advanced machine learning models, compares performance across multiple metrics, performs threshold tuning, and selects the final model based on both technical and clinical considerations.

### 5. Explainability, Fairness & Ethical Analysis  
**Notebook 05**  
Applies global and local explainability techniques, conducts fairness assessments across clinically meaningful subgroups, and discusses ethical risks, limitations, and mitigation strategies.

---

## Model Development & Evaluation
Multiple classification models were implemented and evaluated to balance predictive performance and interpretability, including baseline and more advanced approaches.

### Evaluation Metrics
Given the imbalanced nature of healthcare readmission data, model performance was evaluated using:
- Area Under the ROC Curve (ROC-AUC)  
- Precision, Recall, and F1-score  
- Confusion matrix analysis  

**Recall is prioritised** due to the higher clinical and ethical cost associated with failing to identify high-risk patients who may benefit from early intervention.

---

## Explainability, Fairness & Ethical AI
Healthcare machine learning systems must be interpretable, fair, and responsibly deployed. This project explicitly addresses:

- Model explainability using both global and local interpretation methods  
- Fairness assessment across clinically meaningful demographic subgroups  
- Discussion of model limitations, bias risks, and ethical deployment considerations  

The model is designed strictly as a **decision-support tool** and does **not replace clinical judgment**.

---

## Use of Generative AI
Generative AI tools (large language models) were used as assistive support for problem framing, exploratory analysis planning, code drafting and refactoring, explainability and fairness write-ups, and presentation preparation. All analytical decisions and outputs were reviewed and validated by the author.

👉 Full documentation, including examples and prompts:  
**[docs/generative_ai_usage.md](docs/generative_ai_usage.md)**

---

## Demo Video
A short demo video provides a walkthrough of the business problem, data pipeline, modeling approach, explainability and fairness analysis, and overall project impact.

Link: https://drive.google.com/file/d/1OFOPJRJNNeOeVOXLCyivei1xU47bvtJD/view

---

### Repository Structure / How to Run

```
├── notebooks/
│   ├── 01_problem_framing_data_understanding.ipynb
│   ├── 02_data_cleaning_feature_engineering.ipynb
│   ├── 03_eda_feature_selection_dimensionality_reduction.ipynb
│   ├── 04_model_development_evaluation_selection.ipynb
│   └── 05_explainability_fairness_analysis.ipynb
├── data/
│   └── (raw and/or processed datasets, subject to availability)
├── models/
│   └── (saved model artifacts)
├── outputs/
│   └── (figures, evaluation outputs, and reports)
├── docs/
│   └── generative_ai_usage.md
├── requirements.txt
└── README.md
```

### How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebooks sequentially from `01` to `05`.

---

## Reproducibility Notes
- All analysis is conducted using leakage-safe train/test splits.  
- Each notebook can be run independently, provided required artifacts from earlier steps are available.  
- When using Google Colab, Google Drive must be mounted to access saved datasets and trained models.

---

## References
- Relevant academic literature on hospital readmissions  
- Ethical AI and fairness references  
- Dataset documentation and sources  
