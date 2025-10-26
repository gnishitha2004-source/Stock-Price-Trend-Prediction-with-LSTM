# Stock Price Trend Prediction with LSTM

**Author:** G. Nishitha — AIML Intern  
**Run Environment:** Google Colab / Python 3.x  

---

## Project Overview

This project predicts future stock prices using a **Long Short-Term Memory (LSTM)** neural network. Historical stock data is fetched via **yfinance**, preprocessed, and used to train an LSTM model. Predictions are visualized and compared to actual stock prices.

The project also includes a **Streamlit app** to interactively predict the next closing price for any stock ticker.

---

## Project Features

- Download historical stock data using `yfinance`.
- Preprocess data with **MinMaxScaler** for scaling.
- Create sequences of 60 days of past data to predict the next day's closing price.
- Build an LSTM model with two LSTM layers and Dropout to avoid overfitting.
- Train the model and monitor performance using validation loss.
- Evaluate performance using **MAE** (Mean Absolute Error) and **RMSE** (Root Mean Squared Error).
- Save the trained model and scaler for future predictions.
- Streamlit app for easy, interactive predictions.
- Save **predicted vs actual results** as CSV for analysis.

---

## Project Files

| File | Description |
|------|-------------|
| `Stock_Price_Trend_Prediction_with_LSTM.ipynb` | Main Colab notebook with code and explanations |
| `G_Nishitha_Stock_Price_Trendiction_Report.pdf` | Project report / summary |
| `stock_data.csv` | Downloaded historical stock data |
| `predicted_vs_actual.csv` | Model predictions vs actual prices |
| `lstm_stock_model.h5` | Trained LSTM model |
| `scaler.save` | Scaler object for inverse transformation |
| `app.py` | Streamlit app for interactive predictions |
| `README.md` | Project description and instructions |

---

## How to Run

### 1. Run the Notebook
1. Open `Stock_Price_Trend_Prediction_with_LSTM.ipynb` in Colab.
2. Install required packages (yfinance, tensorflow, pandas, matplotlib, scikit-learn, joblib).
3. Run all cells sequentially to download data, train the model, and visualize results.

### 2. Run Streamlit App (Optional)
```bash
streamlit run app.py
