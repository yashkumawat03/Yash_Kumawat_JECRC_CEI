# Tesla Deliveries Forecasting - End-to-End Machine Learning Pipeline

## Project Overview

This project focuses on analyzing and forecasting Tesla vehicle deliveries using Machine Learning and Time Series Forecasting techniques. The goal is to identify key factors affecting deliveries and predict future delivery trends.

## Dataset

The dataset contains Tesla vehicle delivery information from 2015 to 2025, including:

* Year and Month
* Region
* Vehicle Model
* Production Units
* Average Price (USD)
* Battery Capacity
* Vehicle Range
* Charging Stations
* Estimated Deliveries

## Project Workflow

### 1. Data Preprocessing

* Loaded and explored the dataset
* Checked for missing values and duplicates
* Cleaned and prepared the data for analysis

### 2. Exploratory Data Analysis (EDA)

* Analyzed delivery trends over time
* Studied regional and model-wise deliveries
* Examined relationships between numerical features using correlation analysis

### 3. Feature Engineering

* Created Delivery Efficiency feature
* Created Price per KM feature
* Converted Year and Month into a Date column for time series analysis

### 4. Machine Learning Models

* Linear Regression
* Random Forest Regressor

### 5. Hyperparameter Tuning

* Applied GridSearchCV to optimize Random Forest parameters
* Selected the best-performing model based on evaluation metrics

### 6. Feature Importance Analysis

* Identified the most influential features affecting vehicle deliveries

### 7. Time Series Forecasting

* Forecasted future Tesla deliveries using Holt-Winters forecasting techniques
* Predicted delivery trends for the next 12 months

## Evaluation Metrics

The models were evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

## Key Findings

* Random Forest performed better than Linear Regression.
* Production Units and Average Price were among the most important factors influencing deliveries.
* Historical delivery patterns showed seasonal trends.
* Forecasting models successfully predicted future delivery demand.

## Conclusion

This project demonstrates a complete end-to-end Machine Learning pipeline, including data preprocessing, exploratory analysis, feature engineering, model development, hyperparameter tuning, feature importance analysis, and time series forecasting.


## Note

GitHub may display an "An error occurred" message while rendering the notebook preview. The notebook file itself is valid and opens correctly in Jupyter Notebook and VS Code.

If the preview does not load:

1. Click **Download Raw File** or clone the repository.
2. Open the `.ipynb` file using **Jupyter Notebook**, **Jupyter Lab**, or **VS Code**.
3. Run the notebook locally to view all code, visualizations, and outputs.

This issue is related to GitHub's notebook preview renderer and does not affect the notebook content or functionality.
