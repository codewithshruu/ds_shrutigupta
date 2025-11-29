Data Science Assignment — Web3 Trading
Name - Shruti Gupta
Date - 30/11/2025 


Folder Structure

ds_shrutigupta/
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


Project Overview

This assignment explores the relationship between 'trader behavior' and 'Bitcoin market sentiment' using two datasets:

1. Bitcoin Market Sentiment Dataset — Fear & Greed Index  
2. Historical Trader Data from Hyperliquid — account-level trades

The goal is to identify patterns in 'profitability, trade size, and trade direction' under different market sentiment conditions (Fear vs Greed).


How to Run the Notebook

1. Open 'notebook_1.ipynb' in Google Colab.  
2. Make sure all CSV files are uploaded in the left panel under Files.  
3. Run the notebook step by step to replicate the analysis.  
4. All visualizations and processed data will be saved in 'outputs/' and 'csv_files/' folders.


Key Analysis Performed

- Data Cleaning & Processing:
i)Timestamp conversion and extraction of 'date_only'
ii)Merging trades with Fear & Greed Index
iii)Handling missing sentiment values
iv)Creating new columns: 'side_numeric', 'profit_flag', 'sentiment_numeric'

- Exploratory Data Analysis (EDA):
  i)BUY vs SELL counts
  ii)Profitable vs losing trades
  iii)Trade volume under Fear vs Greed

- Advanced Analysis:
  i)Profitability under Fear vs Greed
  ii)Average trade size under Fear vs Greed
  iii)BUY vs SELL profitability under each sentiment

- Visualizations saved in 'outputs/' folder.


Key Insights

1. SELL trades are generally more profitable than BUY trades under both Fear and Greed.  
2. Traders trade larger volumes during Fear.  
3. Profitability is slightly higher during Greed.  
4. Monitoring Fear & Greed Index can help optimize trade sizes and reduce risk, especially for BUY trades during Fear.


References

i)Historical Trader Data: 'hyperliquid.csv'
ii)Fear & Greed Index: 'fear_greed.csv'  
iii)Analysis conducted using Python, pandas, numpy, matplotlib, and seaborn in Google Colab.

