# Retail Sales Power BI Model & KPI QA Checklist

Validate the model and report after each data refresh. Confirm actual table and column names before using example measures.

## Data preparation
- [ ] Check Power Query data types, nulls, errors, and duplicate business keys.
- [ ] Confirm date columns are true Date values and numeric fields are numeric.
- [ ] Record any row filters, replacements, and removed records.

## Model
- [ ] Use a clearly defined fact-table grain.
- [ ] Validate dimension keys and relationship cardinality.
- [ ] Review relationship direction and avoid ambiguous filter paths.
- [ ] Use a dedicated Date table when time intelligence is required.
- [ ] Sort month names by a numeric month key.

## KPI measures
- [ ] Define sales, profit, distinct orders, and profit margin explicitly.
- [ ] Use DIVIDE for ratios and define the alternate result.
- [ ] Calculate margin from aggregate profit / aggregate sales, not an average of row percentages.
- [ ] Check blank and zero handling against business definitions.

## Report interactions
- [ ] Test each slicer against all relevant KPI cards and visuals.
- [ ] Reconcile filtered and unfiltered totals to source data.
- [ ] Check visual titles, units, date coverage, and filter context.
- [ ] Document refresh timestamp and known limitations before sharing.