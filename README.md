# intraday-trading-strategy
This repository contains a Python implementation of an intraday momentum strategy for the SPY ETF based on the research paper  "Beat the Market" by Zarattini, Aziz, and Barbon (2025). The primary goal of the project is to identify and capture intraday price trends by applying volatility thresholds that filter out market noise. The strategy aims to enter positions only when there is a high probability of a sustained price movement during standard market hours.

The implementation includes the integration of trailing stops that are anchored to the volume weighted average price and the use of dynamic position sizing. These additions are intended to provide a  robust defense against intraday volatility and to enhance the overall stability of the strategy. The backtesting incorporates realistic market frictions such as commissions and slippage.

Historical market data is sourced through the Alpaca API. The whole dataset contains SPY intraday market data from Jan 4, 2016 to Dec 30, 2025.

The final strategy realized a Sharpe Ratio of 1.34, 24% annualized return and 17% annualized volatility over the out-of-sample period.

### Reference
Zarattini, Carlo and Aziz, Andrew and Barbon, Andrea, Beat the Market An Effective Intraday Momentum Strategy for S&P500 ETF (SPY) (May 10, 2024). Swiss Finance Institute Research Paper No. 24-97, Available at SSRN: https://ssrn.com/abstract=4824172 or http://dx.doi.org/10.2139/ssrn.4824172
