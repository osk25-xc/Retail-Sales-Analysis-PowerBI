# Retail Sales Analysis | Power BI

A Power BI portfolio project for exploring retail sales and profitability with a business-focused report.

## Project objective

Prepare a report that helps users review sales performance and compare results across dates, regions, categories, and products.

## Intended KPI measures

The following DAX examples assume the model table is named `Retail_Sales_Analysis_Dataset`. Change the table or column names if your model differs.

```dax
Total Sales =
SUM('Retail_Sales_Analysis_Dataset'[Sales])

Total Profit =
SUM('Retail_Sales_Analysis_Dataset'[Profit])

Total Orders =
DISTINCTCOUNT('Retail_Sales_Analysis_Dataset'[Order ID])

Profit Margin % =
DIVIDE([Total Profit], [Total Sales], 0)
```

Format `Profit Margin %` as Percentage in the model; do not multiply it by 100 again.

## Tools

Power BI Desktop · Power Query · DAX · CSV / Excel

## Suggested report checks

1. Set the order date field to the Date data type.
2. Create a dedicated Date table for time intelligence where needed.
3. Confirm relationships and filter direction.
4. Use distinct count for order IDs.
5. Test KPI cards and charts with each slicer.
6. Reconcile report totals to the source dataset after refresh.
7. Check that month labels sort chronologically.

## How to use

Open the PBIX file if present, confirm source paths, refresh the model, and test the report interactions. Check the repository contents for the current PBIX and dataset files before sharing a live demo.

## Results and limitations

Add dashboard screenshots and numerical findings only after verifying the current report. Clearly identify practice or synthetic data and do not claim real-company impact.

## Skills demonstrated

Power BI · Power Query · DAX · Data modeling · KPI design · Interactive reporting

Maintained by [Omkar S. Kshirsagar](https://github.com/osk25-xc).
