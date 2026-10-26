# Power BI Date Table Template

A dedicated date table supports consistent daily, monthly, and year-to-date reporting. Adjust the date range to your model and confirm the relationship before using time intelligence.

```dax
DateTable =
ADDCOLUMNS (
    CALENDAR ( DATE ( 2024, 1, 1 ), DATE ( 2027, 12, 31 ) ),
    "Year", YEAR ( [Date] ),
    "Month Number", MONTH ( [Date] ),
    "Month", FORMAT ( [Date], "MMM" ),
    "Year-Month", FORMAT ( [Date], "YYYY-MM" )
)
```

## Setup checks

1. Change the start and end dates to cover the actual dataset.
2. Mark this table as the model's date table using its `Date` column.
3. Create a one-to-many relationship from `DateTable[Date]` to the fact table's date column.
4. Sort `Month` by `Month Number` for month labels; use a year-month sort key for multi-year charts.
5. Use the date-table fields in slicers and trend axes.
6. Validate totals with and without date filters.

This is a template, not a verified change to any PBIX file. Confirm the fact table and date column names in the model.