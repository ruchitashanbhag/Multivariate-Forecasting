# Multivariate-Forecasting
Solar PV Power Forecasting uses predictive analysis to calculate total power required for week/month ahead forecasting for a 15-minute interval using seasonal ARIMA (Time Series Model) and exogenous regressors.

Grid search/Hyperparameter optimization to evaluate different combinations of parameters.
For each combination of parameters, a new seasonal ARIMA model is fit with the SARIMAX() function from the statsmodels module in Python and assess its overall quality.

AIC (Akaike Information Criterion) value, which is also returned with ARIMA models is used to check how well a model fits the data along with the least AIC score.
The smallest AIC is 16325.808916722315 for model SARIMAX with the best parameters: (3, 0, 1)x(3, 1, 1, 12).
The final MAPE (Mean Absolute Percentage Error) value obtained for the model was 8.7%.

Dataset used is from the Solar Power Plants in Bhadla, Gujarat.
