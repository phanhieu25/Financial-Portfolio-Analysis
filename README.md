# Financial-Portfolio-Analysis
Financial Data Analysis &amp; Portfolio Optimization in Python. Featuring Time Series wrangling and Train/Test out-of-sample asset allocation.
# Financial Data Analysis & Portfolio Optimization

## Project Overview
This project is designed to collect, clean, and analyze Time Series data for prominent stocks using Python. Beyond price trend analysis, the project applies **Portfolio Optimization** models based on Modern Portfolio Theory (MPT) and conducts objective strategy backtesting through a rigorous Train/Test workflow.

## Analysis Objectives
- **Data Wrangling:** Processed historical data from `stock_close_prices.csv`. Thoroughly handled financial data specifics, including `DatetimeIndex` standardization, timezone synchronization (`tz_localize`, `tz_convert`), and missing value imputation (forward fill).
- **Technical Analysis:** Applied `Resampling` techniques to aggregate daily price data into larger timeframes (Weekly/Monthly) for OHLC chart visualization.
- **Asset Allocation Strategy:** Constructed an optimized investment portfolio balancing the Risk-Return Tradeoff utilizing the `PyPortfolioOpt` library.

## Technologies & Libraries
- **Language:** Python 
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`
- **Quantitative Finance:** `PyPortfolioOpt`

## Key Technical Highlights
- Successfully built an asset allocation evaluation pipeline (n-assets, k-assets) strictly adhering to Train/Test out-of-sample principles, thereby mitigating the risk of overfitting inherent in historical data analysis.
- Evaluated portfolio performance by constructing a Master Trade Log and directly comparing core financial metrics: **ROI, Sharpe Ratio, and Final Equity**.
