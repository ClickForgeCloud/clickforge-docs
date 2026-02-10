# Filter Alignment

Filter Alignment evaluates how query filters line up with ORDER BY keys and skip indexes for the most impactful queries in `system.query_log`.

## Screenshot

![Filter Alignment screenshot (placeholder)](../assets/placeholder.svg)

Replace with a screenshot of the results table with expanded row details.

## What it shows

- Leading and non-leading ORDER BY matches
- Partition key matches
- Skip index matches
- Uncovered filter columns

## How to use it

1. Set a start and end date/time.
2. Choose a sort mode: **Most Impactful**, **Most Executed**, or **Slowest**.
3. Set the number of queries to analyze.
4. Add optional filters. Filters are raw SQL predicates applied to `system.query_log`.
5. Optionally set a **Dimension (group by)** such as `query_user`. The dimension must be a column name, not an expression.
6. Click **Analyze**.

Each row represents a query pattern, with badges summarizing coverage. Expand a row to see per-table filter alignment details.

## Time zone note

Filter Alignment uses the server-side timezone configured in ClickForge (currently `Europe/Paris`). If your team uses a different timezone, adjust the time range accordingly.

**Related**
Start with query patterns: [Query Time](query-time.md)
Test index variants safely: [Index Analysis](index-analysis.md)
