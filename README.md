# 📈 Stock Trend Prediction (CNN + LSTM Hybrid Model)

## 🔹 Overview
Built a **deep learning model** to predict stock prices using a **hybrid CNN + stacked LSTM architecture** with **OHLCV features (Open, High, Low, Close, Volume)**.  
The CNN extracts short-term patterns, while LSTMs capture long-term dependencies, improving prediction accuracy compared to single models.

---

## 🔹 Tech Stack
- **Python**, **TensorFlow/Keras**  
- **Pandas, NumPy, Scikit-learn**  
- **Matplotlib** (visualization)  
- **yfinance** (data collection)

---

## 🔹 Approach
1. Fetched **Apple (AAPL)** stock data from 2015–2023 using Yahoo Finance.  
2. Preprocessed with **MinMax scaling** and created sequences of 60 timesteps.  
3. Built a **CNN + stacked LSTM hybrid model** with dropout for regularization.  
4. Trained with **Huber loss** + Adam optimizer, monitored via early stopping.  
5. Compared performance with **CNN-only** and **LSTM-only** baselines.

---

## 🔹 Results
- Achieved better accuracy than standalone CNN or LSTM.  
- Model successfully captured **stock price trends**.  

## 🔹 How to Run
```bash
git clone https://github.com/your-username/stock-trend-cnn-lstm.git
cd stock-trend-cnn-lstm
pip install -r requirements.txt
python stock_prediction.py
