📊 Trader Behavior vs Market Sentiment Analysis
📌 Assignment Overview

This project analyzes the relationship between trader behavior and market sentiment (Fear vs Greed) using historical cryptocurrency trading data and Bitcoin market sentiment data.
The goal is to identify how profitability, trade volume, and trading direction change under different market sentiments and to uncover insights that can support smarter trading strategies.

📂 Project Structure

The repository strictly follows the required structure:

ds_priya/
├── notebook_1.ipynb
├── csv_files/
│   ├── clean_merged_trades_sentiment.csv
│   ├── feature_engineered_trades.csv
│   └── sentiment_profitability_distribution.csv
├── outputs/
│   └── avg_pnl_by_sentiment.png
├── ds_report.pdf
└── README.md

📁 Datasets Used
1. Bitcoin Market Sentiment Dataset

Columns: Date, Classification

Classification: Fear / Greed

Used to represent daily market sentiment.

2. Historical Trader Data (Hyperliquid)

Key Columns:
Account, Coin, Execution Price, Size USD, Side, Timestamp, Closed PnL, etc.

Used to analyze trader behavior at trade level.

🛠️ Methodology

Converted timestamps and dates into proper datetime format

Merged trader data with sentiment data using the trade date

Removed duplicate and unnecessary columns

Created new features:

profit_label (Profit / Loss / Break-even)

abs_pnl (absolute profit/loss for risk magnitude)

trade_volume_usd

is_buy (Buy/Sell behavior)

Performed sentiment-wise analysis comparing Fear vs Greed

Visualized key insights and saved outputs

All analysis was done in Google Colab.

📊 Key Analysis Performed

Sentiment-wise profitability comparison

Trade volume behavior under Fear vs Greed

Buy vs Sell directional behavior

Risk magnitude analysis using absolute PnL

📈 Outputs

Cleaned and processed datasets saved in csv_files/

Visualizations saved in outputs/

Final insights documented in ds_report.pdf

🔗 Google Colab Notebook

All code and analysis are available in the Colab notebook:

Notebook: notebook_1.ipynb
(Access set to Anyone with the link can view)

📝 Conclusion

The analysis shows that market sentiment significantly influences trader behavior.
Greed periods are associated with higher trade volumes and more aggressive trading, while Fear periods reflect cautious behavior and lower profitability. These insights can help traders adapt strategies based on prevailing sentiment.

👩‍💻 Candidate

Name: Priya
Domain: Data Science
