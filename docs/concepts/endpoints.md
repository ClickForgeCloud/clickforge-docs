# Endpoints

Endpoints are saved ClickHouse connections used across ClickForge features. Each endpoint belongs to a single organization.

## Endpoint fields

- **Name**: Display label used in the UI
- **Host**: ClickHouse host or IP
- **Port**: 9000 (native) or 8123 (HTTP)
- **User**: ClickHouse user for all queries
- **Database**: Default database for new queries
- **Cluster**: Optional label for multi-cluster environments
- **Secret Name**: Optional secret reference for managed auth
- **Impersonate SA**: Optional service account impersonation

## Connectivity checks

Each endpoint card includes a **Test** button. Use it to validate access before running analysis tools.

## Deleting endpoints

Deleting an endpoint removes it from ClickForge. It does not modify your ClickHouse cluster.
