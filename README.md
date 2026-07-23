# CAPM Analysis: Beta, Risk, and Expected Returns (2015-2025)

A Capital Asset Pricing Model (CAPM) analysis of 7 stocks (BA, META, MGM, NFLX, PG, T, TSLA) benchmarked against the S&P 500, using 10 years of daily price data (2015-2025).

## What's inside
- `CAPM_Project_fixed.ipynb` — full analysis notebook (data collection, EDA, beta calculation, CAPM expected returns, Security Market Line)
- `charts/` — standalone interactive HTML exports of each Plotly chart (open directly in any browser)

## Key steps
1. Pulled 10 years of daily prices via `yfinance` for 7 stocks + S&P 500 (`^GSPC`)
2. Calculated daily/annualized returns and volatility, and beta (Cov(stock, market) / Var(market)) for each stock
3. Compared beta stability across two sub-periods (2015-2019 vs 2020-2024)
4. Applied the CAPM formula — `Expected Return = Risk-Free Rate + Beta × (Market Return − Risk-Free Rate)` — using the 10-Year Treasury yield as the risk-free rate
5. Compared actual historical returns to CAPM-predicted returns to flag over/undervalued stocks
6. Plotted the Security Market Line (SML) with each stock positioned by its beta and actual return

## Live charts
Once hosted on GitHub Pages, each file in `charts/` is a fully interactive Plotly chart (zoom, hover, pan) viewable at:
- [Price Evolution](https://nsoriano18-ship-it.github.io/CAPM-Analysis/charts/01_asset_price_evolution.html)
- [COVID-19 Crash](https://nsoriano18-ship-it.github.io/CAPM-Analysis/charts/02_covid_impact.html)
- [Daily Returns Time Series](https://nsoriano18-ship-it.github.io/CAPM-Analysis/charts/03_daily_returns_timeseries.html)
- [Daily Returns Histogram](https://nsoriano18-ship-it.github.io/CAPM-Analysis/charts/04_daily_returns_histogram.html)
- [Correlation Heatmap (Prices)](https://nsoriano18-ship-it.github.io/CAPM-Analysis/charts/05_correlation_heatmap_prices.html)
- [Correlation Heatmap (Returns)](https://nsoriano18-ship-it.github.io/CAPM-Analysis/charts/06_correlation_heatmap_returns.html)
- [Security Market Line](https://nsoriano18-ship-it.github.io/CAPM-Analysis/charts/07_security_market_line.html)
