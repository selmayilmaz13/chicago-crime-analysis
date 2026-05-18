# DS5110 IDMP: Exploring Crime Dynamics in Chicago: Patterns, Trends, and Insights


## Overview

This project explores crime patterns in Chicago between 2019 and 2025. We look at how crimes vary over time (days, months, years), where they tend to happen in the city, and how we can forecast future crime levels using machine learning and statistical methods.

## Authors
This project was completed by Group 14

Course: DS5110 – Introduction to Data Management and Preprocessing

Team: 

[Aishwarya Umesh Honap](honap.ai@northeastern.edu )		

[Elif-Selma Yilmaz](yilmaz.el@northeastern.edu )	

[Rohit Sisir Sahoo](sahoo.ro@northeastern.edu)

## Data
The dataset is based on Chicago crime data (2019–2025).

**Download the Dataset from the API:**

[City of Chicago API URL](https://data.cityofchicago.org/resource/crimes.json?$limit=1600000&$offset=1)

OR 

**Download the data from One Drive**:

[chicago_crimes_2018_2025.csv](https://northeastern-my.sharepoint.com/:x:/g/personal/sahoo_ro_northeastern_edu/ESxGC3oVmaxKm8EOvMe68QwBsbUntDwv0q1agKqREQZQow?e=RTTHC)


## Project 
```
ds-5110-crime-dynamics-chicago/
│
├── notebooks/
│   └── DS5110_Final_Project_Chicago_Crime_Group_14.ipynb
│
├── outputs/
│   ├── analysis/
│   │   └── (all EDA/plots images)
│   ├── forecasting/
│   │   └── (SARIMAX & XGBoost plots)
│   └── clustering/
│       └── crime_hotspots_dbscan.html
│
├── README.md
├── LICENSE  (MIT)
```
---

## What We Did


### Trends & Patterns Over Time
- Analyzed **daily, monthly, and yearly crime trends** from 2019 to early 2025  
- Visualized crime distribution by **hour of day**, **day of week**, and **season**  
- Studied **arrest patterns** across years and **arrest rate** per crime type  
- Compared **domestic vs. non-domestic** crime trends over time  

### Forecasting
- Forecasted **daily crime counts for 2025** using:  
  - **SARIMAX** model for capturing seasonality and trends  
  - **XGBoost** with lag, rolling stats, and calendar features  
- Evaluated model performance using **RMSE** and plotted prediction vs. actual  

### Spatial Clustering
- Performed **DBSCAN clustering** on geolocation data (lat/lon) from 50,000 crimes  
- Tuned `eps` and `min_samples` to form ~500 meaningful clusters  
- Identified **hotspots** with their **dominant crime types**  
- Visualized hotspots using an **interactive Folium map** (saved as HTML)  

### Feature Insights
- Generated **correlation heatmaps** for crime features  
- Compared **crime density by hour** for domestic and non-domestic crimes  
- Used statistical tests (ADF) to check stationarity in time series  

---

## Key Takeaways

- Crime in Chicago follows predictable **daily and seasonal** trends  
- **Short-term fluctuations** are harder to predict, but XGBoost performed well  
- Crimes tend to **cluster in specific neighborhoods**, and certain types dominate in each area
