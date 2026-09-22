# MaryamBuQurayn_Capston_Project_Advanced_ML_Techniques

أساليب تعلم الآلة المتقدمة-(https://github.com/SDAIAAcademy) 

# Diabetes Prediction: From Raw Data to Evaluation

A step-by-step machine learning project that takes raw patient data through cleaning, modeling, and interpretation.

---

## Task

**Binary Classification:** predict whether a patient has diabetes (`1`) or not (`0`).

---

## Dataset

| Feature | Type | Description |
|---|---|---|
| `Age` | Numerical | Patient age |
| `BMI` | Numerical | Body Mass Index |
| `Glucose` | Numerical | Blood glucose level (mg/dL) |
| `BloodPressure` | Numerical | Blood pressure |
| `Insulin` | Numerical | Insulin level |
| `Gender` | Categorical | Male / Female |
| `FamilyHistory` | Categorical | Family history of diabetes |
| `SmokingStatus` | Categorical | Smoking status |
| `ActivityLevel` | Ordinal | Low / Medium / High |
| `Diabetes` | Target | 1 = diabetes, 0 = no diabetes |

---

## Roadmap

| # | Step | Description |
|---|---|---|
| 0 | Setup | Import libraries and load the data |
| 1 | Understand the Data | Review the feature table |
| 2 | EDA | Single-column analysis, then relationships between columns |
| 3 | Imputation | Handle missing values (NaN and hidden zeros) |
| 4 | Cleaning | Remove duplicates and fix inconsistent text |
| 5 | Encoding | Convert categorical columns to numbers |
| 6 | Correlation Matrix | Check relationships between features |
| 7 | Train/Test Split | Split the data and apply standardization |
| 8 | Modeling | Train XGBoost and LightGBM |
| 9 | Exercise | Compute the evaluation metrics yourself |
| 10 | Answers | Confusion Matrix and all performance metrics |
| 11 | SHAP | Model interpretability: why did the model decide this? |

---

## Tech Stack

- **Python**
- **pandas, NumPy** – data handling
- **Matplotlib, Seaborn** – visualization
- **scikit-learn** – preprocessing and metrics
- **XGBoost, LightGBM** – models
- **SHAP** – model explainability

---

## Key Findings

- `Glucose` is the strongest single predictor
- Classes are **imbalanced** (~67% non-diabetic), so Precision, Recall, and F1-Score are used alongside Accuracy
- Diabetes rate decreases as activity level increases
