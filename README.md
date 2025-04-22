# airplane-passenger-forecast 🛫
![image](https://github.com/user-attachments/assets/fbc872c3-a782-4b9e-b111-8a379f5da83d)

This project implements forecasting the number of airplane passengers based on historical data. The model is built using SARIMA (Seasonal AutoRegressive Integrated Moving Average) along with ACF (AutoCorrelation Function) and PACF (Partial AutoCorrelation Function) analysis for selecting the optimal parameters. Forecasting is done on a test dataset, which was split into train and test subsets.

## Description

The project focuses on predicting the number of passengers based on historical data. The SARIMA model is used to account for seasonal fluctuations in the data, allowing for more accurate predictions of time series behavior. The dataset was split into a training set (`train`) for model training and a testing set (`test`) for evaluating the forecasting performance.

The dataset can be downloaded from Kaggle using `kagglehub`. The data contains historical passenger counts for analysis and model training.

## Repository Structure

- **SARIMA.ipynb** — Jupyter notebook for data analysis, model building, and testing.
- **LICENSE** — License file for the project.
## Methods Description
**SARIMA (Seasonal AutoRegressive Integrated Moving Average)**
SARIMA is an extension of the ARIMA model that accounts for seasonal components in the data. It is suitable for time series data that exhibit periodic trends.

**ACF (AutoCorrelation Function)**
ACF helps assess the dependence of the current value of the time series on its previous values. This analysis is used to select the order of the autoregressive (AR) component of the model.

**PACF (Partial AutoCorrelation Function)**
PACF helps evaluate the relationship between time series values while removing the influence of intermediate values. This analysis helps determine the order of the Moving Average (MA) component of the model.

If you'd like to contribute to this project, please fork the repository, make your changes, and create a pull request.

## Dataset
You can download kaggle dataset using kagglehub library
```bash
  import kagglehub
  # Download latest version
  path = kagglehub.dataset_download("ashfakyeafi/air-passenger-data-for-time-series-analysis")
  print("Path to dataset files:", path)
```
If you'd like to contribute to this project, please fork the repository, make your changes, and create a pull request.
