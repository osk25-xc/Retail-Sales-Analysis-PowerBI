# Power BI Retail Report Validation Checklist

## Data and model

- Confirm Power Query has no unexpected errors or empty rows.
- Verify date columns use Date or Date/Time data types as intended.
- Check relationship cardinality and filter direction.
- Prefer a dedicated date table for time-intelligence reporting.
- Validate measures against source totals or a simple independent calculation.

## Visuals and interactions

- Test slicers across all report pages.
- Check that KPI cards, tables, and charts agree for the same filter context.
- Verify daily trend visuals use the date field at the intended granularity.
- Add descriptive titles, units, and meaningful axis labels.
- Test blank selections, single selections, and multiple selections.

## Delivery

- Save and reopen the PBIX file to confirm it works.
- Clearly state the reporting period and data source.
- Label sample or synthetic data honestly.
- Include screenshots only after validating the final report.
- Do not claim findings or measures are verified until they have been checked.