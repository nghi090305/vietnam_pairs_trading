# vietnam_pairs_trading
A backtest-ready implementation of a market-neutral pairs-trading strategy on Vietnam’s top 500 stocks from 2018 to 2025. 

This repository implements a systematic pairs-trading strategy on Vietnam’s top 500 stocks by market capitalization (2018–2025). It automates universe construction via vnstock3, fetches and aligns daily closing prices from multiple data sources, and filters symbols with ≥90% data coverage. After loading and cleaning a 90%-coverage price matrix, it splits into train and test sets (70-30), then screens for cointegrated pairs using the Engle–Granger test on log-prices. Hedge ratios are dynamically estimated via a Kalman Filter, and trading signals are generated from spread half-lives and rolling z-scores. The backtest applies realistic commissions and slippage, computes key performance metrics for each pair, and visualizes equity curves, return distributions, and rolling risk/return measures. Finally, the strategy’s average top-10 performance is benchmarked against VN-Index and VN30, with side‐by‐side cumulative returns and rolling Sharpe/volatility/drawdown plots. 










