# Stock Direction Predictor

## Problem Statement
Can I predict whether the Nifty 50 index will close higher or lower 
tomorrow, using only information available at the end of today?

## Data
- Source: Yahoo Finance via yfinance
- Asset: Nifty 50 Index (^NSEI)
- Period: January 2019 – December 2024
- Rows: 1477 trading days
- Baseline accuracy (always predict up): 55.0%
- File: `data/nifty50_raw.csv`

## Why This Matters
Short-term market direction prediction is a classic and challenging 
machine learning problem. This project explores whether technical 
indicators derived from historical price data carry any predictive signal.

## Data
- Source: Yahoo Finance via yfinance
- Asset: Nifty 50 Index (^NSEI)
- Period: January 2019 – December 2024 (5 years)
- Frequency: Daily OHLCV (Open, High, Low, Close, Volume)

## Target Variable
- 1 → tomorrow's closing price is higher than today's
- 0 → tomorrow's closing price is lower than today's

## Assumptions
- Only end-of-day data is used (no intraday, no news, no sentiment)
- Prediction horizon is exactly 1 day ahead
- Past price patterns contain some predictive signal

## Success Metrics
- Primary: Accuracy > 55% on test set
- Secondary: Confusion matrix analysis
- Baseline to beat: naive model that always predicts "up"

## Project Stages
- [x] Stage 1: Problem definition
- [x] Stage 2: Data collection
- [ ] Stage 3: Feature engineering
- [ ] Stage 4: Modeling
- [ ] Stage 5: Evaluation
- [ ] Stage 6: Notebook cleanup
- [ ] Stage 7: Publish

## Tools
Python, yfinance, pandas, scikit-learn, matplotlib, Google Colab
