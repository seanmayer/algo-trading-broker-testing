# OANDA Algo Trading Basics

A comprehensive proof-of-concept for algorithmic trading with OANDA and Interactive Brokers APIs.

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- OANDA account (for OANDA examples)
- Interactive Brokers account with TWS/IB Gateway (for IBKR examples)

### Installation

1. **Clone or download this repository**

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up your trading credentials** (see Configuration section below)

4. **Start trading!** Open the Jupyter notebooks and begin exploring.

## 📁 Project Structure

```
oanda-algo-trading-basics/
├── brokers/
│   ├── oanda/          # OANDA-specific implementations
│   └── ibkr/           # Interactive Brokers implementations
│       └── notebooks/  # Jupyter notebooks for IBKR
├── requirements.txt    # Python dependencies
└── README.md          # This file
```

## 📚 Available Notebooks

### Interactive Brokers (IBKR)
- **`HistoricalAccountValues.ipynb`** - Fetch and analyze historical market data
- **`TradingChallenge.ipynb`** - Complete SMA crossover trading system with performance analysis

## ⚙️ Configuration

### OANDA Setup
1. Create a `.env` file in the project root
2. Add your OANDA credentials:
   ```
   OANDA_API_KEY=your_api_key_here
   OANDA_ACCOUNT_ID=your_account_id_here
   OANDA_ENVIRONMENT=practice  # or 'live' for real trading
   ```

### Interactive Brokers Setup
1. Install and run TWS (Trader Workstation) or IB Gateway
2. Enable API connections in TWS/Gateway settings:
   - Go to Global Configuration → API → Settings
   - Enable "Enable ActiveX and Socket Clients"
   - Note the Socket Port (usually 7497 for TWS, 4001 for Gateway)
3. The notebooks will connect to `localhost:7497` by default

## 🛡️ Important Safety Notes

⚠️ **ALWAYS USE PAPER TRADING FIRST!**

- Start with demo/paper trading accounts
- Test all strategies thoroughly before risking real money
- The code includes educational examples - modify for your risk tolerance
- Never commit API keys or credentials to version control

## 💡 Getting Started Examples

### 1. Historical Data Analysis
```python
# Run HistoricalAccountValues.ipynb
# - Fetch EUR/USD historical data
# - Analyze price movements
# - Convert data to pandas DataFrames
```

### 2. Complete Trading System
```python
# Run TradingChallenge.ipynb
# - Implement SMA crossover strategy
# - Execute backtests on historical data
# - Analyze performance metrics
# - Optional: Run live signal monitoring
```

## 📊 Features

- ✅ **Multiple Broker Support** - OANDA and Interactive Brokers
- ✅ **Historical Data** - Fetch and analyze market data
- ✅ **Trading Strategies** - SMA crossover and more
- ✅ **Risk Management** - Stop-loss, take-profit, position sizing
- ✅ **Performance Analysis** - Win rate, Sharpe ratio, drawdown analysis
- ✅ **Visualization** - Charts and performance metrics
- ✅ **Backtesting** - Test strategies on historical data

## 🔧 Dependencies

Key libraries used:
- **ib_async** - Interactive Brokers API
- **oandapyV20** - OANDA REST API
- **pandas/numpy** - Data analysis
- **matplotlib** - Visualization
- **requests** - HTTP requests

## 🤝 Contributing

This is a proof-of-concept project. Feel free to:
- Add new trading strategies
- Improve risk management
- Add support for other brokers
- Enhance visualizations

## ⚠️ Disclaimer

This software is for educational purposes only. Trading involves significant risk of loss. The authors are not responsible for any financial losses incurred through the use of this software. Always do your own research and consider consulting with a financial advisor.

## 📞 Support

For questions or issues:
1. Check the notebook comments and documentation
2. Review the broker API documentation
3. Test with paper trading accounts first
4. Ensure all dependencies are properly installed

---

**Happy Trading! 📈**