# Learner Guide - AWS Certified Data Engineer Associate Training

**Course Code:** TGS-2025053209  
**Version:** 1  
**Provider:** Tertiary Infotech Academy Pte Ltd

## Learning Outcomes

- Design a secure S3-based data lake foundation.
- Select AWS ingestion services for batch, streaming, migration, and file-transfer workloads.
- Use Glue Data Catalog, crawlers, and Athena for schema discovery and serverless analytics.
- Plan Glue ETL, data quality checks, and transformation outputs.
- Match Redshift, DynamoDB, OpenSearch, RDS, Athena, and S3 to data modeling requirements.
- Design orchestration with Step Functions, MWAA, Glue Workflows, and EventBridge.
- Apply governance, encryption, lifecycle, and audit controls for data platforms.
- Plan monitoring, reliability, cost optimization, and exam revision.

## Recommended Setup

1. Use a trainer-provided AWS account where available.
2. If using your own account, enable MFA and create an AWS Budget before hands-on work.
3. Create a working folder named `TGS-2025053209-AWS-DEA-Labs`.
4. Save screenshots, SQL snippets, architecture notes, and comparison tables after each lab.
5. Delete temporary AWS resources when instructed.

## Lab 1 - Account Safety, IAM, S3 Data Lake, and Data Formats

### Goal

Configure a safe AWS learning baseline.

### Scenario

You are preparing an AWS data engineering workspace. The first step is to create secure access patterns and a clear S3 data lake structure.

### Step-by-Step Instructions

1. Sign in to the AWS account assigned by your trainer.
2. Confirm you are in the correct region.
3. Open IAM and review users, groups, roles, and policies.
4. Verify MFA is enabled where permitted.
5. Review least-privilege access for S3, Glue, Athena, and KMS.
6. Open S3.
7. Create a bucket only if your trainer permits it.
8. Enable default encryption.
9. Keep Block Public Access enabled.
10. Create prefixes named `raw/`, `curated/`, `analytics/`, and `logs/`.
11. Upload small sample CSV and JSON files to `raw/`.
12. Review object metadata and storage class.
13. Create a table comparing CSV, JSON, Parquet, and ORC.
14. Record which formats support efficient analytics better.
15. Open KMS and review customer managed key concepts.
16. Open Billing and confirm budget monitoring is available.
17. Save your notes.

### Expected Results and Validation

You should be able to explain how IAM, S3 prefixes, encryption, and file formats support a data lake foundation.

### Learner Evidence to Capture

- IAM and least-privilege notes
- S3 data lake prefix structure
- Data format comparison table
- Encryption and cost safety notes

### Troubleshooting Notes

- If the console does not show an option, confirm the correct AWS region and account permissions.
- If a service may incur cost, pause and ask the trainer before creating resources.
- If access is denied, capture the error message and map it to IAM, S3, KMS, or Lake Formation permissions.

## Lab 2 - Data Ingestion with Kinesis, DMS, Transfer, and Event Patterns

### Goal

Compare batch, streaming, migration, and managed file transfer ingestion patterns.

### Scenario

Data platforms ingest files, events, database changes, and streams. This lab focuses on choosing appropriate AWS ingestion services and designing a simple ingestion pattern.

### Step-by-Step Instructions

1. Open the Kinesis console.
2. Review Data Streams, Data Firehose, and Managed Service for Apache Flink use cases.
3. Record the difference between stream capture, delivery, and stream processing.
4. Open AWS Database Migration Service.
5. Review source, target, replication instance, and change data capture concepts.
6. Open AWS DataSync.
7. Review file migration and transfer use cases.
8. Open AWS Transfer Family.
9. Review SFTP, FTPS, and FTP managed transfer use cases.
10. Open EventBridge.
11. Review event bus, rule, schedule, and target concepts.
12. Create an ingestion pattern table for batch files, streaming events, database migration, CDC, managed file transfer, and scheduled events.
13. Draw a simple architecture for ingesting daily CSV files into S3 and cataloging them.
14. Draw a second architecture for streaming click events into S3 or analytics.
15. Identify monitoring points for each architecture.
16. Save your notes.

### Expected Results and Validation

You should be able to select ingestion services for common batch, streaming, migration, and file-transfer scenarios.

### Learner Evidence to Capture

- Ingestion service comparison table
- Batch ingestion architecture notes
- Streaming ingestion architecture notes
- Monitoring and cost considerations

