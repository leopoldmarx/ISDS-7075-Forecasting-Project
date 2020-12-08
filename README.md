# ISDS 7075 Energy Forecasting Project

With the help of Trey Bickham, Michael Allen, and Rachel Parker, we placed first place in the data science project/competition for Dr. Chun's ISDS 7075 Forecasting course. This project composed of two main parts: energy backcasting 8 missing weeks in the dataset and forecasting 1 week in the future.


## Backcasting
1. Predicting load purely based on temperature of the 9 weather stations
2. Deseason residuals (yearly, weekly, then daily)
3. ARIMA from previous data for each week to forecast
4. ARIMA from future data for each week to backcast
5. Compute weighed average between each ARIMA model for each 8 week gap
6. Combine predicted errors, seasonal indexes, and predicted load from temperatures to get forecast

## Forecasting
1. Detrend/account for holidays
2. Deseason residuals (yearly, weekly, then daily)
3. ARIMA from dataset with the predicted 8 weeks to forecast the missing week
4. Combine predicted errors, seasonal indexes, and retrend model.
