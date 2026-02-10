# Query Time

Query Time analyzes query performance over time using data from `system.query_log`.

## Screenshot

![Query Time screenshot (placeholder)](../assets/placeholder.svg)

Replace with a screenshot of the timeline and pattern heatmap.

## What you can do

- Plot average query duration and read rows by hour
- Group results by a dimension (for example `query_user`)
- Add filters to focus on specific query sources
- Overlay individual query patterns on the timeline
- Export query patterns to CSV

## How to use it

1. Choose a start and end date/time.
2. Add optional filters. Filters are raw SQL predicates applied to `system.query_log`.
3. Optionally set a **Dimension (group by)** such as `query_user` or `current_database`. The dimension must be a column name, not an expression.
4. Click **Load** to render the timeline and heatmap.

## Reading the results

- **Timeline** shows average duration and read rows across time.
- **Dimension toggles** let you show or hide specific groups.
- **Query Pattern Heatmap** highlights the most impactful query hashes.
- Selecting a pattern adds it as an overlay on the timeline.

## Time zone note

Query Time uses the server-side timezone configured in ClickForge (currently `Europe/Paris`). If your team uses a different timezone, adjust the time range accordingly.

**Related**
Check filter coverage for top queries: [Filter Alignment](filter-alignment.md)
Compare query changes: [Benchmark](benchmark.md)
