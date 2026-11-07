# Devixo-Solution-Data-Science-Task-3# 📊 Superstore Sales - Business Intelligence & Dashboard Development

### Devixo Solutions - Summer Internship
### Week 3 - Task 03 | Data Science Internship

 Transform raw business data into actionable insights by creating an interactive dashboard and presenting business recommendations.


## 📌 Project Overview

This project analyzes **Superstore Sales data (2014-2017)** containing **9,994 records** to understand sales performance, profit, customer behavior, regional trends, and category performance.

The goal is to convert raw data into a decision-ready dashboard that helps management understand:
- Where is profit coming from?
- Where are we losing money?
- Which products, customers, and regions are most valuable?

**Tool Used:** Power BI Desktop
**Dataset:** Superstore Sales (Business Dataset - 9,994 Rows)

---

## 🛠️ Technologies Used

- **Power BI** - Dashboard, Report & Map
- **DAX** - KPI Calculation, Measures
- **Python / Pandas** - Data Cleaning & Feature Engineering (Bonus)
- **SQL** - Data Querying & Validation
- **Excel** - Data Validation
- **Power Query** - Data Cleaning & Transformation

---

## 📂 Dataset

**Source:** Superstore Sales Dataset
**Records:** 9,994 (Requirement: At least 5,000 ✅)
**Period:** 2014 - 2017
**Columns Used:**
`Order Date, Region, State, City, Category, Sub-Category, Product Name, Sales, Quantity, Profit, Customer Name, Segment, Ship Mode, Discount`

### Data Cleaning Done:
1. Removed null / duplicate values
2. Fixed Date format (Order Date)
3. Created new columns: `Order Year`, `Order Month`, `Profit Margin`
4. Removed extra spaces in Category / State names
5. Validated Sales, Profit, Quantity totals

### Feature Engineering:
- `Profit Margin = Profit / Sales`
- `Order Year = YEAR(Order Date)`
- `Order Month = MONTH(Order Date)`
- `Sales per Quantity = Sales / Quantity`

### KPIs Created (DAX):
- `Total Sales = SUM(Sales)`
- `Total Profit = SUM(Profit)`
- `Total Quantity = SUM(Quantity)`
- `Profit Margin = DIVIDE(Total Profit, Total Sales)`
- `Avg Order Value`

---

## 📈 Key KPIs

| KPI | Value |
| :--- | :--- |
| **Total Sales** | **1,064,046.04** |
| **Total Profit** | **120,000.72** |
| **Total Quantity** | **17,407** |
| **Profit Margin** | **11.28%** |

---

## 📄 Dashboard Structure - 3 Pages

### Page 1: Dashboard (Overview)
- Total Sales, Total Profit, Total Quantity, Profit Margin
- Monthly Sales Trend (2014-2017)
- Sales by Category - Donut Chart
- Sales by Sub-Category - Bar Chart
- Sales by Region - Bar Chart
- Sales by Segment - Donut Chart

### Page 2: Report (Deep Dive Analysis)
- **Sales by Sub-Category** - Treemap
- **Sales by Region** - Pie Chart
- **Profit by Segment** - Bar Chart
- **Matrix Table** - Category x Region: Sum of Quantity & Sum of Profit
- **Shipping Days** Analysis
- **Region Slicer** - Central, East, South, West

### Page 3: Map (Sales BY State Map)
- Interactive US Map - Sales BY State
- Tooltip on Hover: State, Profit, Quantity, Top Product, Region, Profit Margin
- Region Slicer for filtering
- Drill-down from Country -> Region -> State

**Example Tooltips:**
- New York (East): Profit 32,116.52 | Quantity 1990
- Minnesota (Central): Profit 4,144.37 | Quantity 209
- Montana (West): Profit 1,631.55 | Quantity 22
- Idaho (West): Profit 274.73 | Quantity 16

---

## 💡 15 Business Insights

1. Total Sales is 1,064,046.04 but profit is only 120,000.72 (11.28% margin) - cost is high.
2. Technology is the leading category with 38.48% sales (406.5K).
3. Furniture is 2nd with 31.07% (330.5K), Office Supplies is 3rd.
4. Phones are the top-selling sub-category, followed by Chairs & Machines.
5. Labels, Envelopes, Art & Fasteners have the lowest sales.
6. Sales were unstable in 2014-2016, with strong peak growth in 2017.
7. West region is No.1 with 35.95% sales, followed by East 33.75%.
8. South is the weakest region with only 12.51% sales.
9. Consumer segment drives 50.64% of total sales - main customer.
10. Corporate contributes 28.78% and Home Office 20.56%.
11. Consumer segment is also the most profitable (~65K profit).
12. Furniture in Central region is in LOSS: -1,649.71.
13. Furniture in East region is also in LOSS: -423.01.
14. Technology in West is most profitable: 18,659.55 profit.
15. New York is the top state with 32,116.52 profit, while small states like Idaho have very low profit (274.73).

---

## ✅ 10 Business Recommendations

1. **Focus on Technology:** Invest more in Phones, Machines & Accessories - highest sales & profit.
2. **Fix Furniture Loss:** Review pricing & shipping cost for Furniture in Central & East region.
3. **Grow South Region:** Launch targeted marketing & discounts in South (lowest 12.51%).
4. **Retain Consumers:** Create loyalty program for Consumer segment (50.64% sales).
5. **Expand in New York:** New York is star state - increase stock & fast delivery there.
6. **Remove / Bundle Low Sellers:** Bundle Labels, Envelopes & Fasteners with high sellers instead of selling alone.
7. **Control Discount:** High discount is killing profit - set max discount limit, especially on Furniture.
8. **Improve 2017 Momentum:** 2017 growth was best - repeat same product & promotion strategy.
9. **Develop Corporate Clients:** Corporate gives 28.78% - offer B2B bulk deals to grow it to 35%.
10. **Use State Map for Planning:** Open warehouses near high-sales states (NY, CA) to reduce shipping days & cost.

---

## 📋 Executive Summary

The Superstore business is growing in sales but struggling in profit margin. With 1.06M sales and only 120K profit, the company needs to shift focus from sales volume to profitable sales.

Technology, Consumer segment, West & East regions, and New York state are the growth engines. Furniture in Central/East and South region are the weak points.

If the company fixes Furniture pricing, controls discounts, and invests in Technology & South region, profit margin can improve from 11.28% to 15%+ in the next year.

---

## 🚀 How To Use This Project

1. Download / Clone this repository
2. Open `Superstore 5000.pbix` in Power BI Desktop
3. Click Refresh if data source asks
4. Navigate Pages: `Dashboard` -> `Report` -> `Map`
5. Use Region Slicer on top to filter by Region
6. Hover on Map to see State-level details

---

## 📁 File Structure
