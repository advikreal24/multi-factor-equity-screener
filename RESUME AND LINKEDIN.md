# Resume Description (ATS-Friendly Bullet Points)

**Institutional-Style Multi-Factor Equity Screener | Python, Pandas, NumPy, yfinance, Plotly**

- Engineered an end-to-end quantitative equity research pipeline in Python that automatically collects, cleans, and analyzes price and fundamental data for the S&P 500 using `yfinance` and web-scraped index data.
- Designed and implemented a five-factor equity ranking model (Value, Momentum, Quality, Low-Volatility, Size) using cross-sectional Z-score normalization and composite scoring across 15+ underlying financial metrics.
- Built a systematic, rules-based long-only portfolio construction module supporting equal-weight and score-weighted allocation with monthly/quarterly rebalancing simulation.
- Developed a performance analytics engine computing CAGR, Sharpe ratio, Sortino ratio, maximum drawdown, CAPM alpha/beta, and information ratio to benchmark strategy performance against the S&P 500 (SPY).
- Produced 10+ interactive Plotly and Matplotlib visualizations (factor heatmaps, correlation matrices, rolling risk/return charts, portfolio tear sheets) and an `ipywidgets`-based interactive filtering dashboard.
- Applied robust software engineering practices including modular OOP design, config-driven parameters, vectorized Pandas/NumPy computation, and defensive error handling for missing data, API rate limits, and delisted securities.

*Tailor the bullets above to the specific role — lead with the most quantitative bullet for quant research/trading roles, and the most engineering-heavy bullet for software engineering roles.*

---

# LinkedIn Project Description

🏛️ **Building an Institutional-Style Multi-Factor Equity Screener**

I built a quantitative equity research platform that screens the S&P 500 the way factor-based asset managers do — ranking every stock on five institutional factors: **Value, Momentum, Quality, Low-Volatility, and Size**.

The pipeline automatically pulls live index constituents and market/fundamental data, cleans and winsorizes the data to control outliers, standardizes every metric with cross-sectional Z-scores, and combines them into a composite ranking. From there, it constructs a rules-based long-only portfolio, rebalances it periodically, and benchmarks its risk-adjusted performance (Sharpe, Sortino, alpha, drawdown, and more) against the S&P 500.

It was a great excuse to go deep on the full quant research lifecycle: data engineering → factor construction → portfolio construction → performance attribution → visualization — the same workflow used at hedge funds and factor-based asset managers.

🔧 Built with Python, Pandas, NumPy, yfinance, and Plotly, fully documented in a Google Colab notebook.

#quantitativefinance #factorinvesting #python #portfoliomanagement #dataanalytics #fintech
