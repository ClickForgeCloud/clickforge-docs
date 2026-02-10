# Index Analysis

Index Analysis lets you test ORDER BY and skip index variants on sampled data before changing production tables.

## Screenshot

![Index Analysis screenshot (placeholder)](../assets/placeholder.svg)

Replace with a screenshot of the query editor, variants, and results.

## Two modes

- **Single EXPLAIN**: Run EXPLAIN on the query without creating test tables.
- **Variants**: Create test tables for each variant and compare filter alignment and EXPLAIN stages.

## How to use it

1. Paste a SQL query.
2. Add one or more variants.
3. For each variant, set a source table and fetch its schema.
4. Choose ORDER BY columns and skip indexes.
5. Configure sampling (WHERE conditions and LIMIT).
6. Pick a destination database for test tables.
7. Run analysis.

## What you get

- EXPLAIN stages with granules and parts reduced
- Baseline vs variant comparisons
- Filter alignment coverage for each variant

## Saved configurations

Use **Saved Configurations** to load or save a full setup (query, variants, sampling). Saved configs are scoped to your organization.

## Important behavior

When running variants, ClickForge creates test tables named:

`{destination_database}.{source_table}_{variant_name}`

The destination database must already exist before you run analysis.

If **Cleanup After** is enabled, those tables are dropped automatically after the run. If it is disabled, you are responsible for deleting them.

**Related**
Find candidate queries: [Filter Alignment](filter-alignment.md)
Compare query variants end-to-end: [Benchmark](benchmark.md)
Manage stored setups: [Saved Configurations](../reference/resultstore.md)
