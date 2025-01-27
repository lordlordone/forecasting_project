# Project description

The goal of this project was to develop a model for forecasting the demand for flight seats for an airline company. The modeling approach focused on statistical techniques, specifically using SARIMA and ARIMA models.


# Methodology

The analysis began with an exploration of the time series of seat demand. After decomposing the series, it was evident that its components exhibited multiplicative effects. To address this, a logarithmic transformation was applied, converting the series into an additive model. A 1-st order differentiation was applied to eliminate trend-effect and make it stationary and then an analysis of this new series has been performed. A SARIMA model was fitted, and a residual analysis confirmed that the residuals were normally distributed and showed no significant autocorrelation. In order to confirm that the found model has a good generalization cross-validation was performed.


# Model selection

Although the notebook includes only one model, several ones were tested during the development phase. The selection criteria which leads to the one in the notebook was the minimization of the AIC and the maximization of the log-likelihood and ensuring the statistical significance of the model's coefficients through hypothesis testing.


# Frameworks and libraries

  - Pandas: For data manipulation and preprocessing
  - statsmodels: For time series modelling and analysis


# How to reproduce this notebook:

It is reproducible on Google Colab. Simply update the path in the second cell to point to the location of the 'AirPassengers.csv' file.
