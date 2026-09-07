📈 Indian Stock Market Analysis

End-to-end backtesting and strategy comparison on the Nifty-50 index using Python — covering Buy & Hold, Moving Average, RSI, and SIP strategies, with CAGR, XIRR, and Drawdown analysis.

📌 Project Overview

This project analyzes 10+ years of Nifty-50 (^NSEI) data (2015–2026) using Python, comparing five different investment strategies to see which delivers the best risk-adjusted returns. The analysis progresses from a simple buy-and-hold benchmark to rule-based technical strategies (Moving Averages, RSI) and disciplined SIP investing — designed to demonstrate applied data analysis and financial modeling relevant to Data Analyst / Quant roles.

🗃️ Data Source
Source	Description
yfinance	Historical daily OHLC data for ^NSEI (Nifty-50), 2015–2026
🛠️ Tools Used
Tool	Purpose
Python (Jupyter Notebook)	Data cleaning, strategy logic, backtesting
pandas, numpy	Data manipulation & calculations
yfinance	Fetching historical Nifty-50 data
matplotlib, seaborn, plotly	Visualization
scipy (brentq)	XIRR calculation via root-finding
📊 Strategies Analyzed
🟢 1. Buy & Hold Strategy

₹1 Lakh invested in Nifty-50 at the start and held throughout the full period — the baseline every other strategy is measured against.

Metrics: Total Return · CAGR · Max Drawdown

Portfolio Growth

Show Image

🟡 2. MA-20 Strategy

A moving-average crossover strategy using a 20-day window to generate buy/sell signals.

Metrics: CAGR · Max Drawdown · Total Return

🟡 3. MA-50 Strategy

Same crossover logic using a longer 50-day window, to compare sensitivity vs. the MA-20 approach.

Metrics: CAGR · Max Drawdown · Total Return

🔴 4. RSI Strategy

Buy/sell signals generated using the Relative Strength Index (RSI) to time entries and exits based on overbought/oversold conditions.

Metrics: CAGR · Max Drawdown · Total Return

🔵 5. SIP Investing

Simulates a Systematic Investment Plan — a fixed amount invested on one day each month, evaluated using XIRR (since cash flows are staggered, not lump-sum).

Metrics: XIRR · Max Drawdown · Total Return

📊 Strategy Comparison

All five strategies are benchmarked side-by-side on annualized return vs. downside risk.

Risk vs Reward — CAGR/XIRR vs Max Drawdown

Show Image

💡 Key Insights

(Fill in with your actual results once finalized — example format below)

💰 [Strategy] delivered the highest CAGR/XIRR among all approaches
📉 [Strategy] had the lowest max drawdown, making it the safest on a risk-adjusted basis
🔄 SIP investing smoothed out volatility compared to lump-sum strategies
📈 Technical strategies (MA/RSI) [beat / underperformed] Buy & Hold after accounting for drawdown
📂 Repository Structure


   jupyter notebook Indian_Stock_Market_Analysis.ipynb

📬 Contact

Author: Rohit Singh Bisht   GitHub: RohitBishtDA
