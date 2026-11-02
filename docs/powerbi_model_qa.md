# Power BI Model and Report QA

## Model checks
1. Confirm fact-table grain and unique keys.
2. Use a dedicated date dimension for time analysis when appropriate.
3. Validate one-to-many relationships and avoid ambiguous filter paths.
4. Mark the date table and check month sorting.
5. Hide technical keys from report consumers where appropriate.

## Measure checks
- Use `DISTINCTCOUNT` for order identifiers when facts are at line-item grain.
- Calculate margin as `DIVIDE([Total Profit], [Total Sales], 0)`.
- Confirm blank and zero behavior is intentional.
- Validate time-intelligence measures against a known date range.

## Interaction checks
Test slicers, cross-highlighting, drill-through, and page navigation. Reconcile card totals with an independent source calculation after refresh.

## Release checklist
Document data source, refresh timestamp, filters, and known limitations. Do not publish unverified screenshots or performance claims.
