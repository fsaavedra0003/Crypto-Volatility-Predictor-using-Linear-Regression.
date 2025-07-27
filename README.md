# 📈 Bitcoin (BTC-USD) Volatility Predictor

This project uses **Linear Regression** to predict **next-day volatility** of Bitcoin (BTC-USD) based on historical prices and volume. The volatility is calculated as the **rolling 7-day standard deviation** of daily returns. 

The dataset contains **daily Bitcoin price data from 2014 to 2024**.

---

## 🧠 Objective

To build a machine learning model that can forecast the **volatility of Bitcoin** using past returns, price trends, and volume information.

---

## 📦 Dataset

**Source:** [Yahoo Finance](https://finance.yahoo.com/quote/BTC-USD/history/)

**BTC-USD Historical Price (2014 - 2024)**  
The dataset includes:

- `Date`: Date of observation  
- `Open`: Opening price  
- `High`: Highest price of the day  
- `Low`: Lowest price of the day  
- `Close`: Closing price  
- `Adj Close`: Adjusted closing price  
- `Volume`: Daily trade volume

You can access the CSV used in this project here:  
[🔗 Sample CSV File (BTCUSD)](https://www.kaggle.com/datasets/kannapat/btc-usd-historical-price-2014-2024)

---

## 🛠️ Features Used

| Feature         | Description                                    |
|----------------|------------------------------------------------|
| `Return_1d`     | 1-day lagged return                           |
| `Return_2d`     | 2-day lagged return                           |
| `MA_7`          | 7-day moving average of adjusted close price |
| `MA_14`         | 14-day moving average                         |
| `Log_Volume`    | Log-transformed volume                        |

---

## 🎯 Target Variable

- **Next-day volatility**, defined as the **standard deviation of returns over the past 7 days**, shifted forward.

---

## 📊 Model Used

- Linear Regression (`scikit-learn`)

---

## 🧪 Evaluation Metric

- **RMSE (Root Mean Squared Error)** on the test set
- **Visual plot** of predicted vs actual volatility

---

## 📉 Sample Output

![Volatility Prediction Plot](https://via.placeholder.com/800x400.png?text=Insert+your+plot+here)

---

## 🧰 Tech Stack

- Python 🐍
- Pandas & NumPy
- Scikit-learn
- Matplotlib
- Yahoo Finance (via CSV)

---

## 🚀 How to Run

1. Clone this repo
2. Install dependencies:  
   ```bash
   pip install pandas numpy scikit-learn matplotlib
