# Getting Started

This guide walks you through connecting ClickForge to ClickHouse and opening your first endpoint.

## Screenshot

![Getting started screenshot (placeholder)](assets/placeholder.svg)

Replace with a screenshot of the Endpoints list and Add Endpoint flow.

## Prerequisites

You need a ClickHouse user that can read `system.parts`, `system.tables`, `system.columns`, `system.query_log`, and `system.part_log`. For Index Analysis variants, the user must also be able to `CREATE TABLE`, `INSERT`, and `DROP TABLE` in a destination database you control.

If `system.query_log` or `system.part_log` is disabled or access is denied, those features will show empty results.

## 1. Choose your organization

ClickForge scopes everything by organization. Use the Org selector in the sidebar to confirm you are in the correct org before creating endpoints or saving configurations.

## 2. Register a ClickHouse endpoint

Go to **Endpoints** and select **Add Endpoint**. Fill in:

- **Name**: Friendly label for the cluster
- **Host** and **Port**: 9000 for native or 8123 for HTTP
- **User** and **Database**: Defaults for new queries
- **Cluster**: Optional, used for display only
- **Secret Name** / **Impersonate SA**: Optional, for managed environments

Select **Create Endpoint** to save it.

## 3. Test connectivity

On the Endpoints page, select **Test** on the endpoint card. A green badge confirms ClickForge can connect.

## 4. Open the endpoint

Select the endpoint name to open its dashboard and start exploring features from the sidebar.

## 5. Run your first analysis

Start with **Table Monitor** to understand storage and growth, then use **Query Time** and **Filter Alignment** to prioritize the most impactful queries.

**Related**
Endpoint details and fields: [Endpoints](concepts/endpoints.md)
Start exploring storage: [Table Monitor](features/table-monitor.md)
