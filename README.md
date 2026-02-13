**ARIMA Time Series Forecasting Project**

---

**Project Overview**

This project provides a complete **ARIMA time series modeling pipeline** for forecasting financial return of NVIDIA stock. The objective is to model stock returns using time series regression, and evaluate whether the fitted model captures underlying patterns, and generates reliable forecasts.

The workflow includes:

- **Descriptive visualization**
- **Stationarity testing (ADF)**
- **Train–test split (80% / 20%)**
- **Model identification (ACF/PACF)**
- **ARIMA model fitting**
- **Residual diagnostics**
- **Forecast evaluation using MSE, MAE, and RMSE**

Tools
- **Data**: yfinance  
- **Analysis**: pandas, numpy  
- **Modeling**: statsmodels (ARIMA), pmdarima (auto_arima)  
- **Diagnostics**: statsmodels, scipy  
- **Evaluation**: scikit-learn (MSE, MAE, RMSE)  
- **Visualization**: matplotlib  

---

Next Steps
- Add seasonality (SARIMA)  
- Model volatility (GARCH)  
- Compare with machine learning approaches  






