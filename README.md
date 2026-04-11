# Stock Price Analysis & Predictive Modeling

## Overview
This project performs end-to-end **stock price analysis and forecasting** using Python and the Yahoo Finance API. It combines **exploratory data analysis, technical indicators, and predictive model based machine learning** to uncover trends, measure risk, and predict short-term price movements.

---

## Objectives
- Analyze historical stock price data  
- Identify trends, volatility, and momentum patterns  
- Apply technical indicators (RSI, MACD, Bollinger Bands)  
- Build predictive models for next-day stock prices  
- Generate automated insights for decision-making  

---

## Tech Stack
- **Programming:** Python  
- **Libraries:** Pandas, NumPy  
- **Visualization:** Matplotlib
- **Machine Learning:** Scikit-learn (Linear Regression, Random Forest)  
- **Data Source:** Yahoo Finance API (`yfinance`)  

---

## Data Source
Stock data is fetched using the **Yahoo Finance API** via the `yfinance` library.

---

## Key Features

### Exploratory Data Analysis
- Price trend visualization  
- Daily returns distribution  
- Volatility analysis  

### Technical Indicators
- Moving Averages (20-day, 50-day)  
- Relative Strength Index (RSI)  
- Moving Average Convergence Divergence (MACD)  
- Bollinger Bands  

### Risk & Performance Metrics
- Daily returns calculation  
- Volatility (standard deviation of returns)  

###  Predictive Modeling
- Target variable creation using next-day price (`shift(-1)`)  
- Time-series aware train-test split (no shuffling)  
- Linear Regression & Random Forest Regression Models for forecasting  
- Model evaluation using error metrics (RMSE, R^2)

---

## 📊 Key Insights
- Identified **trend patterns and momentum shifts** using moving averages and MACD  
- Detected **overbought and oversold conditions** through RSI analysis  
- Observed **volatility spikes during high market movement periods**  
- Built predictive models to estimate **next-day price direction**, supporting short-term trading insights  
- Random Forest Model was able to predict next day closing prices better than the linear regression model. RF had a higher R^2 value of 0.909 and a lower RSME value of 3.026 compared to linear R^2 value of 0.736 and a RMSE value of 5.244
- **Closing Price, 20-day Moving Average and Lag 1** are the top 3 features which are able to predict next day closing price.
---

## Project Structure

stock-price-analysis/
│
├── stock_analysis_notebook.ipynb
├── README.md
└── requirements.txt

---

## How to Run

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open and run the notebook in Jupyter/VS Code/Colab

---

## Future Improvements
- Implement advanced models (XGBoost, LSTM)  
- Add multi-stock comparison and portfolio analysis  
- Incorporate real-time data streaming  
- Add model explainability (feature importance, SHAP)  

---

## Business Impact
Supports **data-driven short-term trading decisions** by identifying trends, volatility, and momentum signals.

---

