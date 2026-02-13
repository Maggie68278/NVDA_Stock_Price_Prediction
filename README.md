# ARIMA Time Series Forecasting Project

---

## Project Overview

This project provides a complete **ARIMA time series modeling pipeline** for forecasting financial return of NVIDIA stock. The objective is to model stock returns using time series regression, and evaluate whether the fitted model captures underlying patterns, and generates reliable forecasts.

### The workflow includes:
EDA → Stationarity → Model Identification → Model Fitting → Diagnostics → Forecast Evaluation.

- **Descriptive visualization**
- **Stationarity testing (ADF)**
- **Train–test split (80% / 20%)**
- **Model identification (manual lag selection ACF/PACF)**
- **ARIMA model fitting (ARIMA(p,d,q))**
- **Residual diagnostics (Autocorrelation, Normality, Homoscedasticity)**
- **Forecast evaluation using MSE, MAE, and RMSE**

### Tools
- **Data**: yfinance  
- **Analysis**: pandas, numpy  
- **Modeling**: statsmodels (ARIMA), pmdarima (auto_arima)  
- **Diagnostics**: statsmodels, scipy  
- **Evaluation**: scikit-learn (MSE, MAE, RMSE)  
- **Visualization**: matplotlib  

## Results

**Model specification:** ARIMA(p, d, q) = (1, 0, 1)  

**Residual diagnostics:**  
- Shapiro-Wilk Test/ Histogram/ Q-Q plot: Residuals normally distributed
- Ljung–Box test: no autocorrelation  
- Residual ACF: no systematic spikes  

**Forecast performance:**  
- RMSE: 0.1326
- MAE: 0.1086 
- MSE: 0.0176


---

Next Steps
- Add seasonality (SARIMA)  
- Model volatility (GARCH)  
- Compare with machine learning approaches  






