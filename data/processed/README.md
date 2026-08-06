# Processed Data

This folder contains the cleaned and preprocessed version of the Beijing Multi-Site Air Quality Dataset used in the QM640 Data Analytics Capstone project.

## File

`air_quality_processed_dataset.zip`

The processed dataset was generated after data integration and preprocessing, including:

- Missing-value treatment
- Duplicate record verification
- Outlier assessment
- Datetime construction
- Data quality verification

The final forecasting target (`PM2.5_next_hour`) and subsequent predictor preparation are performed within the project notebook as part of the one-hour-ahead PM2.5 forecasting workflow.

The complete modelling and evaluation process is available in:

`notebooks/QM640_Air_Quality_Capstone_Project.ipynb`
