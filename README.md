# Apple Sales Analytics Dashboard
### From Raw Data to Executive Intelligence — A Complete End-to-End Analytics Project

---

## Why I Built This

As a student learning data analytics I wanted to go beyond tutorials and build something real. I chose Apple sales data because Apple is one of the most recognized brands in the world and their product portfolio is diverse enough to make the analysis genuinely interesting.

The challenge I set myself was simple:

> "Can I take over 1 million rows of raw sales data and turn it into something an executive could actually use to make business decisions?"

After weeks of work the answer is yes. This is that project.

---

## Project Summary

| Detail | Info |
|--------|------|
| Dataset Size | 1,040,200 transactions |
| Time Period | January 2020 — November 2024 |
| Countries | 19 worldwide |
| Stores | 75 global locations |
| Products | 89 Apple products |
| Categories | 10 product categories |
| Tools | Power BI, Excel, DAX |
| Dashboard Type | Single page interactive |

---

## Project Structure

```
Apple-Sales-Analytics
├── Apple_Sales_Dashboard.pbix
├── Apple_Sales_Analytics_Report.xlsx
├── DAX_Measures.txt
├── AppleLight_Theme.json
├── Dashboard_Preview.png
├── README.md
└── Data
    ├── FactSales.zip
    ├── DimProduct.csv
    ├── DimStore.csv
    ├── DimDate.csv
    └── ForecastData.csv
```

---

## Data Architecture

I built a proper Star Schema data model — the same architecture used by professional data engineers in large companies.

```
                    DimDate
                       │
DimProduct ────── FactSales ────── DimStore
                       │
                  ForecastData
```

Why Star Schema?
- Faster query performance
- Cleaner relationships
- Easier DAX calculations
- Industry standard approach

---

## Dashboard Design

I made a deliberate decision to keep everything on one single page. In my experience looking at real dashboards the best ones don't make you click through multiple pages. Everything important is visible at once.

The page is divided into three clear zones:

---

### Zone A — The Numbers That Matter Most

Six dynamic KPI cards sit at the top of the dashboard. Every single one responds to the slicers so when a manager filters by country or year the cards instantly update.

| Card | What It Shows |
|------|--------------|
| Revenue | Total sales revenue |
| Profit | Total gross profit |
| Orders | Number of transactions |
| Margin | Gross profit percentage |
| Year Revenue | Revenue for selected year |
| Month Revenue | Revenue for selected month |

---

### Zone B — Understanding Trends and Performance

**Monthly Revenue Trend (Line Chart)**
Five colored lines — one per year — plotted across 12 months. This single visual immediately answers the question "how does this year compare to last year month by month?" The answer is that all years tracked remarkably close to each other until 2024 when a sharp decline appeared.

**Top 10 Products by Revenue (Bar Chart)**
Horizontal bars sorted from highest to lowest. Apple Music surprisingly topped the list ahead of hardware products which challenged my initial assumption that iPhones would dominate.

**Revenue by Category (Donut Chart)**
Ten slices showing the revenue split. Tablets lead at 15.46% followed closely by Accessories at 15.04%. The near equal distribution across categories shows Apple's deliberate strategy of building a balanced product ecosystem.

---

### Zone C — Geography, Growth and the Future

**Revenue by Country (Map)**
Bubble map showing 19 countries with bubble size representing revenue. The USA dominates but the presence of strong bubbles in Asia Pacific shows Apple's global reach.

**Growth Rate Analysis (Column Chart)**
Red and green bars showing year over year growth. The red bar for 2024 at -12.68% is the single most important insight in the entire dashboard. Everything else was flat or marginally growing. 2024 broke that pattern significantly.

**Revenue Forecast 2025 (Line Chart)**
A solid blue line for historical actuals transitions into a dashed orange line for the 6 month forecast. I used seasonality indexing and trend extrapolation to build the model. The projected total for November 2024 to April 2025 is $624.8 million.

---

## Key Findings

### The Good News
- $6.17B total revenue over 5 years
- Consistent 35% profit margin throughout
- 1,040,200 transactions processed
- Strong presence in 19 countries
- Apple Music outperforming all hardware
- Balanced revenue across 10 categories

### The Concerning News
- 2024 revenue declined 12.68% YoY
- Q4 is consistently the weakest quarter
- December is the weakest month
- 5 countries drive 62% of all revenue
- Emerging markets virtually untapped

