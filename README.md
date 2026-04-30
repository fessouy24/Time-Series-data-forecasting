# SMART HOME ENERGY CONSUMPTION FORECASTING

**IoT Analytics & Time Series Modeling | Phase 1: Exploration**  
**Technologies:** Python, SARIMA, Random Forest, IoT Data

---

## Overview

This repository contains Phase 1 of an IoT project focused on monitoring and forecasting energy consumption in a smart home.

Using a real-world dataset of approximately **500,000 observations** (recorded at 1-minute intervals), the project analyzes consumption patterns and compares statistical vs. machine learning approaches for **24-hour forecasting**.

---

## Project Scope

- ~350 days of energy monitoring  
- Total house energy usage (kW)  
- Individual appliance consumption  
- Localized weather conditions  

---

## 🔍 Exploratory Data Analysis

The analysis focuses on identifying intra-day volatility and seasonal cycles.

### Key Observations

- Strong **24-hour seasonal cycles**
  - Troughs at midnight
  - Peaks during active hours
- High volatility in energy consumption:
  - Range: **0.3 kW → 2.4 kW**
- Correlation between:
  - Appliance usage
  - Local weather conditions

---

## 📈 Model Comparison

| Algorithm        | MAE    | Strengths |
|-----------------|--------|----------|
| Random Forest (RF) | 0.2115 | Reacts aggressively to recent spikes; higher accuracy |
| SARIMA          | 0.3218 | Physically interpretable; stable 24-hour seasonal trends |

---

## 🛠 Technical Setup

Install required libraries:

```bash
pip install pandas numpy matplotlib statsmodels scikit-learn seaborn
```
## Data Preprocessing

- Resampling 1-minute data into hourly/daily buckets
- Handling:
  - Missing values
  - Outliers in sensor telemetry
- Feature engineering:
  - Weather lag features
  - Seasonal indices

## 👥 Team Members (Group 4)

- Mohamed Saleh
- Youssef Hesham
- Mohamed Shams
- Youssef Haitham (233579)
Mohamed Shams
Youssef Haitham (233579)
