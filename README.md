
# Heineken Demand Forecasting & Inventory Dashboard

This project demonstrates how a Data Analyst would analyze beer demand and inventory risk using historical sales data and time-series forecasting.  
The analysis simulates real-world operations at Heineken by focusing on SKU-level performance and demand planning.

---

## Project Objective

Build a business-ready demand forecasting dashboard that:
- Visualizes historical sales trends
- Detects inventory risk (overstock / understock)
- Forecasts short-term demand
- Produces actionable business recommendations

---

## Dataset

Source: Public retail alcohol sales dataset  
Scope: Filtered to BEER category  
Granularity: Monthly  
Fields used:
- Date
- Brewery
- Product name (SKU)
- Retail sales
- Warehouse volume
- Inventory transfers

---

## Focus SKU

**HEINEKEN LOOSE NR - 12OZ**

This SKU was selected due to its:
- Consistent transactional history
- Clear business relevance
- Observable demand pattern across seasons

---

## Dashboard Features

The interactive notebook dashboard contains:

### KPI Panel
- Total retail volume
- Average monthly sales
- Warehouse volume
- Inventory transfers

### Demand Trend Chart
- Month-by-month retail sales visualization

### Forecast Panel
- 6-month demand forecast using SARIMA
- Historical vs predicted performance

### Inventory Risk Table
- Overstock risk detection
- Understock risk detection

### Executive Summary
- Automated business interpretation per SKU

---

## Forecast Results

| Month       | Forecast Units |
|--------------|----------------|
| Oct 2020     | 612            |
| Nov 2020     | 468            |
| Dec 2020     | 508            |
| Jan 2021     | 489            |
| Feb 2021     | 635            |
| Mar 2021     | 709            |

---

## Findings

- Sales peaked in 2019 and declined during 2020
- Recovery is uneven and weak
- Seasonality exists but does not drive growth
- Demand is volatile and unstable for this SKU
- Overstock risk is significant without forecast guidance

---

## Business Recommendations

- Reduce inventory exposure for this SKU
- Shift planning toward faster-moving products
- Use rolling monthly forecasts instead of quarterly averages
- Align production schedules with demand volatility

---

## Modeling Approach

The project uses **SARIMA (Seasonal ARIMA)** due to:
- Short time-series length  
- Presence of seasonal behavior  
- Need for interpretability in business context  

SARIMA performs better than machine learning when production data is limited.

---

## Tools Used

- Python
- Pandas
- Matplotlib
- Plotly
- Statsmodels
- ipywidgets

---

## Repository Contents


