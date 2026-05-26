# 📈 Real-Time Stock Price Tracker

A Python desktop application for tracking live stock prices with real-time charts, historical data, and key financial metrics — powered by Yahoo Finance (no API key required).

> Part of my financial data engineering portfolio — demonstrates real-time data ingestion, Pandas-based metric computation, and GUI development.

---

## 📊 What It Tracks

| Metric | Description |
|--------|-------------|
| Live price | Real-time stock price with % change |
| Market Cap | Total market capitalisation |
| P/E Ratio | Price-to-earnings ratio |
| 52-week range | High and low over the past year |
| Dividend yield | Annual dividend as % of price |
| Volume | Trading volume for current session |

---

## ✨ Features

- **Real-time data** — pulls live prices from Yahoo Finance with no API key
- **Interactive charts** — Matplotlib price trend visualisations
- **Historical data table** — Open, High, Low, Close, Volume across multiple timeframes
- **Auto-refresh** — configurable interval (10 seconds to 1 hour)
- **Multi-timeframe** — 1 day, 5 days, 1 month, 3 months, 6 months, 1 year
- **100+ tickers** — tracks any stock symbol available on Yahoo Finance

---

## 🖥️ Screenshot

![Stock Tracker App](image.png)

---

## 🚀 Quick Start

### Prerequisites
- Python 3.8+

### Install & run

```bash
git clone https://github.com/Soumya0713/Stock-price-tracker.git
cd Stock-price-tracker
pip install -r requirements.txt
python main.py
```

### Usage
1. Enter a stock ticker (e.g. `AAPL`, `RELIANCE.NS`, `TCS.NS`)
2. Select a timeframe from the dropdown
3. Toggle auto-refresh and set the interval
4. View live price, charts, and financial metrics instantly

---

## 🏗️ Architecture

```
Yahoo Finance API (yfinance)
        ↓
main.py  ← Fetches data, computes metrics (Market Cap, P/E, 52wk range)
        ↓
Pandas   ← OHLCV data processing & metric calculation
        ↓
Matplotlib ← Renders price charts
        ↓
Tkinter UI ← Desktop GUI with tables, charts, refresh controls
```

---

## ⚡ Performance

- Sub-5 second data refresh for any ticker
- Handles 100+ stock symbols simultaneously
- Auto-refresh with configurable intervals (10s minimum)

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **yfinance** — Yahoo Finance data ingestion
- **Pandas** — financial metric computation & data processing
- **Matplotlib** — interactive price charts
- **Tkinter** — desktop GUI framework

---

## 📈 Possible Improvements

- [ ] Add portfolio tracking (multiple tickers, P&L calculation)
- [ ] Export data to CSV
- [ ] Add moving averages and RSI indicators
- [ ] Build a web version with Streamlit or Dash

---

## 📄 License

MIT License — see [LICENSE](LICENSE)

---

## 👤 Author

**Soumya Barve**
[LinkedIn](https://www.linkedin.com/in/soumya-barve-02767026b/) · [GitHub](https://github.com/Soumya0713) · soumyabarve224@gmail.com
