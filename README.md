# Pair Trading Strategy Using Statistical Arbitrage

This project explores a quantitative trading strategy based on pair trading principles using statistical arbitrage.

## 📈 Overview

The strategy identifies two highly correlated stocks—**GOOGL** and **ACN**—and executes trades based on the spread between their normalized prices. The model uses cointegration tests, correlation analysis, and regression-based beta spread to generate trading signals.

## 🧠 Core Concepts

- **Mean Reversion**: Strategy assumes that the price spread between two correlated stocks will revert to its historical mean.
- **Statistical Arbitrage**: Trades are initiated when the spread deviates beyond one standard deviation and closed when it reverts.

## 🔧 Tools & Libraries

- `yfinance` for data collection
- `pandas` & `numpy` for analysis
- `matplotlib` for visualization
- Linear regression for calculating beta

## 📊 Key Metrics

- **Cumulative Return**: 221.78%
- **Sharpe Ratio**: 1.15
- **Max Drawdown**: −9.54%
- **Annualized Alpha**: 24.59%
- **Profit Factor**: 1.77

## 📅 Data Period

Historical data was used from **01/01/2019 to 31/12/2023** for both stocks.

## 🔍 Strategy Logic

- **Signal = +1**: Short GOOGL, Long ACN (spread > +1 std dev)
- **Signal = -1**: Long GOOGL, Short ACN (spread < -1 std dev)
- Neutral when spread is within ±1 std dev.

## 📁 Files

- `fin_club_application.pdf`: Full write-up of the strategy, methodology, performance analysis, and suggested improvements.
