# PM2.5 Air Quality Analysis and Forecasting in Dhaka

## Project Overview

Air pollution is a major environmental and public health challenge in Dhaka, Bangladesh. This project analyzes PM2.5 concentration data and investigates its relationship with meteorological variables such as temperature, precipitation, and wind speed.

The study also applies time-series forecasting techniques to predict future PM2.5 levels and evaluate potential health risks.

---

## Objectives

- Analyze PM2.5 concentration patterns.
- Handle missing observations using interpolation/Kalman filtering.
- Explore relationships between air quality and weather variables.
- Visualize seasonal and monthly trends.
- Forecast future PM2.5 concentrations using AutoRegressive (AR) models.
- Assess public health risk categories based on PM2.5 levels.

---

## Dataset

The dataset contains:

| Variable | Description |
|-----------|-------------|
| date | Observation date |
| pm25 | PM2.5 concentration (μg/m³) |
| temp_max | Maximum temperature |
| temp_min | Minimum temperature |
| temp_mean | Mean temperature |
| precipitation | Daily precipitation |
| wind_speed | Daily wind speed |

Source:
- US Embassy/Consulate Air Quality Monitoring Data
- Meteorological observations

---

## Methodology

### Step 1: Data Preprocessing

- Load dataset
- Convert date variables
- Handle missing values
- Create cleaned PM2.5 series

### Step 2: Exploratory Data Analysis

- Distribution analysis
- Box plots
- Trend visualization
- Monthly patterns

### Step 3: Missing Data Imputation

Missing PM2.5 observations are filled using interpolation techniques.

### Step 4: Rolling Average Analysis

Calculate:

- 7-day moving average
- 30-day moving average

to identify long-term trends.

### Step 5: Time Series Forecasting

An AutoRegressive (AR) model is fitted to the PM2.5 series.

Forecasting workflow:

1. Split data into training and testing sets.
2. Fit AR model.
3. Generate forecasts.
4. Compare actual and predicted values.

### Step 6: Diagnostic Testing

Model residuals are examined using:

- ACF plots
- PACF plots
- Q-Q plots

### Step 7: Health Risk Assessment

PM2.5 levels are categorized according to air quality health standards:

- Good
- Moderate
- Unhealthy for Sensitive Groups
- Unhealthy
- Very Unhealthy
- Hazardous

---

## Generated Figures

### Figure 1
Box plots of PM2.5 and meteorological variables.

### Figure 2
Missing-value imputation visualization.

### Figure 3
7-day and 30-day rolling averages.

### Figure 4
Model performance comparison.

### Figure 5
AR model forecasting results.

### Figure 6
ACF and PACF diagnostic plots.

### Figure 7
Q-Q plot of residuals.

### Figure 8
Health-risk time series visualization.

### Figure 9
Monthly PM2.5 heatmap.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/PM25-Air-Quality-Forecasting.git
