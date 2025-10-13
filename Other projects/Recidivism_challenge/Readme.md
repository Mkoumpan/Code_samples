# Recidivism Forecasting Challenge

## Overview
This project was developed for the [NIJ Recidivism Forecasting Challenge](https://nij.ojp.gov/funding/recidivism-forecasting-challenge), which aimed to improve the prediction of recidivism outcomes using advanced data-driven approaches. The challenge focused on developing transparent, fair, and explainable models to support decision-making in criminal justice systems.

---

## Situation
Recidivism—when individuals reoffend after being released from incarceration—is a complex issue with societal, economic, and ethical implications. The challenge provided anonymized datasets from various jurisdictions, containing demographic, criminal history, and supervision data.  
The goal was to create models that could accurately forecast recidivism risk while maintaining fairness and interpretability.

---

## Task
Develop and evaluate predictive models for recidivism over 3-year and 6-year horizons.  
Key requirements included:
- Handling missing and imbalanced data.
- Ensuring fairness across demographic subgroups.
- Providing interpretable outputs that could guide policy and decision-making.

---

## Action
- **Data Preprocessing:** Cleaned and standardized datasets, engineered features from criminal history and demographic variables, and applied techniques to mitigate data imbalance.  
- **Modeling:** Trained multiple machine learning models (e.g., Logistic Regression, Random Forest, XGBoost) and tuned hyperparameters using cross-validation.  
- **Fairness & Interpretability:** Assessed performance across demographic groups to detect bias, and used SHAP values for explainability.  
- **Evaluation Pipeline:** Implemented modular Python scripts (via Jupyter Notebook) to handle data loading, training, and evaluation consistently across forecast windows.  
- **Version Control & Reproducibility:** Documented the workflow in this repository with reproducible code and results.

---

## Result
- Achieved competitive predictive performance with **balanced accuracy and AUC improvements** over baseline models.  
- Demonstrated that interpretability and fairness can be incorporated without significant performance loss.  
- Provided a transparent and reproducible workflow that aligns with responsible AI practices in the criminal justice domain.

---

## Technologies Used
- **Python**, **Pandas**, **NumPy**, **Scikit-learn**, **XGBoost**, **Tensorflow**
- **Jupyter Notebook** for experimentation and reporting
- **Matplotlib / Seaborn** for data visualization

---
