### Hospital Revenue Forecasting with SARIMA
**Tools: Python, pandas, statsmodels, scikit-learn, Matplotlib** | M.S. Data Analytics Project (D213 - Advanced Data Analytics)

Using two years of daily hospital revenue, I built a forecasting model to answer a practical planning question: what will revenue look like over the next 120 days, and how confident can we be?
 
- Converted an unlabeled day index into a proper datetime series and verified complete daily coverage with no gaps across 731 observations
- Investigated negative revenue values as possible data errors and confirmed them as legitimate loss days instead of removing them
- Diagnosed non-stationarity with an Augmented Dickey-Fuller test and identified weekly seasonality (Wednesday peaks, Friday dips) through decomposition, ACF/PACF plots, and spectral density analysis
- Moved from a standard ARIMA model, which produced a flat forecast, to a seasonal SARIMA model with a 7-day period
- Evaluated the forecast against a 120-day holdout with an MAE of $2.05M and RMSE of $2.46M, with most actual values inside the 95% confidence interval

[Documentation](https://github.com/hrbergman/postgresql-customer-services-query/blob/main/postgresql-customer-services-query/data-acquisition-documentation.pdf)
| 
[Video Presentation](https://youtu.be/jKOE0cG68rc)
