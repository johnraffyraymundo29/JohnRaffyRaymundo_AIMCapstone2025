# Dataset Information

## Dataset Used
This project uses the **Diabetes 130-US Hospitals for Years 1999–2008** dataset from the UCI Machine Learning Repository.

The dataset contains over 100,000 hospital encounters for patients diagnosed with diabetes and includes demographic information, admission details, clinical variables, and healthcare utilisation metrics. Each row represents a single hospital encounter.

---

## Data Source
- **Source:** UCI Machine Learning Repository  
- **Dataset name:** Diabetes 130-US Hospitals for Years 1999–2008  
- **Time period:** 1999–2008  

The dataset is widely used in academic research and has been referenced in numerous peer-reviewed studies related to healthcare analytics and readmission prediction.

---

## Data Availability and Version Control
The raw dataset file (`diabetic_data.csv`) is **not committed to this repository** to keep the project lightweight and to follow best practices for data governance.

To reproduce this project:
1. Download the dataset from the UCI Machine Learning Repository.
2. Extract the file `diabetic_data.csv`.
3. Place it in this directory:


All notebooks assume this relative file path.

---

## Local Context and Applicability
At present, there are no publicly available patient-level hospital encounter datasets from the Philippines due to data privacy regulations and fragmented health information systems.

This dataset is therefore used to demonstrate a **methodologically transferable machine learning workflow** that can be adapted to Philippine tertiary hospital settings following appropriate local data collection, validation, and governance approvals.

---

## Ethical and Privacy Considerations
- The dataset is fully de-identified and publicly released for research purposes.
- No personally identifiable information (PII) is included.
- Model outputs are intended to support clinical decision-making, not replace professional medical judgment.

Any real-world deployment would require local validation, governance approval, and compliance with applicable data privacy regulations.
