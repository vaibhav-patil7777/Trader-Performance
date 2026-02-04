# Trader Performance vs Market Sentiment  


---

## Overview
The objective of this assignment is to analyze how market sentiment (Fear/Greed) relates to trader behavior and performance on Hyperliquid. Insights from this analysis can inform smarter trading strategies.

---

## Contents
- `Trader_Assignment.ipynb` : Jupyter notebook with full analysis  
- `data/` (optional) : Contains input datasets (if needed locally)  
- `charts/` (optional) : Generated visualizations for analysis  

---

## Datasets
1. **Bitcoin Market Sentiment (Fear/Greed)**  
   Columns: `timestamp`, `value`, `classification`, `date`  

2. **Historical Trader Data (Hyperliquid)**  
   Columns include:  
   `account`, `coin`, `execution_price`, `size_tokens`, `size_usd`, `side`, `timestamp_ist`, `start_position`, `direction`, `closed_pnl`, `transaction_hash`, `order_id`, `crossed`, `fee`, `trade_id`, `timestamp`  

---

## Methodology
1. **Data Preparation**  
   - Loaded both datasets and inspected for missing values and duplicates.  
   - Normalized column names and converted timestamps to datetime.  
   - Aligned both datasets by date for daily analysis.  
   - Created key metrics per trader:  
     - Daily PnL  
     - Win rate  
     - Average trade size  
     - Number of trades  
     - Long/Short ratio  

2. **Analysis**  
   - Compared performance metrics (PnL, win rate) between Fear vs Greed days.  
   - Analyzed trader behavior: trade frequency, position sizes, long/short bias.  
   - Segmented traders: high/low frequency, consistent/inconsistent winners, long/short-biased.  
   - Generated insights backed by charts and tables.  

3. **Actionable Strategies**  
   - Rule 1: Adjust trade size and frequency based on sentiment and trader behavior.  
   - Rule 2: Adjust long/short positions and leverage according to Fear/Greed and trader segment.  

---

## Key Insights
- Fear days tend to have lower PnL for infrequent traders; consistent winners maintain performance.  
- High-frequency traders increase activity during Greed days.  
- Long-biased traders perform better during Greed, short-biased during Fear.  
- Simple rules derived can guide traders on position sizing and trade frequency based on market sentiment.  

---

## How to Run
1. Clone this repository:  
```bash
git clone https://github.com/vaibhav-patil7777/Trader-Performance



