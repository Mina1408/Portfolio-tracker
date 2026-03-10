# Portfolio-tracker
Real-time stock portfolio monitoring with drift detection and Google Sheets dashboard
---
# Automated Portfolio Tracker

> Real-time stock portfolio monitoring system with drift detection and automated Google Sheets dashboard

**[🔗 View Live Dashboard](https://docs.google.com/spreadsheets/d/1sDtTYVAEHsS9N7Qc_DrYftNKr1XrlJRMezkLJp7ABQQ)**

---

##  Problem Statement

Manual portfolio tracking is time-consuming and error-prone, leading to:
- Outdated performance metrics
- Missed rebalancing opportunities  
- Manual data entry errors
- Lack of real-time insights

**Solution:** Automated system that fetches live prices, calculates metrics, and updates a Google Sheets dashboard.

---

##  Key Features

-  **Real-time price fetching** via yfinance API
-  **P&L calculation** (dollars and percentage)
-  **Allocation drift detection** (5% threshold alerts)
-  **Automated Google Sheets updates**
-  **Rebalancing alerts** for portfolio management
-  **Error handling** for API failures

---

##  Demo Output
```
 PORTFOLIO SUMMARY
================================================================================
Total Cost Basis:    $26,300.00
Current Value:       $27,355.90
Total P&L:           $1,055.90 (+4.01%)

 REBALANCING ALERTS
================================================================================
 NVDA: UNDERWEIGHT by 13.30% (Current: 20.03%, Target: 33.33%)
 CAT: OVERWEIGHT by 18.19% (Current: 51.53%, Target: 33.34%)
```

**Sample Dashboard:**

| Ticker | Shares | Cost Basis | Current Price | Current Value | P&L ($) | P&L (%) | Allocation |
|--------|--------|------------|---------------|---------------|---------|---------|------------|
| KO     | 100    | $60.00     | $77.80        | $7,780        | +$1,780 | +29.67% | 28.44%     |
| NVDA   | 30     | $450.00    | $182.65       | $5,479        | -$8,020 | -59.41% | 20.03%     |
| CAT    | 20     | $340.00    | $704.82       | $14,096       | +$7,296 | +107.30%| 51.53%     |

---

##  Tech Stack

- **Python 3.8+** - Core programming language
- **pandas** - Data manipulation and analysis
- **yfinance** - Yahoo Finance API for stock prices
- **gspread** - Google Sheets API integration
- **Google Colab** - Development environment
