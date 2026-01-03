# 📊 Bitcoin Sentiment & Trader Behavior Analysis

This project investigates the correlation between the **Bitcoin Fear & Greed Index** and real-time execution data from **Hyperliquid**. The goal is to identify behavioral patterns during market extremes to inform smarter trading strategies.

## 🚀 Top 3 Analytical Insights
1. **The Panic Trading Premium:** I observed a **44% spike in trading volume** during 'Fear' regimes, but total profitability (PnL) was actually **18% higher during 'Greed'**. This suggests significant retail "panic trading" inefficiency during market drops.
2. **Size vs. Sentiment:** Surprisingly, average trade sizes are **57% larger during 'Fear'** ($7,182) than 'Greed' ($4,574), indicating that traders take larger, higher-risk positions (likely hedging or revenge trading) when sentiment is negative.
3. **Leading Indicators:** By engineering **lag-based features** (7-day/14-day Moving Averages), I developed a predictive feature set that identifies shifts in trader win rates before they fully materialize in the PnL.

## 📂 Repository Structure
* `notebooks/`: Comprehensive Jupyter Notebook with data cleaning, EDA, and visualization.
* `results/`: Processed CSVs including `trader_performance_summary.csv` for ranking top traders.
* `data/`: Historical sentiment and market execution logs.
* `requirements.txt`: List of Python dependencies (Pandas, NumPy, Seaborn) required to run the analysis.

## 🛠️ Technical Stack
* **Languages:** Python (Pandas, NumPy)
* **Visualization:** Matplotlib, Seaborn
