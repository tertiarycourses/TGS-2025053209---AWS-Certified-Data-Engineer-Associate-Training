# Lab 5 - Data Modeling with Redshift, DynamoDB, OpenSearch, and RDS

## Objectives

- Compare data modeling choices across AWS services.
- Review Redshift, DynamoDB, OpenSearch, and RDS use cases.
- Understand keys, distribution, sorting, indexing, and query patterns at a high level.
- Match workload requirements to the right data store.

## Scenario

Data engineers must choose storage and serving layers based on access patterns, scale, latency, and analytics requirements. This lab focuses on service selection and modeling tradeoffs.

## Steps

1. Open Amazon Redshift.
2. Review cluster, serverless, database, schema, table, distribution, and sort key concepts.
3. Open DynamoDB.
4. Review table, partition key, sort key, item, global secondary index, and capacity concepts.
5. Open Amazon OpenSearch Service.
6. Review search and log analytics use cases.
7. Open Amazon RDS.
8. Review relational database use cases and managed backups.
9. Create a use-case table for warehouse analytics, operational NoSQL, search analytics, and relational applications.
10. For a sample order dataset, identify candidate Redshift fact and dimension tables.
11. For a sample event lookup workload, identify a DynamoDB partition key and optional sort key.
12. For a document search workload, identify indexed fields for OpenSearch.
13. Record high-level backup, scaling, and security considerations for each service.
14. Save your notes.

## Deliverables

- Data service selection table
- Sample Redshift model notes
- Sample DynamoDB key design notes
- OpenSearch indexing notes

## Checkpoint

You should be able to match data stores and modeling choices to query patterns and business requirements.
