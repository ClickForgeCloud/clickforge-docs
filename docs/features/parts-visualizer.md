# Parts Visualizer

Parts Visualizer explores active ClickHouse parts and partitions for the selected databases.

## Screenshot

![Parts Visualizer screenshot (placeholder)](../assets/placeholder.svg)

Replace with a screenshot of the Parts Visualizer showing treemap + bar chart.

## What you can do

- Group by partition or by individual parts
- Filter by minimum part size
- Inspect compression ratio, row counts, and bytes on disk

## How to use it

1. Select one or more databases.
2. Choose **Partitions** or **Parts** in the Group by toggle.
3. Set a minimum size threshold to focus on large parts.
4. Use the partition filter inside each table to narrow the view.

## Interpreting the charts

- The treemap shows relative size across partitions or parts.
- The bar chart summarizes compressed vs uncompressed bytes and row counts.
- Hover a chart item to see disk, row, and compression details.

## Data source

Parts Visualizer reads from `system.parts` and only shows active parts.

**Related**
Review table-level stats first: [Table Monitor](table-monitor.md)
Analyze long-term growth: [Growth](growth.md)
