# ClickForge

ClickForge is a ClickHouse performance toolkit for operators who need fast answers about storage growth, query behavior, and indexing decisions.

## What ClickForge helps you do

- Understand where storage is growing and which tables drive it
- Visualize table dependencies, materialized views, and downstream impact
- Inspect query behavior over time and spot slow or heavy patterns
- Test index changes safely on sampled data before applying them in production
- Benchmark two query variants and compare results side by side

## How it works

ClickForge connects to your ClickHouse cluster and reads from system tables like `system.parts`, `system.tables`, `system.part_log`, and `system.query_log`. Some workflows (Index Analysis) also create temporary test tables in a destination database you choose.

## Main areas in the UI

The sidebar groups tools into **Observability** and **Experiments**, matching the app navigation.

**Observability**
Table Monitor: Storage, table stats, and growth trends
Table Lineage: Upstream and downstream dependencies between tables
Parts Visualizer: Part-level storage and compression exploration
Query Time: Query performance trends and pattern heatmaps
Filter Alignment: How query filters match ORDER BY and skip indexes

**Experiments**
Index Analysis: Compare ORDER BY and skip index variants using sampled data
Benchmark: Compare two queries or run parameterized load tests

## Start here

If this is your first time using ClickForge, go to **Getting Started** to connect an endpoint and run your first analysis.
