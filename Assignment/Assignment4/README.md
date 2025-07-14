# Survival Analysis: Kaplan-Meier, Cox Proportional Hazards, and Random Survival Forests Comparison

This repository compares three survival analysis methods: **Kaplan-Meier** (KM) survival curves, **Cox Proportional Hazards regression**, and **Random Survival Forests** (RSF). The comparison is performed on a clinical dataset to assess the impact of various factors (e.g., age, cancer stage, treatment modality) on patient survival. 

### Introduction
Survival analysis is a statistical method used to analyze the time to an event, such as death, relapse, or failure, and determine factors that influence the timing of the event. This repository compares the performance and applicability of three survival analysis methods:

1. **Kaplan-Meier**: A non-parametric estimator of the survival function, commonly used to estimate survival curves.
2. **Cox Proportional Hazards Regression**: A semiparametric regression model used to assess the effect of covariates on survival time.
3. **Random Survival Forests**: A machine learning-based method that can capture complex, non-linear relationships between covariates and survival outcomes.

The dataset used for analysis contains clinical information on patients, including their **age**, **sex**, **stage of cancer**, **treatment modality**, and **survival time**. I use these variables to evaluate their impact on survival outcomes using the three methods.

### Methods

#### Kaplan-Meier (KM) Analysis
- The Kaplan-Meier method estimates the survival function from lifetime data.
- It is useful for comparing the survival rates between different groups (e.g., treatment type, stage of cancer) and visualizing survival curves.
- **Log-rank test** is used to compare survival differences between groups.

#### Cox Proportional Hazards Regression
- The Cox regression model is used to identify the relationship between survival time and one or more covariates.
- It assumes proportional hazards, meaning that the hazard ratio between groups is constant over time.
- This model provides estimates of hazard ratios (HR), which indicate the effect of each covariate on survival.

#### Random Survival Forests (RSF)
- RSF is an ensemble learning method that uses decision trees to model survival data.
- Unlike the Cox model, it can capture non-linear interactions between covariates and does not require the proportional hazards assumption.
- It provides feature importance scores, which help identify the most influential variables in predicting survival.

### Dataset

The dataset used in this analysis is a clinical dataset, which contains the following features:
- **Age**: The patient's age at the time of diagnosis.
- **Sex**: The gender of the patient.
- **Stage**: The stage of cancer (e.g., Early or Advanced).
- **Tx Modality**: Treatment modality (e.g., ChemoRT, RT alone).
- **Length FU**: Follow-up duration (time to event or censoring).
- **Event**: The event indicator (0 = alive, 1 = dead).

### Analysis Overview

- **Kaplan-Meier** survival curves are plotted for different treatment groups and cancer stages.
- **Log-rank tests** are performed to compare the survival curves.
- **Cox Proportional Hazards Regression** is fitted to assess the impact of variables on survival. Proportional hazards assumptions are checked.
- **Random Survival Forests** are trained to predict survival and assess variable importance.

### How to Run

#### Prerequisites
Before running the code, make sure the following Python libraries are installed:
1. pandas
2. numpy
3. matplotlib
4. lifelines
5. scikit-learn
6. sksurv

#### Running the Code
1. Download or clone this repository.
2. Install the required libraries using `pip install <library_name>`.
3. Open and run the Jupyter notebook `main.ipynb`:
   - Execute each cell sequentially to perform the Kaplan-Meier, Cox regression, and Random Survival Forest analyses.
   - Review the survival plots, statistical tests, and model evaluations (C-index) in the notebook.

### Results and Observations
- The **Kaplan-Meier** analysis provides visual comparisons of survival curves for different treatment and stage groups.
- The **Cox Proportional Hazards** model provides a detailed understanding of how various covariates affect survival, including hazard ratios and significance testing.
- **Random Survival Forests** provide a powerful machine learning approach to survival analysis, with feature importance metrics highlighting key variables like age, stage, and treatment modality.

### Conclusion
- This comparison helps in understanding the advantages and limitations of traditional statistical methods (Kaplan-Meier, Cox regression) versus machine learning-based approaches (Random Survival Forests) in survival analysis.
- The Cox model provides easy interpretability with hazard ratios, but the **Random Survival Forests** offer better predictive power, especially for non-linear relationships.
