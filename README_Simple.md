# Apple Sales Analytics Dashboard

## About This Project

I built this project to analyze Apple's global sales data and understand how the business is performing across different countries, products and time periods. The data contains over 1 million sales transactions from 2020 to 2024 across 19 countries and 75 stores worldwide.

I wanted to go beyond just looking at numbers in a spreadsheet. So I built a full interactive dashboard in Power BI where anyone can click and explore the data themselves.

---

## What I Used

- **Power BI** for the dashboard and visualizations
- **Excel** for initial data cleaning and analysis
- **DAX** for writing calculated measures and KPIs
- **Power Query** for transforming and loading data

---

## What The Dashboard Shows

I kept everything on one single page so it's easy to read at a glance. The page is divided into three sections:

**Top Row — KPI Cards**
Six cards showing the most important numbers: total revenue, profit, orders, margin, yearly revenue and monthly revenue. All cards respond dynamically when you use the slicers.

**Middle Row — Trends and Breakdown**
- A line chart showing monthly revenue trends across all 5 years so you can compare how each year performed
- A bar chart showing the top 10 products ranked by revenue
- A donut chart showing how revenue is split across the 10 product categories

**Bottom Row — Geography and Growth**
- A map showing which countries generate the most revenue
- A column chart showing year over year growth with green bars for positive growth and red for decline
- A forecast line chart showing projected revenue from November 2024 to April 2025

---

## What I Found

After analyzing the data these were the most interesting findings:

- Total revenue across 5 years was **$6.17 billion** with a profit of **$2.16 billion**
- Revenue was stable around **$1.26B per year** from 2020 to 2023
- In 2024 revenue dropped by **12.68%** which was the biggest decline in 5 years
- **Apple Music** was the top earning product at **$125M**
- **Tablets** were the biggest category making up **15.46%** of all revenue
- The **United States** was by far the biggest market at **$1.23B**
- **March** was consistently the strongest month every year
- **December** was surprisingly the weakest month which is unusual for a consumer electronics company

---

## Revenue Forecast

Based on historical trends and seasonal patterns I projected the next 6 months of revenue:

| Month | Projected Revenue |
|-------|------------------|
| November 2024 | $104M |
| December 2024 | $105M |
| January 2025 | $107M |
| February 2025 | $97M |
| March 2025 | $108M |
| April 2025 | $104M |

Total 6 month projection: **$624M**

---

## Things I Would Improve

If I had more time or real business data I would look into:

- Why December is so weak and what promotions could fix that
- How to grow in emerging markets like Colombia, Mexico and Thailand which currently contribute less than 3% combined
- Whether bundling subscription services like Apple Music and iCloud could increase overall profit margins since subscriptions have the highest margins

---

## How To Run This Project

1. Download all files from this repository
2. Extract FactSales.zip to get the main data file
3. Open Apple_Sales_Dashboard.pbix in Power BI Desktop
4. Update the data source path to wherever you saved the files
5. Click Refresh and the dashboard will load

---

## Note

This is a portfolio project I built to practice data analytics and Power BI. The dataset is based on simulated Apple sales data.
