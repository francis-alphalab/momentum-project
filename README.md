# Cross-Sectional Momentum Strategy

A momentum-based stock selection strategy tested on the full S&P 500, built in Python.

## What this project does

Each month, the strategy ranks all S&P 500 stocks by their trailing 12-month return and 
holds a basket of the strongest performers, rebalancing monthly. The goal is to test 
whether recent winners keep outperforming over the following month.

## Files

- `Cross Sectional Momentum SP 500.ipynb` — the original Jupyter notebook: data collection, 
  momentum calculation, and backtest.
- `Cross Sectional Momentum SP 500.py` — the same analysis as a plain Python script, runnable 
  cell-by-cell in Spyder.
- `momentum_dash.py` — an interactive Streamlit dashboard version showing the backtest results, 
  monthly returns, and current top-ranked holdings.

## Running the dashboard
pip install streamlit yfinance pandas numpy plotly requests
streamlit run momentum_dash.py

## Data source

Stock prices via [yfinance](https://pypi.org/project/yfinance/); S&P 500 ticker list scraped 
from Wikipedia.