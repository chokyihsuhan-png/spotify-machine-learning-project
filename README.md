# Spotify 2023 – Data Analysis & Predictive Modelling

## Project Overview

This project was completed as part of my Master's in Business Analytics at the University of Limerick.

The objective was to analyse Spotify 2023 streaming data and develop machine learning regression models to predict the number of streams for music tracks.

The project involved exploratory data analysis, data cleaning, feature engineering, regression modelling, hyperparameter tuning and model evaluation.

## Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Analysed Spotify streaming data and descriptive statistics.
- Investigated distributions, correlations and relationships between variables.
- Explored streaming patterns and platform exposure.

### 2. Data Preparation
- Cleaned numeric and categorical variables.
- Handled missing values.
- Created a log-transformed target variable: `log_streams = log(1 + streams)`.
- Prepared features for machine learning.

### 3. Predictive Modelling

Developed and compared seven regression models:

- Baseline Linear Regression
- Ridge Regression (Tuned)
- Lasso Regression (Tuned)
- ElasticNet Regression (Tuned)
- Gradient Boosting Regressor (Untuned)
- Gradient Boosting Regressor (Tuned – Round 1)
- Gradient Boosting Regressor (Tuned – Round 2)

### 4. Model Evaluation

Models were evaluated using:
- RMSE (Root Mean Squared Error)
- R² (Coefficient of Determination)

The same 80/20 train-test split and log-transformed target were used for the final seven-model comparison.

### Model Performance

| Model | Test RMSE | Test R² |
|---|---:|---:|
| Linear Regression | 0.6792 | 0.5029 |
| Ridge | 0.6766 | 0.5068 |
| Lasso | 0.6734 | 0.5114 |
| ElasticNet | 0.6696 | 0.5168 |
| GBR (Untuned) | 0.3442 | 0.8723 |
| GBR (Tuned Round 1) | 0.3568 | 0.8628 |
| GBR (Tuned Round 2) | 0.3570 | 0.8626 |

The untuned Gradient Boosting Regressor achieved the highest test R² of 0.8723 in the final comparison.

## Technologies & Libraries

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy

## Repository Structure

- `notebooks/` – Exploratory analysis, data preparation and modelling.
- `data/` – Original and prepared datasets.

## Key Learning Outcomes

- Exploratory Data Analysis and data visualisation.
- Data cleaning and feature engineering.
- Regression modelling and machine learning.
- Hyperparameter optimisation using GridSearchCV.
- Model evaluation and performance comparison.
- Data-driven interpretation and problem-solving.

## Academic Context

Module: CS6471 – Artificial Intelligence and Machine Learning for Business 
University: University of Limerick

This project was completed as part of Master's coursework.



