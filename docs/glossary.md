# Glossary

Below are short definitions for common terms used in ClickForge.

## ClickForge terms

- <span class="glossary-term">Organization</span>: The top-level scope that owns endpoints and saved configurations.
- <span class="glossary-term">Endpoint</span>: A saved ClickHouse connection used across all features.
- <span class="glossary-term">Saved Configuration</span>: A stored Index Analysis setup (query, variants, and sampling).

## ClickHouse terms

- <span class="glossary-term">Part</span>: A physical data chunk stored by MergeTree tables.
- <span class="glossary-term">Partition</span>: A logical slice of a table used for data organization and pruning.
- <span class="glossary-term">Granule</span>: A group of rows read together by the storage engine.
- <span class="glossary-term">Skip Index</span>: An index that helps ClickHouse skip data blocks during reads.
- <span class="glossary-term">ORDER BY</span>: The sorting key that defines primary data order for MergeTree tables.
- <span class="glossary-term">Materialized View</span>: A view that stores its results in a target table.
- <span class="glossary-term">Query Log</span>: `system.query_log`, which stores historical query execution data.
- <span class="glossary-term">Part Log</span>: `system.part_log`, which stores part creation and merge events.
