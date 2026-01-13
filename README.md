# Portfolio Momentum Trading Strategy (NSE)

This project demonstrates a **momentum-based trading strategy** applied to Indian equities using Python and Yahoo Finance data. It scales the single-stock momentum logic to a **multi-asset portfolio** with monthly rebalancing.

## Strategy Overview

 Universe: HDFC Bank, Reliance, Hindustan Zinc, NIFTY 50 Index
 Momentum Window: 60 trading days
 Ranking: Assets ranked monthly based on past momentum
 Allocation: Equal weight to top assets
 Rebalancing: Monthly
 Risk Management: Look-ahead bias avoided using previous-month signals

### Key Metrics

 Metric | Value 
 Sharpe Ratio (annualized) : 0.90 
 Maximum Drawdown : -28.5% 

### Insights

Portfolio outperformed the benchmark (NIFTY 50) for most of the backtest period.
Longer momentum window + diversification improved risk-adjusted returns.
This strategy is a realistic first-step into quantitative finance, showing both **returns and risk management**.

### Libraries Used
`yfinance`
`pandas`
`numpy`
`matplotlib`

### How it Works
Download historical price data for selected NSE assets.
Calculate daily returns and 60-day momentum.
Rank assets monthly and select top performers.
Allocate capital equally among top-ranked assets.
Rebalance monthly and track cumulative portfolio returns.
Evaluate performance via Sharpe ratio and maximum drawdown.

### Plot
The portfolio performance vs. NIFTY 50 benchmark is visualized to show strategy effectiveness over time.
