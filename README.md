<div align="center">

<h1>Aurora Quant</h1>

<p>
<i>An autonomous quantitative trading intelligence designed to study and navigate financial markets.</i>
</p>

<img src="https://img.shields.io/badge/Quantitative-Trading-black?style=for-the-badge">
<img src="https://img.shields.io/badge/Machine-Learning-LightGBM-darkgreen?style=for-the-badge">
<img src="https://img.shields.io/badge/Market-Crypto-blue?style=for-the-badge">
<img src="https://img.shields.io/badge/Architecture-Systematic-purple?style=for-the-badge">

</div>

---

## Aurora

Aurora Quant is a **quantitative trading intelligence** designed to analyze financial markets through data, statistical models, and machine learning.

Aurora studies market behavior continuously, identifying structural patterns, volatility shifts, and probabilistic opportunities in cryptocurrency markets.

Unlike conventional trading bots that rely on simple indicators, Aurora operates as a **multi-layer decision system** combining quantitative strategies and machine learning filtering.

Her objective is simple:

> transform market data into statistically validated trading decisions.

---

## System Overview

Aurora operates through a modular quantitative architecture.

```
Market Data
│
▼
Feature Engineering
│
▼
Market Regime Detection
│
▼
Strategy Signal Generation
│
▼
Machine Learning Probability Filter
│
▼
Risk Management
│
▼
Execution Engine
```

Each layer serves as a filter, reducing noise and increasing the probability of profitable trades.

---

## Quantitative Strategies

Aurora integrates multiple systematic strategies that activate under different market conditions.

### Trend Following

Captures sustained directional market movements.

Conditions where it operates best:

- strong bullish trends
- strong bearish trends
- momentum continuation environments

Primary indicators:

```
EMA 9
EMA 21
EMA 50
EMA 200
ADX
trend strength metrics
```

---

### Mean Reversion

Detects short-term price exhaustion and temporary inefficiencies.

Conditions where it operates best:

- sideways markets
- temporary volatility spikes
- overbought / oversold environments

Primary indicators:

```
RSI
Stochastic oscillator
Bollinger Bands
volatility bands
```

---

### Volatility Breakout

Identifies moments where volatility expands and price escapes a consolidation range.

Conditions where it operates best:

- regime transitions
- momentum accelerations
- liquidity breakouts

Primary indicators:

```
ATR expansion
volume spikes
range breakouts
volatility compression signals
```

---

## Machine Learning Engine

Aurora integrates a **gradient boosting decision model** to filter strategy signals.

Model architecture:

```
LightGBM Classifier
```

The model evaluates features extracted from market data and estimates the probability that a signal will result in a profitable trade.

Model output:

```
prob_long
prob_short
```

Trade execution rules:

```
long  if prob_long  > threshold
short if prob_short > threshold
otherwise no trade
```

This probabilistic filtering significantly reduces false signals.

---

## Feature Engineering

Aurora analyzes the market through a structured set of engineered features.

### Trend Features

```
ema_9
ema_21
ema_50
ema_200
ema_ratios
trend_strength
```

### Momentum Features

```
rsi
macd
stochastic_k
stochastic_d
rate_of_change
```

### Volatility Features

```
atr
true_range
volatility_windows
bollinger_width
```

### Market Structure

```
swing_high
swing_low
break_of_structure
change_of_character
liquidity_levels
range_extremes
```

### Volume Analytics

```
volume_moving_averages
volume_spikes
vwap
price_vs_vwap
```

These features allow Aurora to understand the **state of the market**, not just price movement.

---

## Market Regime Detection

Aurora first determines the type of market environment before activating strategies.

Possible regimes:

```
bullish trend
bearish trend
range
high volatility
low volatility
```

Strategies are only allowed to operate within regimes where they historically perform best.

---

## Risk Management

Aurora prioritizes capital protection.

Core risk rules:

```
risk per trade: 0.5% – 1%
dynamic stop loss: ATR based
volatility adjusted position sizing
maximum exposure limits
```

Typical configuration:

```
stop_loss  = 1.5 × ATR
take_profit = 3 × ATR
```

Position sizing is calculated according to the distance to the stop loss.

---

## Backtesting Framework

Aurora is validated using institutional-grade research procedures.

Testing pipeline:

```
historical backtesting
walk-forward validation
Monte Carlo simulations
execution noise testing
parameter sensitivity analysis
```

These procedures help detect overfitting and ensure statistical robustness.

---

## Performance Evaluation

Aurora measures performance using professional quantitative metrics.

```
CAGR
Sharpe Ratio
Sortino Ratio
Profit Factor
Maximum Drawdown
Calmar Ratio
Win Rate
```

The focus is not raw profitability but **risk-adjusted performance**.

---

## Technology Stack

Aurora Quant is built with modern data science infrastructure.

```
Python
LightGBM
NumPy
Pandas
VectorBT
Backtrader
Parquet datasets
```

Data sources include cryptocurrency exchanges such as:

```
Binance
```

---

## Research Methodology

Aurora follows a systematic research cycle.

```
hypothesis generation
feature engineering
model training
out-of-sample testing
walk-forward validation
live deployment
```

Only strategies that pass statistical validation become part of the system.

---

## Project Vision

Aurora Quant is designed as a long-term quantitative research platform.

Future development includes:

```
ensemble machine learning models
automatic feature discovery
dynamic strategy allocation
continuous retraining pipelines
multi-asset expansion
```

The long-term objective is to build a **fully adaptive quantitative trading intelligence**.

---

<div align="center">

Aurora Quant

<i>Systematic. Probabilistic. Autonomous.</i>

</div>
