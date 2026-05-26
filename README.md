# Swiggy Sales Performance Dashboard

An interactive Excel-based dashboard built to analyze Swiggy's food delivery sales data across cities, food categories, time periods, and customer segments. The dashboard is designed around three connected views - Dashboard, Analysis, and Data with a dynamic filter panel that drives all visuals simultaneously.


<img width="1280" height="720" alt="Dashboard" src="https://github.com/user-attachments/assets/4517b1e4-f212-4793-bc54-ee1f5ad09e7b" />




## What's Inside

The workbook has three navigable pages:

**Dashboard** — The primary view. Displays all KPIs and charts at a glance. This is where you'll spend most of your time exploring the data.

**Analysis** — A deeper breakdown page, focused on filtered segmentation. Use this when you want to isolate specific categories, price ranges, or rating buckets and compare their performance side by side.

**Data** — The raw data table behind the entire dashboard. All visuals are driven from this sheet.


## KPI Cards

Five summary cards sit across the top of the dashboard. They update automatically based on whatever filters are active:

<p align="center"><img width="1206" height="120" alt="kpi" src="https://github.com/user-attachments/assets/d94d1ae9-2154-41ab-8628-f148c7435c65" />


| KPI | Description |
|---|---|
| **Total Sales** | Sum of revenue across all filtered orders (in ₹ Millions) |
| **Average Rating** | Mean customer rating for the filtered dataset |
| **Avg Order Value** | Total Sales ÷ Total Orders |
| **Users** | Total unique users in the filtered segment (in Millions) |
| **Total Orders** | Count of orders matching active filters (in Thousands) |

When no filters are applied, the full dataset reads: ₹53.01M in Total Sales, 4.34 Average Rating, ₹268.51 Avg Order Value, 5.59M Users, and 197.43K Total Orders.


## Charts & Visuals

**Monthly Sales Trend** — A line chart showing sales movement from January through August. Useful for spotting seasonal peaks and dips across the year. 

<p align="center"><img width="526" height="231" alt="Monthly_sales" src="https://github.com/user-attachments/assets/e39eac16-07a5-4f8e-a944-03f6c8ff3652" />


**Daily Sales Trends** — A bar chart broken down by day of the week (Mon - Sun). Helps identify which days consistently drive higher order volumes and revenue.

<p align="center"><img width="520" height="232" alt="Daily_sales" src="https://github.com/user-attachments/assets/e1c3688b-cf1b-48e8-9dde-41a5d660d9f4" />


**Sales by Food Type** — A donut chart splitting orders between Vegetarian and Non-Vegetarian. In the full dataset, Non-Veg accounts for roughly 66% of sales, Veg at 34%.

<p align="center"><img width="267" height="223" alt="sales_by_food" src="https://github.com/user-attachments/assets/133edd04-2a58-4b57-b404-b08c1f843105" />


**Quarterly Sales and Orders** — A summary table showing Q1, Q2, and Q3 figures for both revenue and order count. At full scope: Q1 ₹17.53M / 64.6K orders, Q2 ₹17.75M / 65.5K orders, Q3 ₹11.95M / 44.2K orders.

<p align="center"><img width="271" height="227" alt="Quaterly_trends" src="https://github.com/user-attachments/assets/6c99757f-be52-47c6-8ccd-626e980ac7ba" />


**Top 5 Cities by Sales** — A horizontal bar chart ranking the highest-grossing cities. Bengaluru leads consistently, followed by Lucknow, Mumbai, Hyderabad, and Ahmedabad (with city rankings shifting slightly based on active filters).

<p align="center"><img width="415" height="222" alt="City_sales" src="https://github.com/user-attachments/assets/909aeb0d-2fc1-4f27-afad-3e1643742472" />


**Sales by State** — A filled map of India showing state-level sales distribution using a colour gradient. Bing Maps integration renders the geographic spread visually.

<p align="center"><img width="385" height="463" alt="Screenshot 2026-05-26 230131" src="https://github.com/user-attachments/assets/af3e5611-bf69-4fd9-a641-8b88d9d7ea2f" />


**Weekly Sales Trend** — A daily bar chart across approximately 36 weeks, showing granular week-by-week fluctuation in revenue.

<p align="center"><img width="780" height="231" alt="weekly_sales" src="https://github.com/user-attachments/assets/a5c44402-bea5-4d0e-8b4b-c9e078ee2a54" />



## Filter Panel

The left sidebar contains four independent slicers. They can be used individually or stacked together:

**Months** — Jan through Sep (presented as a grid). Click one or multiple months to narrow the time window.

<p align="center"><img width="292" height="152" alt="month" src="https://github.com/user-attachments/assets/03d58505-045b-41b6-97ab-b959b9943684" />


**Category** — A scrollable list of food item categories (e.g., Desi Ghee Sweets, Chinese, Pasta, Pizza, Biryani, Cakes, Rolls, etc.). Multiple selections are supported.
  
  <p align="center"><img width="295" height="152" alt="category" src="https://github.com/user-attachments/assets/4f3f86cc-a56c-488a-8275-34d24775bd5b" />


**Price Range** — Segments orders by item price bucket: ₹0–₹100, ₹100–₹200, ₹200–₹300, ₹300–₹400, ₹400–₹500, ₹500–₹600, ₹700–₹800, ₹800-Above.

<p align="center"><img width="292" height="148" alt="price" src="https://github.com/user-attachments/assets/ffe851c8-fc14-4a70-ae0d-d1047a999fea" />


**Rating Category** — Filters by customer satisfaction tier: High Rating, Average Rating, or Low Rating.

<p align="center"><img width="292" height="152" alt="rating" src="https://github.com/user-attachments/assets/d6f61630-0e0f-4d8b-ab3a-f625ae1e476e" />


All slicers are connected to every chart and KPI card on the page.


## How to Use

1. Open `Swiggy Dashboard.xlsb` in Microsoft Excel (2016 or later recommended for full slicer and map support).
2. Navigate to the **Dashboard** tab to start exploring.
3. Click any filter in the left panel to apply it. The KPIs and all charts update instantly.
4. Hold `Ctrl` and click to select multiple items within the same slicer.
5. Use the clear filter button on each slicer header to reset individual filters.
6. Switch to the **Analysis** tab for a more focused breakdown, or **Data** to inspect raw records.

   <p align="center"><img width="462" height="134" alt="Slicer" src="https://github.com/user-attachments/assets/c5c3ee50-bbff-4eb8-9ecc-77bb9cb9b2bc" />



## File Structure

```
Swiggy Dashboard.xlsb
├── Dashboard       ← Main view with KPIs, charts, slicers
├── Analysis        ← Secondary breakdown view
└── Data            ← Source data table
```



## Requirements

- Microsoft Excel 2016 or later
- Bing Maps add-in enabled (for the Sales by State map visual)
- Macros are not required — the dashboard runs entirely on native Excel slicers and PivotCharts



## Data Coverage

- Time period: January – December (Q1 to Q3)
- Cities covered: Bengaluru, Lucknow, Mumbai, Hyderabad, Ahmedabad, Chandigarh, Kolkata, Chennai, Jaipur, New Delhi, and others
- Food categories: Covers the full Swiggy menu taxonomy including combo deals, new launches, price-tier items, and cuisine types
- Order price range: ₹0 to ₹800+

