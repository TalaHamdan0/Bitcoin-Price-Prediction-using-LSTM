# Bitcoin-Price-Prediction-using-LSTM
# Bitcoin Price Prediction using LSTM

## 📌 Overview

This project uses an LSTM (Long Short-Term Memory) neural network to predict the future price of Bitcoin (BTC-USD) based on its historical daily closing prices. LSTM models are ideal for time‑series forecasting because they can capture long‑term dependencies and trends.

---

## 🚀 Objectives

* Build a deep learning model using LSTM to understand Bitcoin price movements.
* Compare **actual vs predicted** prices.
* Forecast the **next 30 days** of Bitcoin prices.
* Visualize results clearly for analysis.

---

## 🗂 Dataset

The data was collected using the **yfinance** API:

* Symbol: `BTC-USD`
* Date range: 2023-01-01 → 2025-11-27
* Interval: 1 day

Stored locally as:

```
BTC-USD_historical.csv
```

---

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* TensorFlow / Keras
* Matplotlib
* scikit‑learn (MinMaxScaler)
* yfinance

---

## 🧹 Data Preprocessing

1. Load Bitcoin closing prices.
2. Apply MinMaxScaler normalization.
3. Create sequences of 60 days → predict day 61.
4. Split into training and testing sets.

---

## 🧠 LSTM Model Architecture

* 3 stacked LSTM layers (50 units each)
* Dropout (0.2) to reduce overfitting
* Dense output layer predicting 1 value
* Optimizer: Adam
* Loss: Mean Squared Error

---

## 📈 Results

### 🔹 Actual vs Predicted Price

Model predictions were plotted against real Bitcoin prices to evaluate accuracy.

### 🔹 30‑Day Future Forecast

The model predicts Bitcoin's trend for the next 30 days based on the last 60 days of input data.

> 💡 *Add your plots here:*
> `images/actual_vs_predicted.png`
> `images/forecast_30_days.png`

---

## 📊 Visualizations

* Price history
* Predicted vs actual comparison
* Future price forecast curve

---

## 🧪 Evaluation Metrics (Optional)

You can calculate additional metrics:

* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)

---

## 📦 How to Run the Project

1. Install requirements:

```
pip install pandas numpy matplotlib tensorflow scikit-learn yfinance
```

2. Run the notebook or script.
3. Make sure `BTC-USD_historical.csv` is in the same directory.

---

## 💡 Future Improvements

* Use GRU or Bidirectional LSTM
* Try multivariate forecasting (Open, High, Low, Volume)
* Deploy as a web app using Flask or Streamlit

---

## 👤 Author

**Tala Hamdan**

A passionate learner exploring Data Science, Machine Learning, and time‑series forecasting.

---

## ⭐ Give the repo a star if you like the project!