### Troubleshooting Notes

- If the console does not show an option, confirm the correct AWS region and account permissions.
- If a service may incur cost, pause and ask the trainer before creating resources.
- If access is denied, capture the error message and map it to IAM, S3, KMS, or Lake Formation permissions.

## Lab 3 - Glue Data Catalog, Crawlers, Athena, and Schema Discovery

### Goal

Create or review a Glue Data Catalog database.

### Scenario

A data lake needs searchable metadata before analysts and pipelines can query it. You will catalog sample data and run basic SQL with Athena.

### Step-by-Step Instructions

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

### Expected Results and Validation

You should be able to explain how Glue Data Catalog and Athena support data discovery and serverless querying.

### Learner Evidence to Capture

- Glue database and crawler notes
- Catalog table screenshot or schema notes
- Athena SQL snippets
- Partition and query-cost notes

### Troubleshooting Notes

- If the console does not show an option, confirm the correct AWS region and account permissions.
- If a service may incur cost, pause and ask the trainer before creating resources.
- If access is denied, capture the error message and map it to IAM, S3, KMS, or Lake Formation permissions.

## Lab 4 - Glue ETL, Data Quality, and Data Transformation

### Goal

Review Glue ETL job concepts.

### Scenario

Raw data often needs cleaning, validation, transformation, and conversion to analytics-friendly formats. You will design or run a small ETL workflow.

### Step-by-Step Instructions

1. Open AWS Glue ETL jobs.
2. Review visual ETL and script-based job options.
3. Create a job only if your trainer permits it.
4. Select S3 raw data as the source.
5. Choose a transform such as select fields, rename fields, drop nulls, or cast data types.
6. Choose S3 curated data as the target.
7. Select Parquet as the output format if assigned.
8. Review job parameters, worker type, bookmarks, retries, and logging.
9. Run the job only if permitted.
10. Open the target S3 prefix and review output files.
11. Open CloudWatch logs for job output.
12. Review AWS Glue Data Quality concepts.
13. Define quality rules such as non-null primary key, valid date format, row count threshold, or allowed value set.
14. Create a data quality checklist for the sample dataset.
15. Record when to use Glue, EMR, Lambda, or Athena CTAS for transformations.
16. Save your notes.

### Expected Results and Validation

You should be able to describe how Glue ETL transforms and validates data before analytics consumption.

### Learner Evidence to Capture

- ETL design notes or job screenshot
- Raw-to-curated transformation checklist
- Data quality rule list
- Output format decision notes

### Troubleshooting Notes

- If the console does not show an option, confirm the correct AWS region and account permissions.
- If a service may incur cost, pause and ask the trainer before creating resources.
- If access is denied, capture the error message and map it to IAM, S3, KMS, or Lake Formation permissions.

## Lab 5 - Data Modeling with Redshift, DynamoDB, OpenSearch, and RDS

### Goal

Compare data modeling choices across AWS services.

### Scenario

Data engineers must choose storage and serving layers based on access patterns, scale, latency, and analytics requirements. This lab focuses on service selection and modeling tradeoffs.

### Step-by-Step Instructions

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

### Expected Results and Validation

You should be able to match data stores and modeling choices to query patterns and business requirements.

### Learner Evidence to Capture

- Data service selection table
- Sample Redshift model notes
- Sample DynamoDB key design notes
- OpenSearch indexing notes

### Troubleshooting Notes

- If the console does not show an option, confirm the correct AWS region and account permissions.
- If a service may incur cost, pause and ask the trainer before creating resources.
- If access is denied, capture the error message and map it to IAM, S3, KMS, or Lake Formation permissions.

## Lab 6 - Pipeline Orchestration with Step Functions, MWAA, and EventBridge

### Goal

Understand orchestration and scheduling choices.

### Scenario

Data pipelines need scheduling, sequencing, dependency management, error handling, and monitoring. This lab teaches orchestration design patterns.

### Step-by-Step Instructions

