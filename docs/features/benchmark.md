# Benchmark

Benchmark compares two queries or runs a parameterized load test against a single query.

## Screenshot

![Benchmark screenshot (placeholder)](../assets/placeholder.svg)

Replace with a screenshot of the Compare Queries and Load Test tabs.

## Compare Queries

Use this tab to run Query A and Query B once and compare performance side by side.

- Paste two queries
- Set a row limit for sample results
- Run the benchmark to see duration, rows read, memory usage, and diff

If both queries return data with matching schemas, ClickForge can also compare result sets.

## Load Test

Use this tab to run the same query multiple times with parameter sets.

- Provide a query with parameter placeholders
- Add JSON parameters as an array of objects
- Optionally supply ClickHouse settings as JSON

The results include run-level charts for duration, memory, and rows read, plus summary stats like P95 and P99.

## Data source

Benchmark collects performance stats from `system.query_log` after each run.

**Related**
Pick candidates to compare: [Query Time](query-time.md)
Design index changes first: [Index Analysis](index-analysis.md)
