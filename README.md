# Sentiment-Driven Behavioral Trading Analysis on Hyperliquid

## Project Overview
## Notebook Access

Kaggle Notebook:  
[https://www.kaggle.com/code/tejakarri/sentiment-trading-analysis-ipynb]


This project investigates how Bitcoin market sentiment influences trader profitability, capital deployment behavior, whale-trade dynamics, and predictive trade outcomes using Hyperliquid execution data and the Bitcoin Fear & Greed Index.

The workflow combines:
- exploratory behavioral analysis
- outlier-resistant financial visualization
- whale-trade investigation
- sentiment-regime segmentation
- interpretable machine learning
- trading strategy synthesis

to identify sentiment-aware trading patterns within crypto markets.

---

# Objective

The primary objective of this project was to analyze whether market sentiment regimes meaningfully influence:
- trader profitability
- risk behavior
- capital deployment
- whale-trade concentration
- predictive trading outcomes

using real-world crypto execution data.

---

# Datasets Used

## 1. Bitcoin Fear & Greed Index
Contains:
- daily sentiment classifications
- numerical sentiment scores
- historical market psychology indicators

## 2. Hyperliquid Historical Trader Data
Contains:
- trade execution prices
- realized profit & loss
- trade direction
- transaction metadata
- capital deployment information

---

# Project Workflow

## Phase 1 — Data Loading & Initial Exploration
- Loaded and validated both datasets
- Performed missing-value verification
- Analyzed initial financial distributions
- Exported summary statistics and inspection tables

## Phase 2 — Temporal Alignment & Data Integration
- Standardized timestamps
- Created unified merge dates
- Merged sentiment data with trader execution records
- Investigated merge anomalies and removed unmatched rows

## Phase 3 — Feature Engineering & Trade Segmentation
- Segmented trade openings vs realized outcomes
- Created profitability classification targets
- Engineered sentiment-aware analytical features
- Analyzed capital deployment behavior

## Phase 4 — Exploratory Behavioral Analysis
- Applied percentile trimming for heavy-tail visualization
- Investigated sentiment-specific profitability patterns
- Analyzed BUY vs SELL regime behavior
- Conducted whale-trade analysis
- Explored volatility-dependent trading structures

## Phase 5 — Predictive Modeling & Error Analysis
- Built RandomForest profitability classifier
- Applied RobustScaler for heavy-tail financial distributions
- Evaluated class imbalance effects
- Extracted feature importance rankings
- Investigated model misclassification behavior

## Phase 6 — Strategy Formulation & Analytical Synthesis
- Converted empirical findings into sentiment-aware trading insights
- Identified regime-dependent risk behaviors
- Synthesized actionable analytical conclusions

---

# Key Findings

## Sentiment Intensity Was the Strongest Predictive Signal
The numerical Fear & Greed score emerged as the single most important predictive feature during RandomForest modeling.

## Fear Regimes Produced Strong Opportunity Structures
Moderate Fear conditions generated:
- high whale-profit concentration
- elevated capital deployment
- strong profitability behavior

suggesting volatility-driven trading opportunities.

## Extreme Fear Concentrated Catastrophic Losses
Extreme Fear environments produced:
- the highest concentration of whale losses
- lower profitability stability
- increased downside risk exposure

## SELL Trades Consistently Outperformed BUY Trades
SELL-side trades achieved stronger win rates across most sentiment regimes, especially during:
- Greed
- Extreme Greed
- Neutral conditions

## Whale Behavior Was Highly Regime-Dependent
Large profit and loss events were not randomly distributed and exhibited strong sentiment-dependent asymmetry.

---

# Machine Learning Results

RandomForest classification achieved approximately:
- **Accuracy:** 80%
- **Profit Recall:** 82%
- **Loss Recall:** 70%

while successfully capturing:
- nonlinear trading behavior
- sentiment-regime effects
- heavy-tail financial structure
- directional trade asymmetry

---

# Repository Structure

```text
datasets/   -> cleaned analytical dataset
notebook/   -> final Kaggle notebook
plots/      -> exported visualizations
tables/     -> exported analytical summaries
```

---

# Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Kaggle Notebook Environment

---

# Future Improvements

Potential future extensions include:
- time-series sequence modeling
- regime-switching volatility analysis
- confidence-threshold trading systems
- real-time sentiment integration
- advanced ensemble learning methods

---

# Final Conclusion

This analysis demonstrated that market sentiment materially influences:
- trader profitability
- capital deployment behavior
- whale-trade dynamics
- predictive trading stability

within the Hyperliquid trading ecosystem.

The resulting workflow combined:
- behavioral financial analysis
- robust exploratory analytics
- interpretable machine learning
- sentiment-aware strategy synthesis

to construct a comprehensive sentiment-driven crypto trading analysis framework.
