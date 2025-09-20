# Time-Series Forecasting

## Project Overview
This project explores forecasting of time series data using both **classical statistical baselines** and **deep learning models**.  
The goal is to build, evaluate, and compare different approaches for predicting future values based on historical observations.

**Dataset:** Daily Minimum Temperatures in Melbourne, Australia (1981–1990)  
**Objective:** Predict the next day’s temperature from previous days.  

**Dataset:** Daily Minimum Temperatures in Melbourne, Australia (1981–1990)  
**Objective:** Predict the next day’s temperature based on previous days.  

---


## Methodology

1. **Data Preprocessing**
   - Load the dataset and handle missing values.
   - Normalize the data to [0,1].
   - Create sequences of length `N` for input to models.

2. **Baseline Models**
   - **Naive / Persistence model**: Predict the next value as the last observed value.
   - **Moving Average**: Predict as the average of the last N days.
   - **Linear Regression / Random Forest**: Use previous N days as features for classical ML models.

3. **Deep Learning Models**
   - **LSTM (Long Short-Term Memory)**: Captures temporal dependencies over longer sequences.

4. **Evaluation**
   - Metrics: **MAE (Mean Absolute Error)**, **RMSE (Root Mean Squared Error)**
   - Visualization: Predicted vs Actual values over time.

---

## Results

| Model              | MAE   | RMSE  |
|--------------------|-------|-------|
| Naive              | 1.95  | 2.48  |
| Moving Avg (7d)    | 2.03  | 2.58  |
| Moving Avg (30d)   | 2.05  | 2.68  |
| **LSTM**           | **1.76** | **2.25** |

✅ The LSTM model outperforms classical baselines, reducing error by ~10%.  

---

## Usage

1. Clone the repository:
```bash
git clone https://github.com/YourUsername/Time-Series-Forecasting.git
cd Time-Series-Forecasting
