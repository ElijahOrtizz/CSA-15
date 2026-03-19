# CSA-15 Crypto Scalping Indicator

TradingView Pine Script indicator for crypto scalping that uses multi-confirmation logic to generate BUY/SELL alerts for short-term trade setups.

##  Overview

CSA-15 is a custom TradingView indicator built for fast-paced crypto trading. It combines multiple confirmations such as trend, momentum, volume, and candle behavior to reduce weak entries and improve signal quality.

This project was built as a practical trading automation tool and is designed to work with alert-based execution workflows such as TradersPost and broker integrations like Webull.

##  Features

- Multi-confirmation BUY/SELL alerts
- Trend-based trade filtering
- Momentum confirmation
- Volume-aware signal logic
- Candle structure confirmation
- Squeeze and volatility behavior filtering
- ATR-based take profit and stop loss projection
- Alert-ready for automation workflows
- Built in TradingView Pine Script

##  Strategy Logic

The indicator evaluates trade opportunities using a confirmation-based framework:

1. **Trend Direction**  
   Uses moving averages to identify bullish or bearish structure.

2. **Momentum Confirmation**  
   Uses RSI, stochastic behavior, and momentum slope to confirm strength.

3. **Volume Behavior**  
   Uses volume surge logic to validate whether a move has enough participation.

4. **Candle Structure**  
   Uses Heikin Ashi confirmation to reduce weak entries.

5. **Volatility / Squeeze Logic**  
   Uses squeeze conditions and momentum expansion behavior to help filter setups.

6. **Risk Projection**  
   Displays ATR-based take profit and stop loss levels when signals appear.

A signal is only generated when multiple conditions align and the minimum score threshold is met.

##  Tech Stack

- **Language:** TradingView Pine Script v5
- **Charting Platform:** TradingView
- **Automation Workflow:** TradersPost
- **Execution Compatibility:** Webull alert workflow

##  Screenshot

![CSA-15 Chart Preview](assets/chart-preview.png)

##  Repository Structure

```text
CSA-15/
├── README.md
├── src/
│   └── CSA-15.pine
└── assets/
    └── chart-preview.png
