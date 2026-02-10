# Quick Wins

A short plan for getting value from ClickForge in your first week.

## Day 1: Connect and validate

1. Add your first endpoint and run a connectivity test.
2. Open **Table Monitor** and review the largest tables.
3. Confirm growth charts render for the last 30 days.

## Day 2: Find query hot spots

1. Open **Query Time** and load the last 7 days.
2. Export the top query patterns to CSV.
3. Note the top 3 query hashes by impact and duration.

## Day 3: Validate index coverage

1. Open **Filter Alignment** for the same time range.
2. Focus on queries with uncovered filter columns.
3. Pick one candidate query and open **Index Analysis**.

## Day 4: Test variants safely

1. Create a destination database for test tables.
2. Add two variants with different ORDER BY and skip indexes.
3. Compare EXPLAIN stages and pick the best reduction.

## Day 5: Compare real query changes

1. Use **Benchmark** to compare the original query and your optimized version.
2. Confirm improvements in duration, read rows, and memory.
3. Share results with your team for implementation.

**Related**
Review the tools in detail: [Table Monitor](features/table-monitor.md)
Look up terminology: [Glossary](glossary.md)
