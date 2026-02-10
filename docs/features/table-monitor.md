# Table Monitor

Table Monitor gives you a fast overview of table size, compression, and growth trends for the selected endpoint.

## Screenshot

![Table Monitor screenshot (placeholder)](../assets/placeholder.svg)

Replace with a screenshot of the Table Monitor page showing filters, table stats, and growth charts.

## What you can do

- Filter by databases and tables
- Review per-table storage stats (rows, compressed size, uncompressed size, parts)
- Visualize storage and row growth over time

## How to use it

1. Pick one or more databases.
2. Optionally choose specific tables.
3. Select a date range for growth charts.

The **Table Statistics** section updates immediately after you select databases. Growth charts render when `system.part_log` data is available for the chosen range.

## Data sources

- Table stats come from `system.parts`.
- Growth charts use `system.part_log` with `event_type = 'NewPart'`.

If `system.part_log` is unavailable or empty, growth charts will show no data.

**Related**
See Growth for longer-term trends: [Growth](growth.md)
Explore storage layout in Parts Visualizer: [Parts Visualizer](parts-visualizer.md)
Investigate slow queries next: [Query Time](query-time.md)
