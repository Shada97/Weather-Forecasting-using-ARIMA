# Weather-Forecasting-using-ARIMA
## Introduction

Accurate weather forecasting is crucial for various societal functions, including scheduling, resource allocation, air traffic management, and disaster mitigation. Inaccurate forecasts can disrupt logistics, agriculture, energy management, and even lead to loss of life. This project focuses on developing a robust weather forecasting model using historical time series weather data. It will cover the dataset used, the chosen forecast model, the development methodology, and an analysis of the training and prediction results.

## Dataset

The historical weather dataset utilized in this project is sourced from <a href="https://www.ncei.noaa.gov/cdo-web/datasets"> NOAA Climate Data Online (CDO)</a>, which is a comprehensive archive recording climate data from
weather stations around the world. For demonstration purposes, our project would base
the forecast model on one of the climate variables originating from the region of Toronto
Pearson international Airport.

## Methodology

This project uses the ARIMA (AutoRegressive Integrated Moving Average) model for weather forecasting due to its ability to handle time series data with trends and seasonality. The project compares manual and automatic ARIMA model fitting methods using Python libraries "statsmodels" and "pmdarima."

The implementation process includes:
1. **Data cleaning**: Handling missing values and preparing the dataset.
2. **Data exploration**: Analyzing normality, correlations, seasonality, and stationarity.
3. **Data preprocessing**: Applying non-seasonal and seasonal differencing to achieve stationarity.
4. **Model selection**: Determining the ARIMA model's order using ACF, PACF, and other tests.
5. **Manual ARIMA fitting**: Manually defining the ARIMA parameters, fitting the model, and adjusting parameters based on residual analysis.
6. **Auto ARIMA fitting**: Using "pmdarima" to automatically fit the ARIMA model and compare it with the manual approach.
7. **Model validation**: Evaluating both models' performance using mean square error and comparing the results to actual data.

## Results

| Accuracy Metrics       | Manual - ARIMA (1, 1, 1) × (0, 1, 1)<sub>52</sub>       |
|-----------------|----------------|
| MPE    | 3.079  |
| MSE    | 8.935  |
| MAE    | 2.429  |
| MAPE   | 3.298  |

Below are the visualization of the final model predictions.

![Prediction1](https://tinyurl.com/46nntrh7)
![Prediction2](https://tinyurl.com/d23ukr7v)

## Interested?
The fastest way to contact me is by shooting me an email to: arabis3@mcmaster.ca