1. Open AWS Step Functions.
2. Review state machines, tasks, choices, retries, catches, and executions.
3. Open Amazon Managed Workflows for Apache Airflow.
4. Review DAG, task, dependency, and environment concepts.
5. Open AWS Glue Workflows if available.
6. Review job and crawler orchestration.
7. Open EventBridge.
8. Review rules, schedules, events, and targets.
9. Create a comparison table for Step Functions, MWAA, Glue Workflows, and EventBridge.
10. Design a daily pipeline with steps for ingest, crawl, transform, quality check, query validation, and notification.
11. Add retry and failure paths to the design.
12. Identify which service would trigger each step.
13. Identify which metrics or logs should be monitored.
14. Create a simple architecture diagram in your notes.
15. Save your design.

### Expected Results and Validation

You should be able to design a simple data pipeline orchestration flow and justify the orchestration service choice.

### Learner Evidence to Capture

- Orchestration service comparison table
- Daily pipeline design
- Retry and failure-handling notes
- Monitoring points

### Troubleshooting Notes

- If the console does not show an option, confirm the correct AWS region and account permissions.
- If a service may incur cost, pause and ask the trainer before creating resources.
- If access is denied, capture the error message and map it to IAM, S3, KMS, or Lake Formation permissions.

## Lab 7 - Security, Governance, Lake Formation, KMS, and Data Lifecycle

### Goal

Review data security controls for AWS data platforms.

### Scenario

Data engineering work must protect sensitive data, control access, encrypt assets, and manage data lifecycle. This lab focuses on governance and security service choices.

### Step-by-Step Instructions

1. Open IAM and review least-privilege roles for Glue, Athena, S3, and Lake Formation.
2. Open S3 and review bucket policies, access points, object ownership, and encryption.
3. Open KMS and review AWS managed keys and customer managed keys.
4. Review key policies and grants at a high level.
5. Open Lake Formation.
6. Review data lake administrators, databases, tables, permissions, and tag-based access control.
7. Review how Lake Formation differs from only using IAM and S3 bucket policies.
8. Create a governance table covering IAM, S3 policies, KMS, Lake Formation, CloudTrail, and Macie.
9. Open Amazon Macie if available and review sensitive data discovery use cases.
10. Review S3 lifecycle rules.
11. Design lifecycle transitions for raw, curated, analytics, and archive data zones.
12. Define retention and deletion rules for a sample dataset.
13. Review CloudTrail auditing for data access changes.
14. Save your notes.

### Expected Results and Validation

You should be able to explain how IAM, S3, KMS, Lake Formation, Macie, lifecycle rules, and audit logs protect data platforms.

### Learner Evidence to Capture

- Data governance service table
- Lake Formation permission notes
- KMS encryption notes
- Lifecycle and retention design

### Troubleshooting Notes

- If the console does not show an option, confirm the correct AWS region and account permissions.
- If a service may incur cost, pause and ask the trainer before creating resources.
- If access is denied, capture the error message and map it to IAM, S3, KMS, or Lake Formation permissions.

## Lab 8 - Monitoring, Cost Optimization, Reliability, and Exam Review

### Goal

Design monitoring for data pipelines.

### Scenario

The final lab ties together operations, reliability, cost, and exam readiness for AWS data engineering workloads.

### Step-by-Step Instructions

1. Open CloudWatch.
2. Review metrics, logs, alarms, and dashboards.
3. Identify monitoring points for S3, Glue, Athena, Kinesis, Step Functions, and Redshift.
4. Open CloudTrail and review audit event concepts.
5. Open AWS Budgets and Cost Explorer.
6. Create a cost-control checklist for data pipelines.
7. Review cost drivers such as scanned data, ETL worker runtime, storage class, stream shard count, and warehouse capacity.
8. Create a reliability checklist covering retries, idempotency, dead-letter queues, partitioning, backup, and disaster recovery.
9. Review exam domains and map each lab to one or more domains.
10. Complete a timed 30-question practice set from trainer-provided questions or AWS practice resources.
11. Mark weak topics by domain.
12. Create a final revision plan.
13. Clean up temporary resources if instructed.
14. Save final notes.

### Expected Results and Validation

You should be ready to explain AWS data engineering services, pipeline patterns, governance, operations, and exam-style scenario choices.

### Learner Evidence to Capture

- Monitoring plan
- Cost optimization checklist
- Reliability checklist
- Timed practice score
- Weak-topic revision plan

### Troubleshooting Notes

- If the console does not show an option, confirm the correct AWS region and account permissions.
- If a service may incur cost, pause and ask the trainer before creating resources.
- If access is denied, capture the error message and map it to IAM, S3, KMS, or Lake Formation permissions.
