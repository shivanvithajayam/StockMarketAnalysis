# Stock Market Analysis & Market Mood

A comprehensive exploratory data analysis (EDA) and performance benchmark comparing 10 major Indian equities against the NIFTY 50 index over a 1-year historical trading window.

## Project Overview

This repository analyzes daily stock delivery reports, price action, volume trends, volatility, and maximum drawdown for 10 prominent companies, evaluating how individual stock momentum correlates with market-wide trends.

### Analyzed Stocks
- **Banking & Financial Services**: HDFC Bank (`HDFCBANK`), ICICI Bank (`ICICIBANK`), State Bank of India (`SBIN`)
- **Information Technology**: Tata Consultancy Services (`TCS`), Infosys (`INFY`)
- **Oil, Gas & Energy**: Reliance Industries (`RELIANCE`)
- **Consumer Goods (FMCG)**: Hindustan Unilever (`HINDUNILVR`), ITC (`ITC`)
- **Infrastructure & Engineering**: Larsen & Toubro (`LT`)
- **Telecommunications**: Bharti Airtel (`BHARTIARTL`)
- **Market Benchmark**: NIFTY 50 Index (`nifty50.csv.csv`)

---

## Directory Structure

```text
StockMarketAnalysis/
├── data/
│   ├── raw/                  # 11 raw CSV reports (10 stocks + NIFTY 50)
│   └── cleaned/              # Standardized datasets
│       ├── all_stocks_cleaned.csv  # Combined & cleaned stock data (2,480 rows)
│       └── nifty50_cleaned.csv     # Cleaned NIFTY 50 index data (248 rows)
├── marketmood.ipynb          # End-to-end Jupyter analysis notebook
├── .gitignore
└── README.md
```

---

## Key Analysis Metrics

1. **Cumulative & Annualized Return**: Comparing 1-year performance of each stock vs NIFTY 50 benchmark.
2. **Volatility & Risk**: 20-day rolling annualized volatility and distribution analysis.
3. **Maximum Drawdown**: Downside risk assessment across peak-to-trough price movements.
4. **Volume & Delivery Analysis**: Correlation between daily trading volume, deliverable quantity %, and price action.
5. **NIFTY 50 Correlation**: Relative indexed performance (Base 100) vs broader market indices.

---

## Getting Started

### Prerequisites
- Python 3.10+
- Jupyter Notebook / JupyterLab / VS Code

### Installation
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install pandas numpy matplotlib seaborn ipykernel
```

### Running the Notebook
Open and run `marketmood.ipynb` in your preferred Jupyter environment. The notebook uses relative paths to automatically load the dataset from `data/raw/` and output results to `data/cleaned/`.
