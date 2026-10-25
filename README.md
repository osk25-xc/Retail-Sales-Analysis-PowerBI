# Retail Sales Analysis | Power BI Dashboard

An interactive Power BI dashboard project for reviewing retail sales, profitability, order volume, product performance, and regional trends.

## Business Objective
Present key sales KPIs in a single report and let users explore results by date, region, and category.

## Dashboard Features
- Total Sales
- Total Profit
- Total Orders
- Profit Margin %
- Daily sales trend
- Sales by category and region
- Top products by sales
- Interactive slicers for filtering

## Tools & Technologies
- Power BI Desktop
- Power Query for data preparation
- DAX for measures
- CSV / Excel source data

## Example DAX Measures
```dax
Total Sales = SUM('Retail_Sales_Analysis_Dataset'[Sales])
```

```dax
Total Profit = SUM('Retail_Sales_Analysis_Dataset'[Profit])
```

```dax
Total Orders = DISTINCTCOUNT('Retail_Sales_Analysis_Dataset'[Order ID])
```

```dax
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
```

Check that the table and column names match your model before using these measures.

## How to Use
1. Download the `.pbix` file and source dataset if included.
2. Open the report in Power BI Desktop.
3. Review KPI cards and charts.
4. Use slicers to compare the selected periods, regions, and categories.

## Business Questions
- How are sales and profit trending over time?
- Which categories and regions contribute most?
- Which products lead sales?
- How does profitability compare with sales volume?

## Notes
This is a portfolio reporting project. Verify the files present in the repository and refresh the model if the source data changes. No real-company impact is claimed.

## Skills Demonstrated
Power BI · Power Query · DAX · KPI design · Interactive dashboards · Business intelligence

---
Created by **Omkar S. Kshirsagar** | [GitHub Profile](https://github.com/osk25-xc)
