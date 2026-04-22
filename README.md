# intraday-trading-strategy
This repository contains a Python implementation of an intraday momentum strategy for the SPY ETF based on the research paper  "Beat the Market" by Zarattini, Aziz, and Barbon (2025). The primary goal of the project is to identify and capture intraday price trends by applying volatility thresholds that filter out market noise. The strategy aims to enter positions only when there is a high probability of a sustained price movement during standard market hours.

The implementation includes the integration of trailing stops that are anchored to the volume weighted average price and the use of dynamic position sizing. These additions are intended to provide a  robust defense against intraday volatility and to enhance the overall stability of the strategy. By adjusting exposure based on real time market conditions and technical anchors, the model seeks to preserve capital while maximizing the capture of trending price action.

The general workflow is as follows: high frequency historical data is sourced through the Alpaca API to provide a reliable basis for analysis. This data is then utilized within a custom backtesting framework that incorporates realistic market frictions such as commissions and slippage to give a realistic view of the strategy's potential in a live market.


### Reference
Zarattini, Carlo and Aziz, Andrew and Barbon, Andrea, Beat the Market An Effective Intraday Momentum Strategy for S&P500 ETF (SPY) (May 10, 2024). Swiss Finance Institute Research Paper No. 24-97, Available at SSRN: https://ssrn.com/abstract=4824172 or http://dx.doi.org/10.2139/ssrn.4824172
