# Time Series Analysis of CO2 Flux Data

This repository contains two Jupyter notebooks that analyze CO2 flux data collected at the Veenkampen measurement station between 2015 and 2023. Each notebook uses a different modeling approach: SARIMAX and Random Forest Regression.

## Dataset Overview

The analysis is based on four main datasets:

1. **Air Quality Data**  
   Includes measurements such as CO2 mixing ratio, H2O mixing ratio, black carbon (BC), NOx, NO, NO2, O3, PM10, and PM2.5

2. **Meteorological Data**  
   Contains temperature (TA), relative humidity (RH), shortwave and longwave radiation (SW_IN, SW_OUT, LW_IN, LW_OUT), visibility (VIS), wind speed (WS), wind direction (WD), and pressure (P)

3. **Soil Data**  
   Contains measurements relevant to soil conditions and moisture

4. **Flux Data**  
   Provides CO2 flux values, which serve as the prediction target

## Notebooks

### SARIMAX_polished.ipynb

This notebook applies a SARIMAX (Seasonal AutoRegressive Integrated Moving Average with eXogenous variables) model to forecast CO2 flux values using seasonal trends and external input variables.

### RandomForest_polished.ipynb

This notebook uses a Random Forest regression model to predict CO2 flux values based on engineered features from the air quality, meteorological, and soil datasets.

## Data Processing

Both notebooks perform:
- Data cleaning
- Handling of missing values
- Outlier detection and removal
- Time series alignment
- Feature engineering

## Requirements

All required Python packages are listed in the `requirements.txt` file. Install them with:

```bash
pip install -r requirements.txt