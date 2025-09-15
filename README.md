# Time-Series Forecasting

## Project Overview
This project demonstrates forecasting of time series data using both **classical baselines** and **deep learning models**. It is designed to showcase skills in **data preprocessing, sequence modeling, evaluation, and visualization**, which are highly valued in Data Science and Machine Learning internships.

**Dataset:** Daily Minimum Temperatures in Melbourne, Australia (1981–1990)  
**Objective:** Predict the next day’s temperature based on previous days.  

---

## Repository Structure


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
   - **GRU (Gated Recurrent Unit)**: Faster and simpler alternative to LSTM.

4. **Evaluation**
   - Metrics: **MAE (Mean Absolute Error)**, **RMSE (Root Mean Squared Error)**
   - Visualization: Predicted vs Actual values over time.

---

## Usage

1. Clone the repository:
```bash
git clone https://github.com/YourUsername/Time-Series-Forecasting.git
cd Time-Series-Forecasting
