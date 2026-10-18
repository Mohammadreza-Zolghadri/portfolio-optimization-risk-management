# Portfolio Optimization and Risk Management

A quantitative finance project implementing Modern Portfolio Theory (Markowitz Mean-Variance Optimization), Monte Carlo simulation, Sharpe ratio maximization, and downside risk analysis using Python.

## Overview
This project constructs an optimal investment portfolio using major U.S. equities (Apple, Microsoft, JPMorgan Chase) and the S&P 500 benchmark index (`^GSPC`) covering the period from January 2019 to January 2024.

## Key Features
- **Data Pipeline:** Automated retrieval, local caching, and processing of adjusted close prices using `yfinance`.
- **Return & Risk Statistics:** Computation of annualized mean returns and annual covariance matrix (assuming 252 trading days).
- **Monte Carlo Simulation:** Simulated 10,000 random portfolio allocations to map the Efficient Frontier.
- **Sharpe Ratio Maximization:** Derived the optimal asset weights for the portfolio maximizing risk-adjusted return.
- **Downside Risk Metrics:** Evaluated historical Daily Value at Risk (VaR at 95% confidence) and Maximum Drawdown (MDD).

## Summary Results & Optimal Weights (2019–2024)

### Optimal Portfolio Weights (Max Sharpe Ratio)
| Asset | Optimal Weight |
| :--- | :---: |
| **AAPL** | 74.08% |
| **MSFT** | 24.32% |
| **JPM** | 1.38% |
| **^GSPC** | 0.22% |

### Performance & Risk Metrics
- **Expected Annual Return:** 36.09%
- **Expected Annual Volatility (Risk):** 30.15%
- **Sharpe Ratio:** 1.1970
- **Daily Value at Risk (VaR 95%):** -2.85%
- **Maximum Drawdown (MDD):** -30.83%

## Project Structure
- `portfolio_optimization.ipynb`: Complete Jupyter Notebook containing data ingestion, return calculations, Monte Carlo optimization, Efficient Frontier visualization, and risk assessment.
- `portfolio_prices.csv`: Locally cached historical adjusted closing prices.

## How to Run
1. Clone this repository:
```bash
   git clone https://github.com/Mohammadreza-Zolghadri/portfolio-optimization-risk-management.git
   
