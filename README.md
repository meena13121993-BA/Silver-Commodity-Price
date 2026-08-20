# Silver Commodity Price Forecasting & Market Intelligence Dashboard

An end-to-end data science and business intelligence solution for predicting silver spot prices, analyzing macroeconomic drivers, and backtesting trading strategies across historical economic crises.

---

## 🚀 Project Overview
Commodity markets are heavily influenced by complex macroeconomic indicators, currency fluctuations, and futures market term structures. This project combines a **Python machine learning backend** with an **interactive Power BI dashboard frontend** to deliver institutional-grade market visibility.

---

## 📊 Core Features & Architecture

### 1. Python Machine Learning Pipeline (`/scripts`)
* **Data Preprocessing & Engineering**: Cleaned multi-frequency datasets (Daily OHLCV, monthly macroeconomic metrics, and futures contract curves), handled missing values, and engineered technical indicators, moving averages, and lag features.
* **Ensemble Modeling**: Trained and evaluated machine learning models (**Random Forest** and **XGBoost**) to predict directional price movements.
* **Signal Generation**: Exported synthesized predictions (`Ensemble_Pred`) into the data pipeline for comparative visualization.

### 2. Power BI Multi-Tab Dashboard (`/dashboard`)
* **Tab 1: Executive Overview**: High-level command center tracking spot prices, daily percentage returns, volume liquidity spikes, and historical multi-decade price trajectories (2000–2025).
* **Tab 2: Macro & Futures Intelligence**: Evaluates the inverse relationship between silver and the US Dollar Index (DXY), gold-silver correlation scatter plots, and futures market term structures (Contango/Backwardation via basis calculations).
* **Tab 3: Market Sentiment & Crisis Backtesting**: Utilizes custom DAX calculated dimensions (`Crisis_Period`) to segment and stress-test market performance across major economic shocks like the **2008 Financial Crisis**, the **2011 Silver Peak**, and the **2020 COVID-19 Crash**.

---

## 🛠️ Tech Stack
* **Programming Language**: Python
* **Libraries**: Pandas, Scikit-Learn, XGBoost, NumPy
* **Business Intelligence**: Power BI (Star Schema, DAX Measures, Conditional Formatting)
* **Version Control**: Git & GitHub

---

## 📁 Repository Structure
```text
├── data/
│   ├── silver_daily_ohlcv_2000_2025.csv    # Daily spot and OHLCV market data
│   ├── silver_macroeconomic_monthly.csv    # Monthly DXY and Gold price indicators
│   └── silver_futures_contracts.csv        # Futures term structure and basis data
├── notebooks/
│   └── silver_price_forecasting.ipynb      # EDA, feature engineering, and ML model training
├── dashboard/
│   └── silver_intelligence_dashboard.pbix  # Power BI interactive report file
└── README.md
