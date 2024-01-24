# Time Series Analysis and ARIMA Forecasting

## Overview

This repository contains code for time series analysis and forecasting using the ARIMA (AutoRegressive Integrated Moving Average) model. The dataset used in this analysis is related to CPU usage over time. The primary goal is to demonstrate the process of time series decomposition, stationarity testing, and ARIMA modeling.

## Table of Contents

1. [Introduction](#introduction)
2. [Dependencies](#dependencies)
3. [Dataset](#dataset)
4. [Time Series Decomposition](#time-series-decomposition)
5. [Stationarity Testing](#stationarity-testing)
6. [ARIMA Modeling](#arima-modeling)
7. [Future Predictions](#future-predictions)
8. [Visualization](#visualization)
9. [Saving the Model](#saving-the-model)
10. [Additional Resources](#additional-resources)

## Introduction

This repository provides a comprehensive analysis of time series data related to CPU usage. The main focus is on understanding the temporal patterns, decomposing the time series into trend, seasonal, and residual components, testing for stationarity, and making future predictions using the ARIMA model.

## Dependencies

The following Python libraries are used in this project:
- pandas
- numpy
- matplotlib
- seaborn
- sqlite3
- statsmodels
- pmdarima

## Dataset
The dataset consists of CPU usage data, with timestamps and corresponding CPU values. Two sets, train_data and test_data, are loaded from CSV files for training and testing purposes.

## Time Series Decomposition
The time series is decomposed into its trend, seasonal, and residual components using the seasonal decomposition function from statsmodels.

## Stationarity Testing
The Augmented Dickey-Fuller (ADF) test is employed to determine the stationarity of the time series. Results indicate that the time series is stationary, implying no significant trend.

## ARIMA Modeling
The ARIMA model is applied to the stationary time series, and the best-fitting parameters are determined using the auto_arima function from pmdarima. The model summary provides information about the chosen order and seasonal order.

## Future Predictions
The trained ARIMA model is used to make future predictions. The forecasted values are then visualized alongside the original stationary time series.

## Visualization
Visualizations include plots of the original time series, trend, seasonal component, residual, autocorrelation function (ACF), and forecasted values.

## Saving the Model
The trained ARIMA model is saved using the pickle library for future use. The saved model file is named modelo_arima.pkl.

## Additional Resources
For further details on time series analysis, stationarity testing, and ARIMA modeling, refer to the accompanying PDF document.
