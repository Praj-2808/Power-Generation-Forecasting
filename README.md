# Power Generation Forecasting and Analysis Using CEA Monthly Generation Reports

## Overview

This project focuses on analyzing and forecasting electricity generation in India using monthly generation reports published by the Central Electricity Authority (CEA) through the National Power Portal (NPP). The objective is to understand historical generation trends and develop predictive models that can forecast future power generation levels.

The dataset contains region-wise statistics for Thermal, Hydro, and Nuclear power generation, including monitored capacity, target generation, actual generation, previous year generation, and Plant Load Factor (PLF). Monthly reports from January 2022 to May 2026 were collected, processed, and consolidated into a structured dataset for analysis.

## Objectives

* Collect and consolidate monthly CEA generation reports.
* Perform data cleaning and preprocessing.
* Analyze generation trends across regions and power sources.
* Identify seasonal and temporal patterns in electricity generation.
* Build forecasting models to predict future generation levels.
* Compare model performance using standard evaluation metrics.

## Data Collection and Preparation

Monthly generation reports were automatically downloaded from the National Power Portal and converted into a unified dataset. The preprocessing stage included:

* Removal of inconsistent and duplicate records.
* Handling of missing values.
* Standardization of column names and formats.
* Transformation of monthly reports into a structured time-series dataset.

## Exploratory Data Analysis

Comprehensive exploratory analysis was conducted to understand power generation behavior across India.

The analysis included:

* Trend analysis of electricity generation over time.
* Source-wise comparison of Thermal, Hydro, and Nuclear generation.
* Region-wise generation analysis.
* Seasonal pattern identification.
* Plant Load Factor (PLF) analysis.
* Correlation and multivariate analysis of generation-related variables.

## Feature Engineering

To improve forecasting accuracy, several time-series features were created:

* Month
* Quarter
* Year
* Lag Features
* Rolling Averages
* Growth Rates

These features help capture seasonality, long-term trends, and historical dependencies within the data.

## Forecasting Models

Three forecasting approaches were evaluated:

### SARIMA

Statistical time-series forecasting model designed to capture trend and seasonality patterns.

### Prophet

Forecasting framework developed for handling seasonality, trend changes, and missing data.

### XGBoost

Machine learning-based regression model utilizing engineered temporal features and historical generation patterns.

## Model Evaluation

The forecasting models were compared using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* Mean Absolute Percentage Error (MAPE)
* R² Score

Among the evaluated models, XGBoost achieved the best overall performance and demonstrated superior predictive capability for electricity generation forecasting.

## Results

The analysis revealed significant regional and seasonal variations in electricity generation across India. Feature engineering substantially improved forecasting performance, while XGBoost effectively captured complex patterns present in the historical data.

The developed forecasting framework provides valuable insights that can support energy planning, operational decision-making, and resource management within the power sector.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Statsmodels
* Prophet
* XGBoost
* Jupyter Notebook

## Conclusion

This project demonstrates the application of data analytics and time-series forecasting techniques to India's power generation sector. By combining historical generation data with machine learning and statistical forecasting methods, the project provides an effective framework for analyzing generation trends and predicting future electricity production.
