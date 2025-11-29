# Data Science Assignment — Web3 Trading

---
## Folder Structure

ds_ryuk/
├── notebook_1.ipynb # Google Colab notebook with analysis
├── csv_files/ # All CSV files used/generated
│ ├── fear_greed.csv # Original Fear & Greed Index dataset
│ ├── hyperliquid.csv # Original Hyperliquid trades dataset
│ ├── merged_trades_sentiment.csv # Cleaned & merged dataset
│ ├── profit_summary.csv # Average profitability by sentiment
│ ├── volume_summary.csv # Average trade size by sentiment
│ └── buy_sell_summary.csv # Profitability by trade type & sentiment
├── outputs/ # All visual outputs (charts, graphs)
│ ├── profitability_fear_greed.png
│ ├── trade_size_fear_greed.png
│ └── buy_sell_profitability.png
├── ds_report.pdf # Final report summarizing the analysis
└── README.md # This README file


---

## Project Overview

This assignment explores the relationship between **trader behavior** and **Bitcoin market sentiment** using two datasets:

- **Bitcoin Market Sentiment Dataset** — Fear & Greed Index  
- **Historical Trader Data from Hyperliquid** — account-level trades  

**Objective:** Identify patterns in **profitability, trade size, and trade direction** under different market sentiment conditions (Fear vs Greed).

---

## How to Run the Notebook

1. Open `notebook_1.ipynb` in **Google Colab**.
2. Upload all CSV files under the left panel in Colab.
3. Run the notebook step by step to replicate the analysis.
4. Processed data and visualizations will be saved in `csv_files/` and `outputs/`.

---

## Key Analysis Performed

- **Data Cleaning & Processing**
  - Converted timestamps and extracted `date_only`.
  - Merged trades with the Fear & Greed Index.
  - Handled missing sentiment values with forward/backward fill.
  - Created new numeric columns: `side_numeric`, `profit_flag`, `sentiment_numeric`.

- **Exploratory Data Analysis (EDA)**
  - Count of BUY vs SELL trades.
  - Distribution of profitable vs losing trades.
  - Trade volume analysis under Fear vs Greed.

- **Advanced Analysis**
  - Profitability under Fear vs Greed.
  - Average trade size by sentiment.
  - Profitability of BUY vs SELL trades under each sentiment.

---

## Key Insights

1. SELL trades are generally more profitable than BUY trades under both Fear and Greed.
2. Traders tend to trade **larger volumes during Fear**, indicating higher risk-taking.
3. Profitability is slightly higher during Greed, but the difference is small.
4. Monitoring the Fear & Greed Index can help optimize trade sizes and reduce risk, especially for BUY trades during Fear.

---

## References

- Historical Trader Data: `hyperliquid.csv`  
- Fear & Greed Index: `fear_greed.csv`  
- Analysis conducted using Python, **pandas**, **numpy**, **matplotlib**, and **seaborn**.
