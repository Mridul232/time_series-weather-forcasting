# time_series-weather-forcasting
The goal of this project is to forecast future temperature trends by applying time series forecasting methods to past temperature data. The project applies statistical models (ARIMA, SARIMA) and exploratory data analysis (moving averages, ACF/PACF diagnostics) to pattern, seasonality, and stationarity in temperature data.

This interface is a part of our project, Weather Prediction using Time Series Forecasting. The application allows users to choose a region (e.g., a country) and specify a forecast period (in days) to study past weather data and forecast future patterns. Using time series forecasting models, the project is designed to provide accurate and easy-to-understand weather information to facilitate planning and decision-making based on forecasted weather conditions.
II. Data Collection and Preprocessing 
Dataset Description
Source: GlobalWeatherRepository.csv (custom-collected or from a public weather API)
Variables Used:
•	Temporal Data: date (renamed from last_updated), temperature_celsius (primary target variable).
•	Location Metadata: country, location_name, latitude, longitude (for filtering).
Additional Available Variables (unused in current analysis but available for expansion):
•	Wind speed (wind_kph, wind_mph), humidity (humidity), precipitation (precip_mm), air quality metrics (air_quality_PM2.5, etc.). 

Preprocessing Steps
1.Column Standardization:
•	Loaded the data and processed missing values, outliers, and normalization where applicable.
•	Renamed column names to lowercase (e.g., Last_Updated → date).
•	Parsed the date column into datetime format for time series processing.
2. Filtering:
•	Filtered data by country or location_name based on user input.
3.  Handling Missing Values:
•	Dropped NaN values in rolling average calculations (SMA, EMA).
4.  Normalization:
•	Not applied in the current implementation (e.g., temperature is retained in °C).
5. Model Evaluation:
•	Tested the model’s performance using metrics such as MAE, RMSE, and MAPE.


