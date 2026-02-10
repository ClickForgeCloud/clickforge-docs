# Table Lineage

Table Lineage visualizes dependencies between tables, materialized views, distributed tables, and dictionaries.

## Screenshot

![Table Lineage screenshot (placeholder)](../assets/placeholder.svg)

Replace with a screenshot of the lineage graph and schema panel.

## How to use it

1. Select one or more databases.
2. Optionally select specific tables.
3. Click **Load Lineage**.

ClickForge will include related upstream and downstream nodes so the graph shows complete paths between selected objects.

## What the graph represents

- Dependencies are derived from `system.tables` and object definitions.
- Materialized views show both the source table they read from and the target table they write to.
- Distributed tables are linked to their local tables where possible.

## Schema panel

Selecting a node shows its schema details including columns, engine, ORDER BY, and partition key.

**Related**
Understand endpoint setup: [Endpoints](../concepts/endpoints.md)
Identify heavy query patterns: [Query Time](query-time.md)
