# Growth

Growth analytics focuses on storage and row trends over time. It appears both as a standalone page and inside Table Monitor.

## Screenshot

![Growth analytics screenshot (placeholder)](../assets/placeholder.svg)

Replace with a screenshot of the Growth charts (storage + row growth).

## What the charts show

- **Storage Growth**: Compressed bytes by table, with an option to overlay uncompressed size
- **Row Growth**: Row counts by table

Both charts support log scale to highlight changes across very different table sizes.

## Tips

- Use a longer date range to spot slow creep and sudden spikes.
- Compare compressed vs uncompressed to detect compression drift.
- If no data appears, confirm `system.part_log` is enabled and has recent entries.

**Related**
Monitor tables alongside growth trends: [Table Monitor](table-monitor.md)
Drill into storage layout: [Parts Visualizer](parts-visualizer.md)
