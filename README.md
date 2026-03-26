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

</div>

---

🎥 Live Demo: AI predicting stock trends in real-time: https://drive.google.com/file/d/1AJryxzrN2oh1xKYd3mWqTMw-zzDqQTSz/view?usp=drivesdk
---

## 🌟 Project Overview

**LiveStockForecast** ek professional-grade, real-time AI stock trading dashboard hai jo **Streamlit** aur **Yahoo Finance API** ke saath bana hai. Yeh dashboard live price monitoring, AI-powered price predictions, technical analysis, aur paper trading simulator sab kuch ek jagah provide karta hai — bilkul ek pro trading terminal ki tarah.

> **Yeh kaam kya karta hai?**  
> Har **5 seconds** mein live stock prices fetch karta hai, real-time technical indicators calculate karta hai, aur **multiple AI models** combine karke next price prediction deta hai. Saath mein volume pressure, RSI momentum, ATR volatility aur MACD trend bhi dikhata hai.

---

## ✨ Key Features

```
┌─────────────────────────────────────────────────────────────┐
│  📡 LIVE PRICE      →  Real-time price via yFinance API     │
│  🔮 AI PREDICTIONS  →  LR + MA + Volume + RSI + ATR Model  │
│  📊 TECHNICAL       →  RSI, MACD, BB, VWAP, EMA, SMA       │
│  🕯️  CANDLESTICK    →  Interactive TradingView-style chart  │
│  📰 NEWS FEED       →  Latest stock news auto-fetched       │
│  💼 PORTFOLIO       →  Real-time P&L tracker                │
│  🎯 PAPER TRADING   →  Virtual $1,00,000 simulator          │
│  📐 SUPPORT/RESIST  →  Auto S/R level detection             │
└─────────────────────────────────────────────────────────────┘
```

---

## 🤖 AI Prediction Engine

Yeh dashboard ek **custom multi-factor prediction model** use karta hai jo sirf static Linear Regression nahi hai — har refresh pe genuinely alag value aati hai:

| Model Component | Description |
|---|---|
| 📐 **Linear Regression** | Historical price trend se slope-based projection |
| 📊 **MA + Volume Pressure** | Moving average + above-average volume multiplier |
| ⚡ **RSI Momentum Bias** | Overbought/oversold zones se direction adjustment |
| 🌊 **ATR Volatility** | Average True Range se prediction spread decide hoti hai |
| 📈 **MACD Direction** | EMA crossover se trend strength weighting |
| 🎲 **Microstructure Noise** | `time.time()` seeded noise — real bid/ask fluctuation simulate karta hai |
| 🤖 **AI Combined** | 35% LR + 35% MA + 15% Momentum + 15% MACD blend |

> **Confidence Score** (45%–95%) bhi dynamically calculate hoti hai based on recent candle direction consistency aur volume ratio.

---

## 📸 Dashboard Tabs

| Tab | Description |
|---|---|
| 🕯️ Candlestick | Full OHLC chart with BB, EMA50/200, VWAP, S/R levels, prediction arrows |
| 📉 Line Plot | Price line with comparison mode (upto 3 stocks simultaneously) |
| 📊 MACD | MACD histogram + signal line chart |
| 📦 Volume | Volume bars with 20-period moving average |
| 📰 News | Latest news articles for selected stock |
| 💼 Portfolio | Live P&L for tracked portfolio holdings |
| 🎯 Trade Tracker | Paper trading — buy/sell with stop loss & target |

---

## 🚀 Quick Start

### 1. Clone the repo
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

> 🌐 Opens at `http://localhost:8501`

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
├── app.py              # 🚀 Main Streamlit dashboard
├── train.py            # 🧠 Model training utilities
├── model/              # 📦 Saved model artifacts
├── requirements.txt    # 📋 Python dependencies
└── README.md           # 📖 You are here
```

---

## ⚙️ Configuration (Sidebar)

| Setting | Range | Default | Effect |
|---|---|---|---|
| SMA Window | 5–50 | 10 | Simple Moving Average period |
| EMA Fast | 5–30 | 12 | Fast EMA for MACD |
| EMA Slow | 20–100 | 26 | Slow EMA for MACD |
| BB Window | 10–50 | 20 | Bollinger Band period |
| BB Std Dev | 1.0–3.0 | 2.0 | Band width multiplier |
| Refresh Rate | 5/10/30/60s | 5s | Live data refresh interval |

---

## 📊 Supported Stocks

```
AAPL  GOOGL  MSFT  TSLA  AMZN
META  NVDA   NFLX  AMD   INTC
```
> Compare mode mein ek saath 3 stocks simultaneously dekh sakte hain (normalized).

---

## ⚠️ Disclaimer

> Yeh dashboard **educational aur learning purposes** ke liye hai. Isme jo predictions aur signals hain woh **financial advice nahi hain**. Real money trading mein use karne se pehle apne financial advisor se consult karein. Market investments subject to market risk hain.

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



