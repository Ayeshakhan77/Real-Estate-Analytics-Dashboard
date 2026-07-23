# 🏡 Real Estate Analytics Dashboard
**DataBuzz Power BI Challenge | Advanced Property Market Intelligence**

<p align="center">
  <img src="Real_estate.png" alt="UK Real Estate Dashboard" width="1000">
</p>

## Overview
An 8-page interactive Power BI dashboard analysing the complete UK residential property market — from lead generation and transaction analysis through to rental investment viability, mortgage affordability, and market anomaly detection. Built on 8 interconnected tables with advanced DAX, inactive relationships, disconnected parameter tables, and dynamic field-based metric switching.

---

## Dashboard Pages

| # | Page | Key Analysis |
|---|------|-------------|
| 1 | Executive Summary | Market Temperature Score, Rolling 12M Price Trend, YoY Momentum |
| 2 | Transaction Analysis | Listing vs Transaction Date Revenue, Pipeline Lag, Status Breakdown |
| 3 | Agent & Agency Performance | Conversion Rate, Percentile Banding, DOM vs Benchmark, Seniority Analysis |
| 4 | Buyer Funnel & SDLT | Lead Funnel, SDLT by Buyer Type, Conversion Rate by Segment |
| 5 | Mortgage & Rate Scenarios | Live Rate Modelling, DSCR Banding, Affordability Risk by Region |
| 6 | Dynamic Metric Explorer | 10-metric switchable dashboard via Field Parameters |
| 7 | Rental & Investment | Gross/Net Yield, DSCR Heatmap, EPC Premium Analysis |
| 8 | Market Intelligence & Anomalies | Z-Score Outlier Detection, New Build %, Price Per SqFt |

---
## Key Insights

- **Avg listing-to-sale pipeline:** 66.8 days across all regions
- **London premium:** Highest Price-to-Income ratio — affordability risk RED zone
- **Top performing channel:** First Time Buyers show highest lead conversion rate
- **EPC premium:** A-rated properties command measurably higher average sale prices
- **DSCR reality check:** At current rates (5.25% base), all property types show Cashflow Negative DSCR — highlighting the BTL squeeze in UK market
- **Market temperature:** South East and London consistently Seller's Market conditions
- **Anomaly detection:** 82 price outliers identified via Z-Score (>±2.5σ from regional mean)
- **New Build share:** 10.14% of total transactions — below national target

---

## Advanced Features

| Feature | Implementation |
|---------|---------------|
| Dual date analysis | USERELATIONSHIP (inactive relationship) |
| 10-metric dynamic page | Field Parameters + SELECTEDVALUE/SWITCH |
| Live rate modelling | Disconnected DIM_RateScenario + SELECTEDVALUE |
| Tiered SDLT | Multi-tier DAX with FTB relief + 3% / 2% surcharges |
| Z-Score anomalies | STDEVX.P with ALLEXCEPT regional context |
| Agent percentile bands | RANKX with ALLSELECTED + ratio banding |
| Market Temperature | Composite 4-signal score (0–100) |
| DSCR heatmap | Numeric rules-based conditional formatting |
| Affordability risk color | Price-to-Income ratio with RAG thresholds |
| EPC green premium | A→F sorted via Power Query custom sort column |

---

## Tech Stack

| Tool | Usage |
|------|-------|
| Microsoft Power BI Desktop | Dashboard development |
| DAX | All measures and calculations |
| Power Query (M) | Data loading, sort columns |
| Excel (.xlsx) | Source data — 8 sheets |
| Bing Maps | UK geographic intelligence |

---
## Disclaimer

> This dashboard is built on simulated training data for educational purposes only; values do not represent real organisational data.

---

## Acknowledgements

Built as part of the **DataBuzz UK Real Estate Power BI Challenge** — a community-driven analytics competition focused on production-grade dashboard development and advanced DAX.


