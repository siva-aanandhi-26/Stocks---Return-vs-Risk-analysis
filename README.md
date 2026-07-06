# US Tech Stocks Return-Risk Performance Analysis Dashboard

## Overview
This project analyzes the return, risk, and trend performance of major US technology stocks — **AAPL, AMZN, GOOGL, MSFT, and NVDA** — using **Python, SQL, and Power BI**. It combines stock market time-series analysis, financial KPI engineering, SQL-based exploration, and dashboard storytelling to compare stock growth, volatility, drawdowns, liquidity, and risk-adjusted returns from **2020 to 2025**.

The project is structured as an end-to-end analytics workflow:
- **Python** for data extraction, cleaning, feature engineering, and KPI calculation
- **SQL** for analytical queries and stock-level comparisons
- **Power BI** for interactive dashboarding and storytelling

---

## Objectives
- Compare the long-term performance of major US tech stocks
- Measure return, risk, drawdown, volatility, and liquidity
- Identify high-growth vs high-risk stocks
- Build an interactive dashboard for stock comparison and trend analysis
- Practice end-to-end analytics using Python, SQL, and Power BI

---

## Tech Stack
- **Python**: pandas, numpy, yfinance, matplotlib
- **SQL**: MySQL
- **Power BI**
- **Jupyter Notebook**

---

## Dataset
Historical stock data was collected using the **yfinance** Python library for the following US tech stocks:

- **AAPL** – Apple
- **AMZN** – Amazon
- **GOOGL** – Alphabet
- **MSFT** – Microsoft
- **NVDA** – NVIDIA

**Time period covered:** 2020–2025

---

## Project Workflow

### 1) Data Collection
Stock price data was downloaded using `yfinance`, including:
- Date
- Open
- High
- Low
- Close
- Volume

The data for all five stocks was combined into a single time-series dataset.

---

### 2) Feature Engineering
Using Python, the following stock market indicators and time-series features were created:

- **Daily Return**
- **20-day Moving Average (MA20)**
- **50-day Moving Average (MA50)**
- **Rolling Volatility**
- **Price Change**
- **Year**

This cleaned and enriched dataset was exported as:

---

### 3) Financial KPI Analysis
A stock-level KPI table was created to compare performance across return, risk, and liquidity dimensions.

The following KPIs were calculated:

- **Annual Return**
- **CAGR (Compound Annual Growth Rate)**
- **Maximum Drawdown**
- **Sharpe Ratio**
- **Average Liquidity**
- **Risk Score**

The final KPI output was saved as:

---

### 4) SQL Analysis
SQL was used to perform stock-level analytical queries such as:

- yearly highest closing price by stock
- one-day percentage gain analysis
- annual volume trends
- stock-level return and ranking comparisons
- grouped summaries using aggregate functions and window functions

SQL queries are available in:


---

### 5) Power BI Dashboard
A **2-page interactive Power BI dashboard** was built to summarize stock performance and time-series trends.

#### Dashboard Pages

### **Page 1 – Performance Overview**
This page compares the five stocks using key return-risk KPIs.

It includes:
- Highest CAGR
- Best Sharpe Ratio
- Lowest Risk Score
- Best Annual Return
- CAGR by Stock
- Risk Score by Stock
- Risk vs Return Trade-off
- KPI comparison table

### **Page 2 – Trend Analysis**
This page focuses on time-series behavior and stock-specific drill-down.

It includes:
- Closing Price Trend by Stock (Yearly)
- Close vs MA20 vs MA50
- Rolling Volatility Trend
- Trading Volume Trend

A ticker slicer is used to drill into trend behavior for a selected stock.

---


## Key Insights

- **NVDA** delivered the highest CAGR and strongest average annual return, but it also showed the highest risk score and one of the deepest drawdowns.
- **AAPL** and **MSFT** demonstrated relatively balanced return-risk profiles with lower drawdowns and more stable long-term performance.
- **AMZN** showed moderate growth but weaker risk-adjusted performance compared to some peers.
- Trend analysis highlighted clear differences in volatility and trading activity across the five stocks over time.



