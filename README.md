# Sales Performance Dashboard

**Internship Project — Task 1: Sales Performance Dashboard**
Kinetrexa Software Pvt. Ltd. | Data Analytics Internship

Analysis of a real-world retail sales dataset to uncover revenue trends,
top-performing products, customer purchasing behavior, and regional sales
performance, delivered as an interactive Excel dashboard.

## Dataset

**Sample Superstore** — US retail order data (2015–2018), 9,994 clean order
line items after data cleaning, covering Consumer, Corporate, and Home
Office customer segments across Furniture, Office Supplies, and Technology
categories.

## Project Structure

```
sales-dashboard/
├── data/
│   ├── superstore_raw.csv        # Original dataset
│   └── superstore_clean.csv      # Cleaned dataset (output of notebook)
├── notebooks/
│   └── Sales_Performance_Dashboard.ipynb   # Full analysis notebook
├── dashboard/
│   └── Sales_Performance_Dashboard.xlsx    # Interactive Excel dashboard
├── reports/
│   ├── kpi_summary.csv
│   ├── monthly_trend.csv
│   ├── yearly_growth.csv
│   ├── category_performance.csv
│   ├── subcategory_performance.csv
│   ├── top_products.csv
│   ├── regional_performance.csv
│   ├── state_performance.csv
│   ├── segment_performance.csv
│   ├── top_customers.csv
│   └── ship_mode_performance.csv
├── visuals/                      # Exported chart images
└── Sales_Performance_Insights_Report.pdf
```

## What Was Done

1. **Data Cleaning & Preprocessing** — removed blank/incomplete rows, fixed
   data types (dates, numerics), removed duplicates, engineered features
   (Profit Margin %, Ship Days, Order Month/Year).
2. **Sales KPI Analysis** — Total Sales, Total Profit, Profit Margin,
   Average Order Value, Total Orders, Units Sold.
3. **Interactive Charts** — monthly trend, category/sub-category
   breakdown, regional performance, discount-vs-margin relationship,
   customer segment share.
4. **Regional Sales Analysis** — performance by Region and State.
5. **Product Performance** — best and worst performing categories,
   sub-categories, and individual products.
6. **Business Insights** — see the full report for details and
   recommendations.

## How to Run

```bash
cd notebooks
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook Sales_Performance_Dashboard.ipynb
```

Open `dashboard/Sales_Performance_Dashboard.xlsx` in Excel to explore the
interactive dashboard — KPI cards recalculate live, and the Raw Data tab
has filterable columns (Region, Category, Segment, etc.).

## Key Findings (summary — full detail in the PDF report)

- Revenue grew from ~$484K (2015) to ~$733K (2018), with a consistent Q4
  seasonal spike each year.
- The **Tables** sub-category is a net loss-maker despite $200K+ in sales,
  driven by heavy discounting.
- Profit margin trends toward zero/negative once discounts exceed ~20%.
- **West** and **East** regions lead in both sales and profit margin;
  **Central** lags with under 8% margin.
- **Home Office** customers have the highest average order value.

## Author

Himesh Khare — Data Analytics Intern, Kinetrexa Software Pvt. Ltd.
