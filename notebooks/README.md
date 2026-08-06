# Notebooks

This folder contains the Jupyter notebook used for the QM640 Data Analytics Capstone project.

## Main Notebook

`QM640_Air_Quality_Capstone_Project.ipynb`

The notebook contains the complete analytical workflow for one-hour-ahead PM2.5 forecasting, including:

- Data loading and integration
- Data quality assessment and preprocessing
- Missing-value treatment and outlier assessment
- Feature engineering and creation of the one-hour-ahead target (`PM2.5_next_hour`)
- Exploratory data analysis
- Chronological training and testing split
- Development and comparison of eight regression models
- Model evaluation using MAE, RMSE, and R²
- Expanding-window time-series cross-validation
- Standardized coefficient analysis
- SHAP-based model interpretation

The notebook is designed to provide a reproducible record of the data analysis, model development, evaluation, and interpretation conducted for the capstone study.
