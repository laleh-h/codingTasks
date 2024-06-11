# Predicting Diabetes Progression: A Multiple Linear Regression Approach

## Description
This project develops a multiple linear regression model to predict the one-year progression of diabetes (PROGRESSION) using various demographic and health-related features. The features include age, sex, body mass index (BMI), average blood pressure (BP), and six blood serum measurements (S1-S6). By leveraging these predictors, the model aims to provide accurate predictions of diabetes progression, offering valuable insights for healthcare providers and patients.

## Required Libraries
- `pandas`
- `numpy`
- `matplotlib.pyplot`
- `seaborn`
- `scipy.stats`
- `sklearn.preprocessing`
- `sklearn.model_selection`
- `sklearn.linear_model`
- `sklearn.metrics`
- `joblib`

## Dataset

The dataset used in the diabetes progression analysis contains information about individuals' demographics, health metrics, and diabetes progression measurements. The dataset includes the following columns:

- `AGE`: The age of the individual.
- `SEX`: The gender of the individual (1 for male, 2 for female).
- `BMI`: Body mass index, a measure of body fat based on height and weight.
- `BP`: Average blood pressure.
- `S1-S6`: Six blood serum measurements.
- `PROGRESSION`: The target variable indicating the one-year progression of diabetes. It refers to the change or advancement in the severity or stage of diabetes over a one-year period. It is a measure of how much the condition of diabetes has worsened or improved for an individual within that timeframe.