# Reusable DAX Measure Examples

These are templates. Replace table and column names with the actual model schema and validate each measure in Power BI before using it in a report.

## Total Sales

```dax
Total Sales =
SUM ( Sales[SalesAmount] )
```

## Total Profit

```dax
Total Profit =
SUM ( Sales[Profit] )
```

## Order Count

```dax
Order Count =
DISTINCTCOUNT ( Sales[OrderID] )
```

## Profit Margin

```dax
Profit Margin % =
DIVIDE ( [Total Profit], [Total Sales] )
```

Format the measure as a percentage in the model. `DIVIDE` handles a zero or blank denominator safely by returning blank unless an alternate result is specified.

## Validation notes

- Confirm that SalesAmount and Profit have the correct business definitions.
- Check whether the source is one row per order or one row per order line.
- Use a distinct order count when order IDs repeat across line items.
- Compare measures with independently calculated source totals.
- Test slicers, date filters, and category filters.
- These examples are templates and have not been tested against a specific PBIX model.