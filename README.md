# Commodity Market Analysis & Trading Strategy Backtest

## Overview
A quantitative research project analyzing historical gold and crude oil futures price series, comparing their risk-return characteristics, and evaluating a simple moving-average trading strategy against a buy-and-hold benchmark.

## Objectives
- Compare historical price performance and risk across two commodities.
- Calculate annualized returns, volatility and maximum drawdown.
- Implement a 20-day/50-day moving-average crossover strategy.
- Evaluate strategy performance after an assumed transaction cost.
- Investigate whether results are consistent across different periods.

## Tools
Python, pandas, NumPy, matplotlib, yfinance and Google Colab.

## Methodology
1. Retrieved historical daily price data for gold (`GC=F`) and crude oil (`CL=F`).
2. Calculated daily percentage returns and descriptive risk metrics.
3. Implemented a long-or-cash moving-average crossover strategy on crude oil.
4. Compared the strategy with buy-and-hold using cumulative returns, volatility, maximum drawdown and the Sharpe ratio.
5. Examined performance across the first and second halves of the sample.

## Key Findings
- Gold showed higher annualized price appreciation and lower realized volatility than crude oil in the observed sample.
- The moving-average strategy returned 53.29% cumulatively, compared with 16.25% for buy-and-hold under the implemented assumptions.
- Strategy annualized volatility was 31.17%, compared with 41.60% for buy-and-hold.
- Maximum drawdown remained substantial at -52.09%.
- Performance was uneven: the strategy returned -9.52% in the first half and +69.42% in the second half, indicating potential sensitivity to market regimes.

## Limitations
The analysis uses continuous-futures price series, which do not necessarily represent executable contract-level returns. Transaction costs are simplified, and the backtest does not fully model contract rolls, slippage, margin or market impact. The strategy has not been established as robust through comprehensive out-of-sample testing.

## Reproducibility
The analysis and visualizations are contained in the accompanying Jupyter notebook. Run the notebook from top to bottom in Google Colab or a compatible Python environment.

## Disclaimer
This project is for educational and research purposes only. Historical results do not guarantee future performance and should not be interpreted as investment advice.
