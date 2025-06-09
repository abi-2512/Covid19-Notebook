# COVID-19 Cases Analysis and Forecasting Project

## Overview
Our 2nd Year Final Project analyzes and forecasts COVID-19 cases in five countries (India, USA, United Kingdom, Russia, and Iran) using machine learning models and time series forecasting. The analysis compares Linear Regression and Random Forest Regressor models, then implements ARIMA models for time series forecasting of new cases.

## Features
- Data extraction from Our World in Data COVID-19 dataset
- Comparison of two regression models (Linear Regression vs. Random Forest)
- Time series forecasting with ARIMA models
- Visualization of actual vs. predicted cases
- 7-day case forecasting for each country
- Performance evaluation using RMSE

## Requirements
- Python 3.7+
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn
  - statsmodels
  - pmdarima
  - yellowbrick

## Installation
```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels pmdarima yellowbrick
```

## Project Structure
1. **Data Preparation**: 
   - Load COVID-19 dataset from OWID
   - Filter data for 5 countries
   - Handle missing values
   - Feature engineering

2. **Model Comparison**:
   - Linear Regression models for each country
   - Random Forest Regressor models
   - Performance evaluation using RMSE
   - Visualization of predictions vs actual data
   - Prediction error analysis

3. **Time Series Forecasting**:
   - ARIMA model parameter selection
   - Model fitting and evaluation
   - 7-day case forecasting
   - Comparison of ARIMA vs regression models

## Key Findings
1. **Model Performance**:
   - Random Forest Regressor outperformed Linear Regression in all countries
   - ARIMA models showed the best performance overall with the lowest RMSE
   
2. **Country Analysis**:
   - Each country showed distinct COVID-19 case patterns
   - Forecasting accuracy varied by country based on case volatility

3. **7-Day Forecast**:
   - Generated case predictions for next week
   - Visualized forecast trends for each country

## How to Use
1. Run the Jupyter notebook sequentially
2. Modify the `countries` list to analyze different countries
3. Adjust ARIMA parameters in `*_param` variables for tuning
4. Modify forecast period by changing `steps` in `forecast()` calls

## Future Improvements
- Incorporate additional features (vaccination rates, mobility data)
- Implement more sophisticated time series models (SARIMA, Prophet)
- Add confidence intervals to forecasts
- Create interactive visualizations
- Implement automatic parameter tuning

## Data Source
[Our World in Data COVID-19 Dataset](https://github.com/owid/covid-19-data/tree/master/public/data)
