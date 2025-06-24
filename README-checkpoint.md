# 🧠 Trader Performance & Sentiment Analysis

This project explores the relationship between crypto trader performance and market sentiment using historical trading data and the Bitcoin Fear & Greed Index. The objective is to uncover actionable insights and build a machine learning model to predict trader profit/loss (`Closed PnL`).

---

## 📂 Project Structure

├── data/
│ ├── historical_data.csv
│ ├── fear_greed_index.csv
│ └── merged_data.csv
├── notebooks/
│ ├── data_cleaning_merge.ipynb
│ ├── eda_visualization.ipynb
│ └── model_training.ipynb
├── Final_Trader_Performance_With_Plots.pptx
├── README.md
└── requirements.txt

---

## 📊 Data Description

- **historical_data.csv**: Trade-level data (account, coin, execution price, side, size, etc.)
- **fear_greed_index.csv**: Daily sentiment scores and classifications (e.g. Fear, Greed)
- **merged_data.csv**: Combined data on a per-day basis for analysis

---

## 🧪 Notebooks Overview

- `data_cleaning_merge.ipynb`: Preprocess, clean, and merge datasets
- `eda_visualization.ipynb`: In-depth EDA using visualizations and sentiment impact analysis
- `model_training.ipynb`: Train and evaluate a regression model to predict Closed PnL

---

## 🎯 Key Insights

- Trader profits are higher during **Extreme Greed** sentiment periods
- Market sentiment has measurable influence on trading behavior
- Random Forest model trained to predict `Closed PnL` with sentiment + trade features

---

## 🤖 Model Performance

- **Model**: RandomForestRegressor
- **Target**: `Closed PnL`
- **Features**: execution_price, size_usd, side, direction, sentiment
- **R² Score**: ~0.16 (initial baseline model)

---

## 🛤️ Next Steps

- Add technical indicators (MACD, RSI)
- Deploy model with Streamlit dashboard
- Try boosting models (XGBoost, LightGBM)

---

## 🧰 Setup Instructions

1. Clone this repo
2. Install requirements:
```bash
pip install -r requirements.txt




