---
title: "Time Series ARIMA and SARIMAX for Covid-19 Forecasting"
description: "Vector Autoregressive (VAR) model, Granger causality test:, ARIMA and SARIMAX used to determine the covid-19 forecasting in Boston"
dateString: Dec 2022
draft: false
tags: ["Time Series", "ARIMA", "SARIMAX", "Hypothesis Testing", "Finance"]
showToc: false
weight: 206
cover:
    image: "projects/TimeSeries/Time-Series-Analysis.png"
--- 
### 🔗 [GitHub repository](https://github.com/Abhiashu10/TImeSeries-ARIMA-Covid19-Forecasting.git)

## Description
The goal of this analysis is to forecast the number of positive COVID-19 tests in Boston based on various factors such as emergency department visits, hospitalizations, airport passenger arrivals, and COVID-19 testing data. The dataset contains information about these variables over time.

## Technique Used
The technique used in the code is Vector Autoregression (VAR) modeling. VAR is a multivariate time series analysis method that models the relationship between multiple variables as a system of equations. It extends the autoregressive (AR) model to multiple variables.
- Causal Analysis: Granger causality tests are performed to determine the causal relationship between the variables.
- Johansen's Cointegration Test is conducted to check for long-term equilibrium relationships among the variables.
- Stationarity Check: Augmented Dickey-Fuller (ADF) test is performed to test the stationarity of the variables.
If the variables are non-stationary, differencing is applied to make them stationary.
- Model Order Selection:Different lag orders (p) are tested using the VAR model, and the Akaike Information Criterion (AIC) is used to select the optimal lag order.
- Model Training and Forecasting: The VAR model is fitted to the training data.Serial correlation of residuals is checked using the Durbin-Watson statistic.The model is used to forecast future values based on the differenced data.

![my notes](/projects/TimeSeries/HeatMap.png)

### 🔗 [GitHub Code](https://github.com/Abhiashu10/TImeSeries-ARIMA-Covid19-Forecasting/blob/0531a660de0e65cc35e01c23b4c29dd90b110cc1/Time_Series-ARIMA-%20Boston_Covid19_ForeCasting.ipynb)