---

## Revenue Performance By Year

| Year | Revenue | YoY Growth |
|------|---------|------------|
| 2020 | $1.27B | — |
| 2021 | $1.26B | -0.4% |
| 2022 | $1.27B | +0.4% |
| 2023 | $1.26B | -0.6% |
| 2024 | $1.10B | -12.7% |

---

## Top 10 Products

| Rank | Product | Revenue |
|------|---------|---------|
| 1 | Apple Music | $125.45M |
| 2 | iMac 27-inch | $124.01M |
| 3 | iPad mini (5th Gen) | $123.95M |
| 4 | iPad (9th Gen) | $123.95M |
| 5 | Beats Fit Pro | $118.45M |
| 6 | MacBook Air (Retina) | $118.11M |
| 7 | AirPods (3rd Gen) | $118.08M |
| 8 | iPad Pro (M2) | $116.03M |
| 9 | iPad Pro 11-inch | $114.06M |
| 10 | MacBook Air (M1) | $113.20M |

---

## Top Markets

| Country | Revenue | Share |
|---------|---------|-------|
| United States | $1.23B | 20.0% |
| Australia | $577M | 9.4% |
| China | $575M | 9.3% |
| Japan | $496M | 8.0% |
| UAE | $412M | 6.7% |
| Canada | $411M | 6.7% |
| United Kingdom | $329M | 5.3% |
| France | $326M | 5.3% |

---

## 6-Month Revenue Forecast

| Period | Projected Revenue |
|--------|------------------|
| November 2024 | $104.3M |
| December 2024 | $105.7M |
| January 2025 | $106.6M |
| February 2025 | $96.8M |
| March 2025 | $107.7M |
| April 2025 | $103.7M |
| 6-Month Total | $624.8M |

Forecast methodology: Historical seasonality index x annual trend rate (-0.21% per year)

---

## Business Recommendations

Based on my analysis here is what I would recommend if this were a real business situation:

**1. Investigate the 2024 decline urgently**
A 12.68% drop after 4 stable years is a serious signal. This needs root cause analysis — is it pricing, competition, market saturation or something else?

**2. Fix the Q4 holiday problem**
December being the weakest month for an electronics company is counterintuitive. A focused holiday campaign could add $50M+ in revenue.

**3. Bundle subscription services**
Apple Music, iCloud and Apple TV+ have near-100% profit margins. Bundling them as Apple One and cross-selling to hardware buyers could significantly improve overall profitability.

**4. Invest in emerging markets**
Colombia, Mexico and Thailand combined contribute less than 3% of revenue despite having active stores. Localized pricing and marketing could unlock $200M+ in new revenue.

**5. Reduce geographic concentration risk**
Five countries generating 62% of revenue creates significant business risk. Diversifying revenue across more markets would make the business more resilient.

---

## Technical Highlights

**DAX Measures Written:**
- Time intelligence (YoY, MoM, YTD)
- Dynamic KPI cards with slicer awareness
- Revenue forecasting with seasonality
- Pareto and ranking calculations
- Conditional formatting measures

**Data Modeling:**
- Star schema with 4 dimension tables
- Active relationships across all tables
- Custom date table for time intelligence
- Optimized for Power BI performance

**Dashboard Design:**
- Custom Apple Light theme
- Consistent color palette throughout
- Responsive to all 4 slicers simultaneously
- Single page layout for executive use

---

## How To Use This Project

Requirements: Power BI Desktop (free download from Microsoft)

```
1. Clone or download this repository
2. Extract FactSales.zip in the Data folder
3. Open Apple_Sales_Dashboard.pbix
4. Click Transform Data and update file paths
   to point to your Data folder location
5. Click Close and Apply
6. Click Refresh on the Home tab
7. Explore the dashboard
```

---

## What I Learned

This project taught me things that no tutorial ever could:

- Real data is messy and cleaning it properly takes longer than the analysis
- The data model you build at the start determines how easy or hard everything else is
- DAX time intelligence only works when your date table relationships are correct
- The best dashboards tell a story not just display numbers
- Business insights matter more than technical complexity

---

## Disclaimer

This project uses simulated sales data for educational and portfolio purposes. Apple Inc. brand names and product names are trademarks of Apple Inc. This project has no affiliation with Apple Inc.

---

Built with curiosity, persistence and a lot of DAX debugging
