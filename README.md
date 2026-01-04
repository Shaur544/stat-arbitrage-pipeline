# Statistical Arbitrage Research Pipeline

A research-grade statistical arbitrage pipeline built from scratch using Python.  
The project focuses on **mean-reversion strategies**, **rolling hedge ratios**, and **stationarity validation**, following industry-standard quant research practices.

---

## 📌 Project Overview

This project implements an end-to-end **statistical arbitrage (pairs trading)** workflow:

- Raw market data ingestion
- Feature construction using returns
- Asset relationship analysis
- Hedge ratio estimation via regression
- Mean-reversion validation using ADF tests
- Trading signal generation
- Backtesting and performance evaluation

The goal is not prediction, but **relative value trading** based on statistical structure.

---

## 🧠 Key Concepts Used

- Log returns & simple returns
- Rolling correlation
- OLS regression (hedge ratio estimation)
- Rolling hedge ratios (adaptive parameters)
- Beta-hedged spreads
- Stationarity testing (ADF)
- Z-score normalization
- Rule-based trading signals
- Backtesting (PnL, drawdown, Sharpe)

---

## 🏗️ Pipeline Structure

### Phase 1: Data Ingestion & Cleaning
- Downloaded equity data using Yahoo Finance
- Handled MultiIndex price structures
- Extracted Close prices
- Enforced datetime indexing
- Removed missing data
- Performed sanity checks

### Phase 2: Feature Engineering
- Computed simple and log returns
- Ensured proper time alignment
- Visualized return behavior

### Phase 3: Relationship Modeling
- Rolling correlation analysis
- Static hedge ratio estimation (OLS)
- Construction of log-price spreads

### Phase 4: Mean-Reversion Validation
- Augmented Dickey-Fuller (ADF) test
- Identified weak global stationarity
- Introduced rolling hedge ratios
- Constructed rolling beta-hedged spreads
- Re-tested stationarity

### Phase 5: Trading Strategy
- Z-score normalization of spread
- Entry/exit signal generation
- Long/short position logic
- Market-neutral exposure

### Phase 6: Backtesting & Evaluation
- Strategy return computation
- Cumulative returns
- Drawdown analysis
- Sharpe ratio calculation

---

## 📊 Results

- Demonstrates realistic behavior of financial time series
- Shows why many pairs fail stationarity tests
- Highlights importance of rolling parameters
- Produces a complete research-grade backtest

---

## ⚠️ Notes

- This is a **research project**, not production trading code
- Transaction costs and slippage are not modeled
- Strategy performance is illustrative, not investment advice

---

## 🛠️ Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- Statsmodels
- yFinance
- Jupyter Notebook

---

## 🚀 Future Improvements

- Transaction cost modeling
- Multi-pair portfolio construction
- Parameter sensitivity analysis
- Modular codebase refactor
- Walk-forward validation

---

## 👤 Author

Shaurya Singh  
MS CS (AI) Incoming – NYU  
Interested in Quantitative Research, Quant Dev, and Applied ML

---

## 📎 Disclaimer

This project is for educational and research purposes only.  
Not financial advice.
