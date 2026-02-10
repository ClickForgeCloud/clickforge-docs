# Glossary

Below are short definitions for common terms used in ClickForge.

## ClickForge terms

- **Organization**: The top-level scope that owns endpoints and saved configurations.
- **Endpoint**: A saved ClickHouse connection used across all features.
- **Saved Configuration**: A stored Index Analysis setup (query, variants, and sampling).

## ClickHouse terms

- **Part**: A physical data chunk stored by MergeTree tables.
- **Partition**: A logical slice of a table used for data organization and pruning.
- **Granule**: A group of rows read together by the storage engine.
- **Skip Index**: An index that helps ClickHouse skip data blocks during reads.
- **ORDER BY**: The sorting key that defines primary data order for MergeTree tables.
- **Materialized View**: A view that stores its results in a target table.
- **Query Log**: `system.query_log`, which stores historical query execution data.
- **Part Log**: `system.part_log`, which stores part creation and merge events.
