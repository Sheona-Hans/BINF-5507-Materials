# Heart Disease Dataset - Regression Model Analysis

This repository provides a regression analysis pipeline using the **Heart Disease** dataset from OpenML. The goal is to **predict serum cholesterol ('chol')** based on other patient features using an **ElasticNet regression model** with hyperparameter tuning and performance visualization.

---

## Project Overview

- Load and inspect the dataset
- Check for missing values and summarize dataset statistics
- Use 'ElasticNet' regression to model cholesterol levels
- Perform **grid search** over 'alpha' and 'l1_ratio'
- Evaluate model performance with **R² score** and **RMSE**
- Visualize results using **heatmaps**

---

## How to run
Open the notebook
Filename: main.ipynb
Execute each cell of the notebook sequentially until classification model

# Heart Disease Classification with Logistic Regression and k-NN

This project implements and evaluates two classification algorithms — **Logistic Regression** and **k-Nearest Neighbors (k-NN)** — to predict the presence of heart disease using the **Heart Disease** dataset from OpenML from OpenML.

---

## Project Overview

- Load and clean the dataset
- Define binary classification target ('target': presence of heart disease)
- Implement Logistic Regression with different solvers and penalties
- Implement k-NN with varying values of 'k'
- Evaluate models using Accuracy, F1 Score, AUROC, and AUPRC
- Plot ROC and Precision-Recall curves for the best models

---

## How to run
Open the notebook
Filename: main.ipynb
Execute each cell of the notebook sequentially from Classification model