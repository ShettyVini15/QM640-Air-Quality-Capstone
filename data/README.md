# Data

This folder contains the raw and processed data used in the QM640 Data Analytics Capstone project, **Machine Learning-Based Forecasting of Urban Air Quality Using Environmental and Meteorological Data**.

## Dataset Source

The study uses the **Beijing Multi-Site Air Quality Dataset** from the UCI Machine Learning Repository.

Dataset reference:

Chen, S. (2017). Beijing Multi-Site Air Quality [Data set]. UCI Machine Learning Repository.  
https://doi.org/10.24432/C5RK5G

## Data Structure

### Raw Data

The `raw/` folder contains the original 12 station-level CSV files covering hourly air quality and meteorological observations from 1 March 2013 to 28 February 2017.

### Processed Data

The `processed/` folder contains the cleaned and preprocessed dataset used for subsequent analysis.

The final one-hour-ahead forecasting target (`PM2.5_next_hour`) and predictor preparation are performed within the project notebook.

## Reproducibility

The complete analytical workflow is available in:

`notebooks/QM640_Air_Quality_Capstone_Project.ipynb`

The notebook includes data preprocessing, exploratory data analysis, feature engineering, one-hour-ahead target construction, chronological train-test splitting, machine learning model development, model evaluation, time-series cross-validation, and model interpretation.
