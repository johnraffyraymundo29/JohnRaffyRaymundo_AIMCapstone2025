# Generative AI Usage Documentation

This document describes how Generative AI tools (large language models) were used in this project to support productivity, clarity, and documentation quality. All modeling decisions, data handling, evaluations, and conclusions were human-led, with Generative AI serving strictly as a supporting assistant.

---

**1) Problem Framing & Research Design**

### How Generative AI Was Used
- Assisted in refining the business problem of hospital readmissions into a machine learning formulation.
- Supported selection and justification of evaluation metrics for an imbalanced healthcare classification task (e.g., prioritizing Recall due to clinical risk).

### Example Prompt
```text
“How should a hospital readmission prediction problem be framed as a machine learning task,
and which evaluation metrics are most appropriate from a clinical perspective?”

**Application in This Project**

- Confirmed binary classification framing.
- Reinforced prioritization of Recall due to the high cost of false negatives in clinical settings.
- Improved alignment between business objectives and technical success metrics.

**2. Exploratory Data Analysis (EDA) & Feature Engineering**
How Generative AI Was Used

- Suggested EDA techniques to analyze class imbalance, feature distributions, and correlations.
- Proposed domain-relevant feature engineering ideas based on healthcare context.
- Helped interpret exploratory findings to improve clarity in notebook explanations.

**Example Prompt**
What exploratory data analysis techniques help identify drivers of hospital readmissions
in structured healthcare data?

**Application in This Project**
- Guided visualization choices such as distributions and correlation analysis.
- Supported feature selection and redundancy reduction.
- Enhanced written interpretation of EDA results.

**3. Code Assistance & Optimization**
How Generative AI Was Used

- Assisted in drafting Python code templates for preprocessing pipelines, model evaluation, and metric comparison.
- Helped refactor repetitive code into reusable, cleaner functions.
- Supported validation of evaluation logic (e.g., confusion matrix interpretation, metric selection).

**Example Prompt**
Generate a Python function that evaluates a classification model using Recall, Precision,
F1-score, and ROC-AUC.

Example Output (Reviewed and Adapted)
def evaluate_model(y_true, y_pred, y_prob):
    return {
        "Recall": recall_score(y_true, y_pred),
        "Precision": precision_score(y_true, y_pred),
        "F1": f1_score(y_true, y_pred),
        "ROC_AUC": roc_auc_score(y_true, y_prob)
    }


All AI-generated code was reviewed, tested, and modified before use.

**4. Model Explainability, Ethical AI & Bias Analysis**
How Generative AI Was Used

- Supported explanations of model interpretability concepts such as feature importance and coefficient interpretation.
- Assisted in structuring discussions on bias, fairness, and ethical risks in healthcare ML.
- Helped propose mitigation strategies and governance practices.

**Example Prompt**
How should fairness risks and ethical limitations be communicated for a healthcare
machine learning model, and what mitigation strategies can be proposed?

Application in This Project
- Strengthened clarity of explainability and fairness sections.
- Improved articulation of limitations such as proxy variables and data representativeness.
- Supported development of responsible AI recommendations.

**5. Communication & Presentation**
How Generative AI Was Used

- Assisted in structuring technical and business presentations.
- Helped translate technical findings into non-technical, executive-friendly language.
- Supported creation of speaker notes for clearer communication.

**Example Prompt**
Rewrite this technical machine learning explanation so it is suitable for a
non-technical healthcare executive audience.

Human Oversight & Limitations

- Generative AI did not make final analytical or modeling decisions.
- All outputs were critically reviewed for correctness, domain relevance, and ethical considerations.
- The author retains full responsibility for the data, models, evaluations, and conclusions presented in this project.

**Summary**
Generative AI was used as a productivity- and clarity-enhancing tool to support ideation, code drafting, explanation refinement, and communication quality. The project remains human-directed, ethically evaluated, and technically validated, aligning with responsible AI principles.