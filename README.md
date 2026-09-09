# 📈 Indian Stock Market Analysis

**End-to-end backtesting and investment strategy analysis on the Nifty-50 using Python**, covering **Buy & Hold, MA-20, MA-50, RSI, and SIP strategies** with performance evaluation using **Total Return, CAGR/XIRR, and Maximum Drawdown**.

---

## 📌 Project Overview

This project analyzes **10+ years of historical Nifty-50 (`^NSEI`) data from 2015–2026** to evaluate and compare five different investment strategies.

The analysis progresses from a simple **Buy & Hold benchmark** to rule-based technical strategies using **Moving Averages and RSI**, along with a **Systematic Investment Plan (SIP)** approach.

The objective is to understand how different investment approaches perform in terms of **annualized returns and downside risk**, while demonstrating practical skills in **data analysis, financial modeling, and strategy backtesting**.

> **Note:** Results are based on historical data and the assumptions defined in the notebook. They are intended for analytical and educational purposes and do not represent investment advice.

---

## 🗃️ Data Source

| Source       | Description                                                  |
| ------------ | ------------------------------------------------------------ |
| **yfinance** | Historical daily OHLC data for Nifty-50 (`^NSEI`), 2015–2026 |

---

## 🛠️ Tools & Technologies

| Tool / Library                | Purpose                                              |
| ----------------------------- | ---------------------------------------------------- |
| **Python / Jupyter Notebook** | Data analysis, strategy implementation & backtesting |
| **pandas**                    | Data manipulation and analysis                       |
| **NumPy**                     | Numerical calculations                               |
| **yfinance**                  | Historical market data                               |
| **Matplotlib**                | Data visualization                                   |
| **Seaborn**                   | Statistical visualization                            |
| **Plotly**                    | Interactive visualization                            |
| **SciPy (`brentq`)**          | XIRR calculation using numerical root-finding        |

---

# 📊 Strategies Analyzed

## 🟢 1. Buy & Hold Strategy

₹1 Lakh is invested in the Nifty-50 at the beginning of the analysis period and held throughout.

This serves as the **baseline benchmark** against which all other strategies are evaluated.

**Metrics:** Total Return · CAGR · Maximum Drawdown

<img width="462" height="65" alt="Image" src="https://github.com/user-attachments/assets/f6bb1979-1501-4594-84df-6e52007ca443" />

---

## 🟡 2. MA-20 Strategy

A **20-day Moving Average crossover strategy** that generates buy and sell signals based on price crossing the MA-20.

**Metrics:** Total Return · CAGR · Maximum Drawdown

<img width="270" height="65" alt="Image" src="https://github.com/user-attachments/assets/49a2c23e-5f37-4ce2-a0f5-bf77c32b15d8" />

---

## 🟡 3. MA-50 Strategy

A **50-day Moving Average crossover strategy** using the same methodology as MA-20, with a longer lookback period.

This allows comparison between **shorter-term and longer-term trend signals**.

**Metrics:** Total Return · CAGR · Maximum Drawdown

<img width="241" height="62" alt="Image" src="https://github.com/user-attachments/assets/a81ff0d6-1385-4dbd-a517-cd7af42ec4be" />

---

## 🔴 4. RSI Strategy

A rule-based strategy using the **Relative Strength Index (RSI)** to generate entry and exit signals.

* **Buy:** RSI crosses above 20
* **Sell:** RSI crosses above 80

**Metrics:** Total Return · CAGR · Maximum Drawdown

<img width="415" height="67" alt="Image" src="https://github.com/user-attachments/assets/e158145e-4adf-4757-99d1-70bc47e0821b" />

---

## 🔵 5. SIP Investing

A **Systematic Investment Plan (SIP)** simulation where a fixed amount is invested on the first trading day of each month.

Because SIP involves **multiple cash flows occurring on different dates**, **XIRR** is used as the annualized return measure instead of CAGR.

**Metrics:** Total Return · XIRR · Maximum Drawdown

<img width="338" height="65" alt="Image" src="https://github.com/user-attachments/assets/73b20acf-cd1d-4eef-8438-632b4bccf7d2" />

---

# 📈 Nifty-50 Market Overview

The project begins by analyzing the historical price movement of the Nifty-50 over the study period.

<img width="1282" height="587" alt="Image" src="https://github.com/user-attachments/assets/3f7e4907-53f9-4036-8512-8bbeb296213c" />

---

# 📊 Strategy Comparison

The five strategies are compared using their respective **annualized return measure (CAGR/XIRR)** and **Maximum Drawdown** to evaluate the relationship between returns and downside risk.

### Risk vs. Return

<img width="1350" height="563" alt="Image" src="https://github.com/user-attachments/assets/0ffe5296-f690-4e73-9c9d-f6fa0b4823d2" />

---

# 🔑 Key Insights

* **SIP** provides the strongest balance between annualized return and downside risk among the strategies tested.
* **MA-20 and MA-50** reduce drawdown compared with Buy & Hold, although this comes with lower annualized returns.
* **MA-50 slightly outperforms MA-20**, suggesting that the longer lookback period performed better during this particular backtest.
* **RSI** underperforms the other strategies in this implementation, producing a negative annualized return and the highest drawdown.
* **Buy & Hold** delivers the highest nominal total return but also experiences the deepest drawdown.

### 💡 Key Takeaway

> **Within this backtest period, SIP provides the strongest balance between annualized return and downside risk among the five strategies tested.**

These results are specific to the selected **time period, strategy rules, investment assumptions, and market conditions** and should not be interpreted as a guarantee of future performance.

---

# 📐 Performance Metrics

### Total Return

Measures the overall percentage gain or loss over the investment period.

### CAGR

Measures the annualized growth rate for strategies involving an initial lump-sum investment.

### XIRR

Measures the annualized return for investments involving multiple cash flows occurring on different dates, making it appropriate for the SIP analysis.

### Maximum Drawdown

Measures the largest decline in portfolio value from a previous peak and provides an indication of historical downside risk.

---

# 📂 Repository Structure

```text
Indian-Stock-Market-Analysis/
│
├── 📓 Indian_Stock_Market_Analysis.ipynb
├── 📄 README.md
│
└── 📁 images/
    ├── MA_20_Chart.png
    ├── MA_20_Performance_Metrics.png
    ├── MA_20_Portfolio_Growth.png
    ├── MA_50_Chart.png
    ├── MA_50_Performance_Metrics.png
    ├── MA_50_Portfolio_Growth.png
    ├── Nifty_50_over_time.png
    ├── Nifty_50_Performance_Metrics.png
    ├── Risk_vs_Reward__Strategies_.png
    ├── RSI_Chart.png
    ├── RSI_Performance_Metrics.png
    ├── RSI_Portfolio_Growth.png
    ├── SIP_Performance_Metrics.png
    └── SIP_Portfolio.png
```

---

# 🎯 Project Highlights

* Analyzed **10+ years of Nifty-50 historical data**
* Backtested **5 investment strategies**
* Implemented rule-based **Moving Average and RSI signals**
* Simulated **monthly SIP investing**
* Calculated **CAGR and XIRR**
* Evaluated **Maximum Drawdown**
* Compared strategies based on **return and downside risk**
* Built financial performance visualizations using Python
* Applied data cleaning, analysis, modeling, and visualization techniques

---

# 📓 Notebook

The complete analysis, including **data preparation, strategy logic, backtesting, performance calculations, and visualizations**, is available in:

`Indian_Stock_Market_Analysis.ipynb`

---

# 📬 Contact

**Rohit Singh Bisht**

🔗 GitHub: **RohitBishtDA**
