# Retail Sales Power BI — KPI Definitions

The source CSV contains order, customer, segment, geography, channel, product, sales, cost, and payment fields.

## Recommended DAX measures

Confirm the model table name before using these examples.

```dax
Total Sales =
SUM('Retail_Sales_Analysis_Dataset'[Sales])

Total Profit =
SUM('Retail_Sales_Analysis_Dataset'[Profit])

Total Orders =
DISTINCTCOUNT('Retail_Sales_Analysis_Dataset'[Order ID])

Profit Margin % =
DIVIDE([Total Profit], [Total Sales], 0)

Units Sold =
SUM('Retail_Sales_Analysis_Dataset'[Quantity])
```

Format `Profit Margin %` as Percentage in the model. Do not multiply by 100 again when using percentage formatting.

## Model and report checks

1. Set `Order Date` to the Date data type.
2. Use a dedicated Date table for time intelligence when the report requires it.
3. Mark the Date table as the model's date table and create a relationship to the sales fact table.
4. Use distinct count for order IDs.
5. Check that all KPI cards respond to Region, Category, and Date slicers as intended.
6. Reconcile total sales and profit to the source CSV after refresh.
7. Confirm that monthly trends sort by date, not alphabetically by month label.

## Metric interpretation

Profit Margin % = Total Profit / Total Sales. Calculate this measure from totals in the current filter context. It is not the average of individual row-level profit percentages.

The CSV is a portfolio practice dataset. Validate the source and model before presenting numerical conclusions as project findings.
