# CSA-15 Crypto Scalping Indicator

TradingView Pine Script indicator for crypto scalping that uses multi-confirmation logic to generate BUY/SELL alerts for short-term trade setups.

## Overview

CSA-15 is a custom TradingView indicator built for fast-paced crypto trading.  
It combines multiple confirmations such as trend, momentum, volume, and candle behavior to reduce weak entries and improve signal quality.

This project was built as a practical trading automation tool and is designed to work with alert-based execution workflows such as TradersPost and broker integrations like Webull.

## Features

- Multi-confirmation BUY/SELL alerts
- Trend-based trade filtering
- Momentum confirmation
- Volume-aware signal logic
- Candle structure confirmation
- Designed for short-term crypto scalping
- Alert-ready for automation workflows
- Built in TradingView Pine Script

## Strategy Logic

The indicator evaluates trade opportunities using a confirmation-based framework:

1. **Trend Direction**  
   Uses moving-average logic to determine whether the market is bullish or bearish.

2. **Momentum Confirmation**  
   Checks whether price movement has enough strength to support an entry.

3. **Volume Behavior**  
   Uses volume conditions to help validate whether a move has participation behind it.

4. **Candle Structure**  
   Filters entries based on candle behavior to avoid weak or noisy setups.

A signal is only generated when multiple conditions align.

## Tech Stack

- **Language:** TradingView Pine Script
- **Charting Platform:** TradingView
- **Automation Workflow:** TradersPost
- **Execution Environment:** Webull-compatible alert workflow

## Use Case

This project is intended for traders who want:

- Faster decision support on lower timeframes
- Structured BUY/SELL alerts instead of manual guesswork
- A more rules-based approach to crypto scalping
- Integration potential with alert automation systems

## Repository Structure

```text
CSA-15/
├── README.md
├── src/
│   └── CSA-15.pine
├── docs/
│   ├── setup-guide.md
│   └── strategy-notes.md
└── assets/
    └── chart-preview.png
