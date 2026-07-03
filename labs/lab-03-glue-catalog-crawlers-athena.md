# Lab 3 - Glue Data Catalog, Crawlers, Athena, and Schema Discovery

## Objectives

- Create or review a Glue Data Catalog database.
- Use crawlers to discover schema if permitted.
- Query cataloged data with Athena.
- Understand partitions and schema evolution.

## Scenario

A data lake needs searchable metadata before analysts and pipelines can query it. You will catalog sample data and run basic SQL with Athena.

## Steps

1. Open AWS Glue.
2. Open Data Catalog databases.
3. Create a database only if your trainer permits it.
4. Review tables, columns, partitions, and schema metadata.
5. Open Crawlers.
6. Create a crawler for the S3 `raw/` prefix if permitted.
7. Assign or review the crawler IAM role.
8. Run the crawler.
9. Review the created table schema.
10. Open Athena.
11. Configure a query result location in S3 if required.
12. Select the Glue database.
13. Run a simple `SELECT *` query with a limit.
14. Run a count or group-by query.
15. Review query cost awareness based on scanned data.
16. Review how partitions reduce scanned data.
17. Add notes about schema evolution and crawler recrawls.
18. Save SQL snippets and screenshots.

## Deliverables

- Glue database and crawler notes
- Catalog table screenshot or schema notes
- Athena SQL snippets
- Partition and query-cost notes

## Checkpoint

You should be able to explain how Glue Data Catalog and Athena support data discovery and serverless querying.
