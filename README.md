# Equity Portfolio Performance and Risk Analysis

A Python-based portfolio analytics project examining the historical performance and risk characteristics of an equally weighted portfolio of **JPMorgan Chase (JPM), Morgan Stanley (MS), and Bank of America (BAC)** against the **S&P 500 Index**.

## Research Questions

- How did the selected financial-sector portfolio perform relative to the broad equity market?
- What were its historical volatility and market sensitivity?
- How did it perform on a risk-adjusted basis?
- What were its maximum drawdown and historical tail-loss measures?

## Methodology

The notebook covers market-data retrieval with `yfinance`, simple and logarithmic returns, equal-weight portfolio aggregation, annualized return and volatility, benchmark comparison, CAPM beta and alpha, Sharpe / Sortino / Treynor / Calmar ratios, maximum drawdown, historical VaR at 90%, 95%, and 99%, and historical Expected Shortfall.

## Assets and Benchmark

| Role | Instrument | Ticker |
|---|---|---|
| Portfolio | JPMorgan Chase | JPM |
| Portfolio | Morgan Stanley | MS |
| Portfolio | Bank of America | BAC |
| Benchmark | S&P 500 Index | ^GSPC |

The notebook uses equal weights across the three constituents and a sample beginning in January 2024.

## Technology

Python · NumPy · pandas · yfinance · Matplotlib · Plotly · Jupyter Notebook

## Run

```bash
pip install numpy pandas yfinance matplotlib plotly jupyter
jupyter notebook
```

Open `Investment_Analysis_for_Equity_Portfolio.ipynb.ipynb` and run the cells. Yahoo Finance data is retrieved at runtime, so results may change as historical observations are revised.

## Interpretation and Limitations

This is a historical analysis, not a live portfolio-management system or a forecast. Results depend on the assets, sample period, benchmark, return conventions, and risk-free-rate assumption. The equal-weight portfolio should not be interpreted as evidence of persistent alpha or an investable strategy.

Further validation should include consistent date alignment, explicit missing-data treatment, transaction costs, rebalancing assumptions, and statistical inference for benchmark-relative performance.

## Disclaimer

Educational and research purposes only. Not investment advice or a recommendation to buy or sell securities.
