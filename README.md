# Combined Cycle Power Plant Regression Analysis

This project involves analyzing and predicting the electrical energy output of a Combined Cycle Power Plant using various regression models. The dataset spans 6 years and includes hourly average measurements of ambient conditions as predictors. This project was completed as part of Homework 2 for the DSCI 552 course, covering concepts in regression, interaction terms, and model evaluation.

## Table of Contents
- [Project Overview](#project-overview)
- [Data Exploration](#data-exploration)
- [Regression Models](#regression-models)
- [Nonlinear and Interaction Terms](#nonlinear-and-interaction-terms)
- [K-Nearest Neighbors Regression](#k-nearest-neighbors-regression)
- [Results and Analysis](#results-and-analysis)
- [Requirements](#requirements)

## Project Overview
The objective is to predict the net hourly electrical energy output (EP) of the power plant using ambient variables:
- Temperature (T)
- Ambient Pressure (AP)
- Relative Humidity (RH)
- Exhaust Vacuum (V)

The dataset can be found on the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Combined+Cycle+Power+Plant).

## Data Exploration
- The dataset was examined to understand its structure, including:
  - Number of rows and columns.
  - Statistical summaries: mean, median, range, quartiles, and interquartile ranges.
- Pairwise scatterplots were created for each predictor and the response variable to examine potential relationships.

## Regression Models
1. **Simple Linear Regression**  
   Simple linear regressions were fit for each predictor against the response. Plots were created to analyze statistical significance and identify any potential outliers.

2. **Multiple Linear Regression**  
   A multiple regression model was built using all predictors to test significance across all variables. Predictors with statistically significant associations were identified.

3. **Comparison of Univariate and Multiple Regression Coefficients**  
   Coefficients from simple and multiple regressions were compared to assess consistency across models.

## Nonlinear and Interaction Terms
- Polynomial regression was applied to test for nonlinear relationships between predictors and the response.
- Interaction terms were incorporated in a full model to test for significant interactions among predictors.

## K-Nearest Neighbors Regression
- K-Nearest Neighbors (KNN) regression was performed using both normalized and raw feature values.
- The optimal `k` was selected by testing values from 1 to 100 and plotting training and testing errors.

## Results and Analysis
- Results from the linear regression models and KNN regression were compared, identifying the model with the lowest test error.
- Train and test Mean Squared Errors (MSE) were reported, and models were evaluated based on their predictive performance.

## Requirements
The project requires:
- Python
- Libraries: `numpy`, `pandas`, `matplotlib`, `sklearn`