<div align="center">

<!-- Animated Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=📈%20LiveStockForecast&fontSize=50&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Real-Time%20AI-Powered%20Stock%20Trading%20Dashboard&descSize=18&descAlignY=58&descColor=aaaaaa" width="100%"/>

<!-- Badges -->
<p>
  <img src="https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white"/>
  <img src="https://img.shields.io/badge/yFinance-00897B?style=for-the-badge&logo=yahoo&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
</p>

<p>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square"/>
  <img src="https://img.shields.io/badge/Refresh-5s%20Live-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/Stocks-10%2B-orange?style=flat-square"/>
</p>

<br/>

> **A professional-grade, real-time AI stock trading dashboard built with Streamlit and Yahoo Finance API.**
> Live price monitoring · AI-powered predictions · Full technical analysis · Paper trading simulator — all in one terminal.

</div>

---

🎥 Live Demo: AI predicting stock trends in real-time: https://drive.google.com/file/d/1AJryxzrN2oh1xKYd3mWqTMw-zzDqQTSz/view?usp=drivesdk

---

## 🌟 Project Overview

**LiveStockForecast** is a real-time, AI-driven stock market dashboard that refreshes every **5 seconds** to deliver live price data, dynamic technical indicators, and multi-model price predictions — designed to look and feel like a professional trading terminal.

The dashboard fetches live stock prices via the **Yahoo Finance API**, computes a suite of technical indicators in real time, and combines **multiple prediction models** (Linear Regression, Moving Average, RSI Momentum, ATR Volatility, MACD Trend, and Volume Pressure) into a single unified AI forecast with a confidence score.

---

## ✨ Key Features

```
┌─────────────────────────────────────────────────────────────────┐
│  📡 LIVE PRICE       →  Real-time price fetched via yFinance    │
│  🔮 AI PREDICTIONS   →  LR + MA + Volume + RSI + ATR Model     │
│  📊 TECHNICAL TOOLS  →  RSI, MACD, BB, VWAP, EMA50/200, SMA    │
│  🕯️  CANDLESTICK     →  Interactive TradingView-style chart     │
│  📐 SUPPORT/RESIST   →  Auto S/R level detection & annotation   │
│  📰 NEWS FEED        →  Latest stock news auto-fetched          │
│  💼 PORTFOLIO        →  Real-time P&L tracker for holdings      │
│  🎯 PAPER TRADING    →  Virtual $100,000 trade simulator        │
└─────────────────────────────────────────────────────────────────┘
```

---

## 🤖 AI Prediction Engine

This dashboard uses a **custom multi-factor prediction model** that generates genuinely different values on every refresh cycle — not just a static linear projection.

| Model Component | Description |
|---|---|
| 📐 **Linear Regression** | Slope-based price projection from historical close data |
| 📊 **MA + Volume Pressure** | Moving average weighted by above-average volume ratio |
| ⚡ **RSI Momentum Bias** | Directional adjustment based on overbought/oversold zones |
| 🌊 **ATR Volatility** | Average True Range determines prediction spread width |
| 📈 **MACD Direction** | EMA crossover signal used for trend strength weighting |
| 🎲 **Market Microstructure** | `time.time()` seeded noise simulating live bid/ask fluctuation |
| 🤖 **AI Combined Score** | 35% LR + 35% MA + 15% Momentum + 15% MACD weighted blend |

The **Confidence Score** (range: 45%–95%) is dynamically computed based on recent candle direction consistency and real-time volume ratio, giving you a clear sense of how reliable each prediction cycle is.

---

## 📸 Dashboard Tabs

| Tab | What It Shows |
|---|---|
| 🕯️ **Candlestick** | Full OHLC chart with Bollinger Bands, EMA50/200, VWAP, S/R levels, and live prediction arrows |
| 📉 **Line Plot** | Price line chart with multi-stock comparison mode (up to 3 stocks simultaneously, normalized) |
| 📊 **MACD** | MACD line, signal line, and histogram with zero-line reference |
| 📦 **Volume** | Color-coded volume bars with 20-period moving average overlay |
| 📰 **News Feed** | Latest news articles auto-fetched for the selected stock |
| 💼 **Portfolio** | Live P&L tracking for your configured portfolio holdings |
| 🎯 **Trade Tracker** | Full paper trading simulator with stop loss, target price, and balance management |

---

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/live-stock-forecast.git
cd live-stock-forecast
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the dashboard
```bash
streamlit run app.py
```

> 🌐 Dashboard opens at `http://localhost:8501`

---

## 📦 Requirements

```txt
streamlit>=1.32.0
yfinance>=0.2.36
pandas>=2.0.0
numpy>=1.24.0
plotly>=5.18.0
```

---

## 📁 Project Structure

```
live-stock-forecast/
│
├── app.py              # 🚀 Main Streamlit dashboard application
├── train.py            # 🧠 Model training and utility functions
├── model/              # 📦 Saved model artifacts
├── requirements.txt    # 📋 Python package dependencies
└── README.md           # 📖 Project documentation
```

---

## ⚙️ Sidebar Configuration

| Setting | Range | Default | Effect |
|---|---|---|---|
| SMA Window | 5 – 50 | 10 | Simple Moving Average period |
| EMA Fast | 5 – 30 | 12 | Fast EMA span used in MACD |
| EMA Slow | 20 – 100 | 26 | Slow EMA span used in MACD |
| BB Window | 10 – 50 | 20 | Bollinger Band rolling period |
| BB Std Dev | 1.0 – 3.0 | 2.0 | Band width multiplier |
| Refresh Rate | 5 / 10 / 30 / 60s | 5s | Live data auto-refresh interval |

---

## 📊 Supported Stocks

```
AAPL   GOOGL   MSFT   TSLA   AMZN
META   NVDA    NFLX   AMD    INTC
```

> Use **Compare Mode** to overlay up to 3 stocks simultaneously on the Line Plot tab (prices normalized to a common base for fair comparison).

---

## ⚠️ Disclaimer

> This dashboard is built for **educational and learning purposes only**. The predictions, signals, and indicators shown here do **not** constitute financial advice. Please consult a qualified financial advisor before making any real investment decisions. All market investments are subject to market risk.

---

<div style="text-align:center; padding:20px; border-radius:15px; background:linear-gradient(135deg,#0f2027,#203a43,#2c5364); color:white;">

  <h1>👨‍💻 Shiv Kumavat</h1>

  <p style="font-size:18px;">
    🚀 AI & ML Developer <br>
    📊 Building Smart Dashboards & Predictive Systems
  </p>

  <marquee behavior="scroll" direction="left" scrollamount="6">
    🔥 AI • Machine Learning • Stock Prediction • Real-Time Systems 🔥
  </marquee>

  <br><br>

  <a href="https://github.com/shivtechcrafts-sketch" style="text-decoration:none;">
    <button style="padding:10px 20px; border:none; border-radius:10px; background:#00c6ff; color:black; font-weight:bold;">
      Visit GitHub
    </button>
  </a>

</div>
---

