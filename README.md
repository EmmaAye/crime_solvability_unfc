# 📊 Solving Crime in Los Angeles: Predictive Modeling for Case Solvability

This project focuses on analyzing and modeling crime data from Los Angeles to predict whether reported crime cases are likely to be solved. The project was conducted as part of the **CPSC 610 - Python for Data Analytics** course and applies machine learning techniques to a real-world criminal dataset.

## 📁 Project Overview

The goal of this project is to support public safety efforts and resource planning by identifying which types of crimes and circumstances are more or less likely to result in case resolution. We formulated research questions and hypotheses, engineered features from raw data, and applied classification models to assess case solvability.

## 🎯 Objectives

- Identify patterns and trends that influence whether a crime gets solved.

- Build predictive models using historical crime data from Los Angeles.

- Evaluate the models using metrics like accuracy, precision, recall, and F1-score.

- Derive actionable insights for policy-making and public safety improvement.

## 🧪 Research Questions


- **Primary Question**: What features influence the likelihood of a case being solved?

- **Sub-questions**:

  - Are cases more likely to be solved if the suspect's information is available?

  - Does the use of a weapon or the type of crime impact case resolution?

  - Are demographic or geographic factors statistically significant?

## 🧹 Data Preprocessing & Feature Engineering

- Cleaned nulls and reformatted datetime features.

- Created engineered features such as:

  - **Report delay** (days between occurrence and reporting)

  - **Crime type encoding** (top 40 frequent crime codes)

  - **Weapon code grouping**

  - **Victim/suspect demographics**

  - **Normalized location data (lat/lon)**

## ⚙️ Modeling & Evaluation

- Trained multiple classification models:

  - **Logistic Regression**

  - **Random Forest**

  - **XGBoost**

- Evaluated using:

  - Accuracy

  - Precision, Recall, F1-score

  - ROC-AUC Curve

- Used cross-validation and grid search for tuning.

## 📈 Key Findings
- Cases with suspect age, gender, and known weapon were significantly more likely to be solved.

- Shorter delays between crime occurrence and reporting improved solvability.

- Certain crime types (e.g., assaults) showed higher clearance rates than others (e.g., vandalism or burglary).

- XGBoost showed the best performance with balanced precision and recall.

## 🛠 Tools & Technologies
- Python (Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn)

- Jupyter Notebook

- Git/GitHub

## 📌 Future Work
- Remove the feature incident_admincode_1, which may be data leakage or not generalizable, and retrain the models to assess robustness.

- Explore additional model types such as LightGBM and CatBoost.

- Experiment with deep learning models (e.g., RNNs or attention-based architectures).

- Integrate contextual data such as neighborhood-level crime rates, income levels, or police department staffing levels.

- Conduct fairness analysis to ensure models do not reinforce bias based on race, gender, or socioeconomic status.

## 🙌 Acknowledgements

This project was completed as part of **CPSC 610 – Python for Data Analytics** at the **University of Niagara Falls Canada**. Special thanks to our instructor and teaching assistants for guidance throughout this assignment.
