# 🏛️ Institutional-Style Multi-Factor Equity Screener

A production-style quantitative research platform that ranks S&P 500 equities on **Value, Momentum, Quality, Low-Volatility, and Size** factors, builds a rules-based long-only portfolio from the top decile, and benchmarks it against the S&P 500 (SPY).

Built end-to-end in a single, fully documented Google Colab notebook — no paid API keys required to run.

---

## Features

- 🔄 **Automated data collection** — live S&P 500 constituent list (Wikipedia) + historical prices & fundamentals (`yfinance`), with optional plug-ins for Financial Modeling Prep, SEC EDGAR, Alpha Vantage, and FRED.
- 🧹 **Robust data cleaning** — winsorized outlier control, missing-data handling, delisted-ticker filtering.
- 🧮 **Five-factor model** — Value (P/E, P/B, EV/EBITDA), Momentum (3/6/12M returns), Quality (ROE, margin, leverage), Low-Volatility (annualized & rolling), Size (market cap).
- 📏 **Cross-sectional Z-score normalization** and an equal-weighted composite factor score.
- 🏆 **Systematic ranking & stock selection** (configurable top-N / top-decile).
- 💼 **Portfolio construction** — equal-weight or score-weighted, with monthly/quarterly rebalancing simulation.
- 📈 **Institutional performance analytics** — CAGR, Sharpe, Sortino, Max Drawdown, Beta, Alpha, Information Ratio, Win Rate — vs. SPY.
- 📊 **11 professional visualizations** — ranking bar chart, factor heatmap, sector/ticker allocation treemap, cumulative performance, rolling return/vol, drawdown, correlation matrix, factor distributions, ranking bubble chart.
- 🎛️ **Interactive dashboard** with live sector and top-N filtering via `ipywidgets`.

## Installation

```bash
git clone https://github.com/<your-username>/multi-factor-equity-screener.git
cd multi-factor-equity-screener
pip install -r requirements.txt
```

Or simply open `multi_factor_equity_screener.ipynb` directly in **Google Colab** — the first cell installs all dependencies automatically.

## Usage

1. Open the notebook in Colab or Jupyter.
2. Edit the `CONFIG` dictionary to set universe size, lookback window, weighting scheme, and rebalance frequency (optional API keys can be added here too).
3. Run all cells top to bottom.
4. Review the auto-generated performance summary, charts, and interactive dashboard.
5. Exported files (`factor_scores.csv`, `portfolio_holdings.csv`, `performance_summary.csv`) are saved to the working directory.

## Screenshots

*(Add exported chart images here after your first run, e.g. `outputs/figures/ranking_chart.png`, `outputs/figures/tearsheet.png`)*

## Example Outputs

- `factor_scores.csv` — full ranked universe with per-factor Z-scores and composite score.
- `portfolio_holdings.csv` — selected long-portfolio holdings and weights at the latest rebalance.
- `performance_summary.csv` — side-by-side performance/risk metrics, portfolio vs. benchmark.

## Future Improvements

- Barra-style multi-factor risk model with full covariance-based risk attribution
- Sector-neutral factor scoring
- Machine-learning-based ranking (gradient boosting / learning-to-rank)
- PCA-based statistical factor discovery
- Regime detection (Hidden Markov Models) with dynamic factor tilts
- Mean-variance / CVaR portfolio optimization and risk-parity weighting
- Black-Litterman allocation blending factor views with market equilibrium
- Full backtesting engine with transaction costs, turnover constraints, and point-in-time fundamentals
- Deployment as a live Streamlit/Dash screening dashboard

## License

MIT License — free to use, modify, and distribute with attribution.
