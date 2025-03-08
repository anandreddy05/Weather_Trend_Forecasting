## Preprocessing Steps

The following preprocessing steps were performed to clean and structure the dataset:

### Handling Missing Values

- The dataset was inspected, and no missing values were found.

- Therefore, no imputation or removal was necessary.

### Handling Duplicate Entries

No duplicate rows were found in the dataset.

### Standardizing Country Names

Some country names were present in different languages or had special characters.

- Malásia → Malaysia

- كولومبيا → Colombia

- Гватемала → Guatemala

- Польша / Polônia → Poland

- Турция / 火鸡 → Turkey

- Südkorea → South Korea

- Bélgica → Belgium

- Turkménistan → Turkmenistan

### Feature Selection

To remove unnecessary columns and keep only relevant weather-related features, we selected the following columns:

### Retained Columns:

- country, location_name, latitude, longitude, timezone

- last_updated, temperature_celsius, condition_text, wind_kph, wind_degree, wind_direction

- pressure_mb, precip_mm, humidity, cloud, feels_like_celsius, visibility_km, uv_index, gust_kph

- air_quality_Carbon_Monoxide, air_quality_Ozone, air_quality_Nitrogen_dioxide, air_quality_Sulphur_dioxide, air_quality_PM2.5, air_quality_PM10

### Saving Cleaned Data

The cleaned dataset was saved in the data folder as:

- data/cleaned_weather.csv

- This cleaned dataset will be used for Exploratory Data Analysis (EDA) and forecasting models.



# Exploratory Data Analysis (EDA)

The EDA focuses on understanding the underlying patterns in weather data using various visualizations and statistical techniques.

1. Data Cleaning & Preprocessing

- Handled missing values using imputation and forward-fill techniques.

- Scaled numerical features using MinMaxScaler/StandardScaler.

##  Key Insights from Visualizations

- Heatmap (Correlation Matrix)

- Shows strong correlations between certain weather parameters.

- Example: Temperature and humidity exhibit an inverse relationship, while temperature and pressure might be positively correlated.

## Histogram

- Reveals the distribution of variables like temperature and wind speed.

- Identifies skewness and normality of data distributions.

## Boxplot & Violin Plot

- Detects outliers in variables such as temperature and wind speed.

- Highlights extreme weather conditions and variations.

## Scatter Plot

- Visualizes relationships between variables, e.g., temperature vs. humidity.

- Helps in identifying direct and inverse correlations.

## Seasonal Decomposition

- Confirms seasonal variations in temperature and other parameters.

- Trend component showcases long-term weather patterns.

## Anomaly Detection

- Identifies unusual weather events like extreme temperature fluctuations.

- Helps in understanding and predicting extreme weather conditions.



This cleaned dataset will be used for Exploratory Data Analysis (EDA) and forecasting models.