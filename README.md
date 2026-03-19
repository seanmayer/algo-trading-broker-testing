# OANDA Algo Trading Basics

Educational project for learning market data analysis and algorithmic trading workflows with:
- `pandas`-based financial analysis notebooks
- broker-focused examples for OANDA and Interactive Brokers (IBKR)

This repository is structured as a learning workspace, not a production trading system.

## What Changed
The project now includes a substantially expanded notebook curriculum under `pandas-financial-data-analysis/`, including topics like:
- return frameworks (simple, log, compound)
- annualization and rolling statistics
- covariance/correlation and diversification
- short-selling intuition and coding challenges
- leverage, margin trading, and path-dependent risk

## Project Structure

```text
oanda-algo-trading-basics/
├── pandas-financial-data-analysis/   # Main financial analytics notebook track (0..23)
├── pandas-timeseries-data/           # Pandas time-series fundamentals
├── brokers/
│   ├── oanda/                        # OANDA examples and utilities
│   └── ibkr/                         # IBKR notebooks and examples
├── requirements.txt
├── .env.template
└── README.md
```

## Quick Start

### 1) Create and activate a virtual environment

```bash
python3 -m venv venv
source venv/bin/activate
```

### 2) Install dependencies

```bash
pip install -r requirements.txt
```

### 3) Launch Jupyter

```bash
jupyter notebook
```

Open notebooks in `pandas-financial-data-analysis/` to start with the analytics track.

## Recommended Learning Path (Pandas Financial Analysis)

A practical sequence:
1. `1-yahooFinance.ipynb`
2. `2-priceChangesAndFinancialReturns.ipynb`
3. `3-measuring-reward-and-risk-finanical-instruments.ipynb`
4. `5-investment-multiple-and-CAGR.ipynb`
5. `6-compound-returns-and-geometric-return.ipynb`
6. `10-log-returns.ipynb`
7. `12-comparing-financial-instruments.ipynb`
8. `13-none-normality-of-finacial-returns.ipynb`
9. `14-annualising-return-and-risk.ipynb`
10. `15-resample-smoothing-financial-data.ipynb`
11. `16-rolling-statisitics.ipynb`
12. `18-shortselling-explainer.ipynb`
13. `19-shortselling-example.ipynb`
14. `20-coding-challenge-shortselling.ipynb`
15. `21-portfolio-returns.ipynb`
16. `21-covariance-correlation-and-portfolio-diversification.ipynb`
17. `22-leverage-and-margin-trading-returns.ipynb`
18. `22-leverage-with-real-data.ipynb`
19. `23-coding-challenge-leverage.ipynb`

Challenge notebooks are included throughout (e.g. `0`, `4`, `7`, `11`, `17`, `20`, `23`).

## Data Files Used by Notebooks

Common local datasets in `pandas-financial-data-analysis/`:
- `close.csv`
- `different_assets.csv`
- `msft.csv`

Several notebooks can also fetch data online (e.g., `yfinance`) and include fallbacks when fetch is unavailable.

## Broker Tracks

### OANDA
- Path: `brokers/oanda/`
- Includes connection helpers and example trading/data scripts.
- Configure credentials via `.env` (see `.env.template`).

### IBKR
- Path: `brokers/ibkr/`
- Includes notebooks for connectivity, contracts, market data, and trading examples.
- Requires TWS/IB Gateway with API enabled.

## Configuration

Create a `.env` file in the project root (copy from `.env.template`) and add required keys for broker examples.

Example OANDA fields:

```env
OANDA_API_KEY=your_api_key_here
OANDA_ACCOUNT_ID=your_account_id_here
OANDA_ENVIRONMENT=practice
```

## Safety Notes

- Use paper/demo environments first.
- Do not commit API keys or account secrets.
- Treat all notebooks/scripts as educational examples and validate logic before any live deployment.

## Disclaimer

This repository is for educational purposes only. Trading and investing involve risk, including potential loss of capital.
