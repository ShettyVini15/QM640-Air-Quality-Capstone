# Machine Learning-Based Forecasting of Urban Air Quality Using Environmental and Meteorological Data

## Overview

This repository contains the **QM640 Data Analytics Capstone** project titled **Machine Learning-Based Forecasting of Urban Air Quality Using Environmental and Meteorological Data**.

The project develops and evaluates machine learning regression models for **one-hour-ahead PM2.5 forecasting** using air pollutant, meteorological, temporal, wind-direction, and monitoring-station variables from the **Beijing Multi-Site Air Quality Dataset**.

The study compares multiple regression algorithms to identify a robust and interpretable model for short-term PM2.5 forecasting and potential air-quality monitoring applications.

## Objectives

- Forecast **PM2.5 concentration one hour ahead** using machine learning regression models.
- Compare the predictive performance of multiple regression algorithms using **MAE, RMSE, and R²**.
- Examine the contribution of pollutant, meteorological, temporal, and location-related variables to one-hour-ahead PM2.5 forecasting.
- Evaluate the temporal robustness of the selected model using **time-series cross-validation**.
- Improve model interpretability using **standardized coefficients and SHAP analysis**.

## Dataset

**Source:** UCI Machine Learning Repository – Beijing Multi-Site Air Quality Dataset

https://archive.ics.uci.edu/dataset/501/beijing+multi+site+air+quality+data

The dataset contains hourly air-quality and meteorological observations collected from **12 monitoring stations in Beijing** between **March 2013 and February 2017**.

The original dataset contains **420,768 observations and 18 variables**.

## Machine Learning Models

The following eight regression models were evaluated:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor
- Gradient Boosting Regressor
- AdaBoost Regressor
- LightGBM Regressor
- CatBoost Regressor

## Model Evaluation

Model performance was evaluated using:

- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **Coefficient of Determination (R²)**

A **chronological training and testing split** was used to preserve the temporal structure of the forecasting problem.

The selected model was further evaluated using **5-fold expanding-window time-series cross-validation**.

## Key Result

Based on the chronological testing results, **Linear Regression emerged as the leading model overall**, achieving:

- **Test MAE:** 10.16 µg/m³
- **Test RMSE:** 19.13 µg/m³
- **Test R²:** 0.9477

Although **LightGBM achieved the lowest Test MAE of 9.85 µg/m³**, Linear Regression achieved the **highest Test R² and lowest Test RMSE** and was selected for further robustness and interpretability analysis.

## Model Interpretability

The selected Linear Regression model was interpreted using:

- **Standardized coefficient analysis**
- **SHAP (SHapley Additive exPlanations) analysis**

The interpretability analysis identified **current-hour PM2.5 concentration as the dominant predictor of one-hour-ahead PM2.5 concentration**, with additional contributions from pollutant, meteorological, and temporal variables.

## Repository Structure

```text
QM640-Air-Quality-Capstone/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── reports/
├── images/
├── README.md
├── requirements.txt
└── .gitignore
```

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- LightGBM
- CatBoost
- SHAP
- Jupyter Notebook

## Project Status

**Current Stage:** Machine learning analysis and model evaluation completed.

Completed activities include:

- Data preprocessing
- Exploratory data analysis
- One-hour-ahead forecasting target creation
- Feature preparation and categorical encoding
- Chronological train-test splitting
- Development and evaluation of eight regression models
- Model performance comparison
- Time-series cross-validation of the selected model
- Standardized coefficient analysis
- SHAP model interpretability analysis
- Interim report preparation

**Next Stage:** Final report refinement, mentor/evaluator feedback, and completion of subsequent capstone deliverables.

## Author

**Vinita R. Shetty**

QM640 Data Analytics Capstone  
Walsh College
