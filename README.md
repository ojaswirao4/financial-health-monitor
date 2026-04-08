# Corporate Financial Health Monitor

Financial due diligence style analysis of Indian equities using Python, SQL, Excel, and Power BI.

---

## Overview

This project analyzes the financial health of major Indian companies using real market data. It evaluates companies based on profitability, growth, leverage, and valuation to identify strong performers, risky companies, and potential investment opportunities.

The overall workflow is designed to resemble financial due diligence performed in consulting and advisory roles.

---

## Problem Statement

Analyzing multiple companies across sectors can be time-consuming and inconsistent when done manually. There is a need for a structured approach that can:

* Consolidate financial data
* Standardize evaluation metrics
* Highlight risks and opportunities clearly

---

## Data Collection

A hybrid approach was used:

* Company list (NIFTY 50) was scraped from Wikipedia using Beautiful Soup
* Financial data was retrieved using the yfinance library

This approach was chosen because most financial websites restrict scraping, while APIs provide more reliable and structured data.

---

## Tools & Technologies

* Python (Pandas, NumPy)
* Beautiful Soup (web scraping)
* yfinance (financial data extraction)
* SQL (DuckDB)
* Excel (financial reporting)
* Power BI (dashboard visualization)

---

## Methodology

### Data Collection

Collected company names, symbols, and sectors through web scraping, and financial metrics such as revenue, margins, ROE, debt, and growth using an API.

### Data Cleaning

Handled missing values, standardized metrics, and prepared the dataset for analysis.

### Feature Engineering

Created additional indicators including:

* PEG Ratio
* Earnings Quality Score
* Leverage Risk Category
* Valuation Tag (Undervalued / Fair / Overvalued)
* Growth Tag

### Financial Health Scoring

Developed a composite score (0–100) based on:

* Profitability
* Return ratios
* Leverage
* Valuation
* Growth

Companies were categorized into Strong, Moderate, and Weak groups.

### SQL Analysis

Performed business-focused analysis such as:

* Identifying top-performing companies
* Sector-wise benchmarking
* Detecting high-risk companies
* Finding undervalued opportunities
* Ranking companies within sectors

### Reporting

* Excel was used to create a financial summary
* Power BI was used to build an interactive dashboard

---

## Key Insights

* Financial sector companies showed consistently strong performance
* High leverage was a major risk factor in weaker companies
* Some companies were undervalued despite strong fundamentals
* Growth combined with profitability was a strong indicator of financial strength

---

## Output

* Clean dataset with financial metrics
* Financial health score for each company
* SQL analysis outputs
* Excel report
* Power BI dashboard

---

## Project Structure

```id="h2k8mz"
financial-health-monitor/
│
├── data/
│   └── clean_financial_data.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── sql/
│   └── queries.sql
│
├── excel/
│   └── report.xlsx
│
├── powerbi/
│   ├── dashboard.pbix
│   └── dashboard.pdf
│
└── README.md
```

---

## Conclusion

This project demonstrates how financial data can be transformed into structured insights using a combination of data collection, analysis, and visualization tools.

The workflow reflects real-world financial analysis practices used in consulting, investment analysis, and advisory roles.

## Future Improvements

* Expand to more companies
* Include historical trend analysis
* Add predictive modeling
* Automate data pipeline
