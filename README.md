# Daily WIG20 Returns and Risk Analysis

## Abstract
This project analyzes daily returns of the WIG20 index (Warsaw Stock Exchange) over eight years (2015–2023). The focus is on descriptive statistics, testing for normality, and estimating financial risk measures, including Value at Risk (VaR) and Expected Shortfall (ES), using historical and EWMA methods. Backtesting validates the accuracy and time-dependence of risk estimates.

## Problem Statement
WIG20 consists of the 20 largest companies in Poland. Understanding the distribution of returns and risk is crucial for portfolio management and regulatory compliance. The study evaluates the effectiveness of simple historical vs. conditional volatility (EWMA) models in capturing market dynamics.

## Methods
- **Simple historical VaR and ES** – non-parametric, based on empirical distribution.
- **EWMA (Exponentially Weighted Moving Average)** – accounts for heteroskedasticity and emphasizes recent volatility.
- **Backtesting** – Kupiec and Christoffersen tests to validate unconditional coverage and independence of VaR violations.

## Findings
- Returns exhibit negative skewness and high kurtosis (fat tails).
- Both methods capture volatility, but EWMA responds faster to sudden market changes.
- Historical VaR satisfies unconditional coverage but shows time-dependence; EWMA better handles time dynamics but slightly overestimates violations.

## Files
- `main.ipynb` – code and calculations
- `analyse_risk_wig20_market.pdf` – detailed project report
