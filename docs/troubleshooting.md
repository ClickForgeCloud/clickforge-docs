# Troubleshooting

## Query Time or Filter Alignment shows no data

- Confirm `system.query_log` is enabled and has recent entries.
- Check the time range and timezone. ClickForge currently evaluates query log time in `Europe/Paris`.
- Make sure your ClickHouse user can read `system.query_log`.

## Growth charts are empty

- `system.part_log` may be disabled or empty.
- Ensure the ClickHouse user can read `system.part_log`.

## Index Analysis fails with database errors

- The destination database must exist before you run variants.
- The ClickHouse user needs `CREATE TABLE`, `INSERT`, and `DROP TABLE` permissions in that database.

## Lineage graph is empty

- Select at least one database and table.
- Ensure the ClickHouse user can read `system.tables`.
