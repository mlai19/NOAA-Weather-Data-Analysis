# NOAA Weather Data Analysis

## Project Overview  
**Project Title**: Weather Data Analysis  
**Database**: jfk_weather [Kaggle]

<img width="1170" height="570" alt="image" src="https://github.com/user-attachments/assets/721f7a2c-db10-402b-b199-ebbe994fc33e" />

<br>
<br>

****Overview****
<br>
This project analyzes historical NOAA hourly weather data using Python and pandas to explore patterns, trends, and relationships across key meteorological variables. The workflow covers the full process of cleaning and preparing raw CSV files, converting timestamp fields into a usable time-series index, handling missing or inconsistent values, and transforming the dataset for deeper analysis. The goal is to strengthen data-wrangling, time-series processing, and exploratory analysis skills while uncovering meaningful insights about temperature, humidity, wind behavior, and atmospheric conditions over time.




**Project Steps**
---
**1. Data Loading** 
Before performing any analysis, the dataset is loaded into Python and inspected to understand its structure and data quality. This step includes:
- Viewing column names and data types
- Checking the number of records and memory usage
- Previewing raw weather measurements across temperature, humidity, wind, and atmospheric pressure
- Identifying inconsistent values such as "*" and missing data

**2. Data Cleaning & PreProcessing** 
Once familiar with the dataset, the next step focuses on preparing it for analysis:

- Converting the DATE column into a proper datetime format
- Setting the datetime column as the DataFrame index for time-series analysis
- Replacing invalid or placeholder values (e.g., "*") with NaN
- Ensuring numeric columns are correctly typed (float/int)
- Removing unnecessary columns and handling missing data

**3. Feature Engineering** 
To support deeper insights, additional transformations and derived features are created, including:

- Splitting complex time fields into structured datetime components if needed
- Transforming wind direction into sine/cosine values for easier modeling
- Creating new indicators for weather patterns or atmospheric trends

**4. Exploratory Data Analysis (EDA)** 
With a clean dataset, exploratory analysis is conducted to uncover trends and patterns:
- Visualizing temperature, humidity, and pressure changes over time
- Examining distributions of key variables
- Identifying seasonal or hourly patterns in the weather
- Comparing variables to detect correlations (e.g., humidity vs. temperature)

**5. Time-Series Insights & Interpretation**
Using the datetime index, time-series analysis provides additional understanding:
- Resampling data (e.g., hourly → daily averages)
- Observing long-term trends and anomalies
- Generating summary statistics for different time periods
