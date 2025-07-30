---

# Project Objective

Analyze the relationship between **market sentiment** and **trader behavior** using real-world trading data and sentiment indicators. 

We aim to:
- Understand how leverage and side (Buy/Sell) choices vary across sentiments
- Determine which sentiments yield higher profitability
- Analyze volatility patterns during different sentiment phases

---

# Data Sources

1. **Sentiment Data**

   - Source: [Alternative.me BTC Fear & Greed Index](https://alternative.me/crypto/fear-and-greed-index/)
   - Attributes: `timestamp`, `value`, `classification` (e.g. Fear, Neutral, Greed)

2. **Trader Data**
   - Source: Hyperliquid Historical Data
   - Attributes: `account`, `execution price`, `size`, `leverage (estimated)`, `PnL`, `side`, `timestamp`, etc.

---

# Key Analysis Steps

- **Data Cleaning**: Handled nulls, standardized column names, derived `estimated_leverage`, calculated daily aggregates.
- **Merging**: Synced sentiment and trade data by date.
- **EDA & Correlation Analysis**:
  - PnL vs Sentiment
  - Leverage vs Profitability
  - Side (Buy/Sell) preferences during sentiment phases
- **Volatility & Top Trader Profiling**:
  - Assessed variance in PnL
  - Visualized patterns among top-performing accounts

---

# Visualizations

- `avg_pnl_by_sentiment_side.png`: Shows which sentiment-side combinations lead to higher profits.
- `trade_volume_by_sentiment.png`: Helps assess volume distribution.
- `leverage_pnl_correlation.png`: Indicates correlation strength between leverage and closed PnL.
- `daily_volatility_boxplot.png`: Highlights risk variation during Fear vs Greed periods.

---

# Tools Used

- `Pandas`, `NumPy` – Data wrangling
- `Matplotlib`, `Seaborn` – Visualization
- `Jupyter Notebook` – Analysis Environment
- `Google Sheets` – Collaborative data cleaning

---

# Final Deliverable

- `ds_report.pdf`: Polished PDF report.
- `outputs/`: All analysis-related images and graphs.

---

# Author

**Mahek Tamboli**  
_Junior Data Scientist | Web3 Trading Team Project_  
Contact: [mahek.22311370@viit.ac.in]

---

# License

This repository is strictly for academic and internal use within the Web3 Trading Team. Not for public redistribution.

---
