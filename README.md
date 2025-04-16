# Gold Price Forecasting Using Macroeconomic Indicators

This project focuses on analyzing and forecasting gold prices using various global macroeconomic indicators. It involves data preprocessing, exploratory data analysis, Granger causality testing, and time series modeling using the VAR and CVAR (Johansen Cointegration) frameworks.

## Project Objectives

- Analyze the impact of global and domestic macroeconomic indicators on gold prices and Exchange rates.
- Test for Granger causality between indicators and gold price.
- Build VAR/CVAR models to forecast gold prices.
- Evaluate model performance using RMSE and MAPE.

## Dataset

The dataset includes monthly records of the following variables:

- **Gold_price(USD/Ounce)**
- **Exchange_rate(INR)**
- **Percentage Change in Gold**
- **Repo Rate (India)**
- **US Fed Rate**
- **CPI India**
- **CPI US**
- **Forex Reserves (India)**
- **Nifty 50 Index**
- **S&P 500 Index**
- **Crude Oil Price ($ per Barrel)**
- **DXY Index**
- **Trade Balance (India)**
Note: All macroeconomic indicators have been differenced or transformed as necessary to ensure stationarity for time series modeling.

## Methodology

1. **Data Preprocessing**
   - Handled missing values and ensured time alignment.
   - Applied differencing where necessary to achieve stationarity.

2. **Exploratory Data Analysis**
   - Visualized trends, seasonal components, and distributions.
   - Performed correlation analysis.

3. **Granger Causality Testing**
   - Tested whether each variable Granger-causes gold prices and Exchange rate using up to 8 lags.
   - Identified variables with significant predictive power.

4. **Model Building**
   - Built VAR and ARIMA models on differenced data.
   - Used train-test split for model validation.

5. **Model Evaluation**
   - Evaluated performance using RMSE and MAPE.
   - Compared multiple models to assess accuracy.

## Requirements

- pandas
- numpy
- matplotlib / seaborn
- statsmodels
- scikit-learn
