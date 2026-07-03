# Learner Guide - AWS Certified Data Engineer Associate Training

> Course: AWS Certified Data Engineer Associate Training  
> Course Code: TGS-2025053209  
> Registration: https://www.tertiarycourses.com.sg/wsq-aws-certified-data-engineer-associate-training.html

This learner guide supports a practical AWS Certified Data Engineer Associate course. It is designed for learners preparing to design data models, manage data lifecycles, ensure data quality, ingest and transform data, and orchestrate AWS data pipelines.

## Learning Outcomes

By the end of the labs, you should be able to:

- Design a secure S3-based data lake structure.
- Select ingestion services for batch, streaming, file transfer, and database migration patterns.
- Use Glue Data Catalog, crawlers, and Athena for schema discovery and querying.
- Design Glue ETL and data quality workflows.
- Compare Redshift, DynamoDB, OpenSearch, RDS, Athena, and S3 for data serving and modeling.
- Design orchestration using Step Functions, MWAA, Glue Workflows, and EventBridge.
- Apply security and governance using IAM, S3 policies, KMS, Lake Formation, Macie, CloudTrail, and lifecycle rules.
- Plan monitoring, reliability, and cost optimization for data pipelines.
- Prepare for exam-style AWS data engineering questions.

## Recommended Setup

1. Use a trainer-provided AWS account where available.
2. If using your own account, enable MFA and create a budget alert before starting labs.
3. Create a working folder named `TGS-2025053209-AWS-DEA-Labs`.
4. Save screenshots, SQL snippets, architecture notes, and service comparison tables.
5. Delete temporary AWS resources after each hands-on exercise.

## Cost Safety Rules

- Use small sample datasets.
- Avoid long-running streams, clusters, and warehouses unless explicitly assigned.
- Stop or delete jobs, crawlers, streams, databases, and buckets after labs if instructed.
- Keep S3 lifecycle and budget alerts in mind for every design.
- Check Billing and Cost Management after hands-on labs.

## Lab 1 - Account Safety, IAM, S3 Data Lake, and Data Formats

### Objectives

- Set up a safe AWS learning baseline.
- Review IAM and least privilege for data services.
- Create an S3 data lake structure.
- Compare data formats.

### Procedure

1. Sign in to the AWS account assigned by your trainer.
2. Confirm the account and region.
3. Open IAM and review users, groups, roles, and policies.
4. Verify MFA where permitted.
5. Review least-privilege access for S3, Glue, Athena, and KMS.
6. Open S3.
7. Create a bucket only if permitted.
8. Enable default encryption and keep Block Public Access enabled.
9. Create prefixes for raw, curated, analytics, and logs.
10. Upload small sample CSV and JSON files.
11. Review object metadata and storage class.
12. Compare CSV, JSON, Parquet, and ORC.
13. Review KMS customer managed key concepts.
14. Save your notes.

### Checkpoint

You should be able to explain how IAM, S3, encryption, prefixes, and data formats support a data lake foundation.

## Lab 2 - Data Ingestion with Kinesis, DMS, Transfer, and Event Patterns

### Objectives

- Compare ingestion patterns.
- Review streaming, migration, file transfer, and event services.
- Design simple ingestion architectures.
- Identify monitoring and cost considerations.

### Procedure

1. Review Kinesis Data Streams, Data Firehose, and Managed Service for Apache Flink.
2. Review Database Migration Service and CDC concepts.
3. Review DataSync and Transfer Family.
4. Review EventBridge rules, schedules, and targets.
5. Create an ingestion pattern table.
6. Draw a batch file ingestion architecture.
7. Draw a streaming event ingestion architecture.
8. Identify monitoring points.
9. Save your notes.

### Checkpoint

You should be able to select ingestion services for batch, streaming, migration, CDC, and managed file-transfer scenarios.

## Lab 3 - Glue Data Catalog, Crawlers, Athena, and Schema Discovery

### Objectives

- Catalog sample data.
- Query data with Athena.
- Understand schema and partitioning.
- Manage query cost awareness.

### Procedure

1. Open AWS Glue Data Catalog.
2. Create a database if permitted.
3. Create and run a crawler for S3 sample data if permitted.
4. Review generated table schema.
5. Open Athena.
6. Configure a query result location if required.
7. Run basic `SELECT`, `COUNT`, and `GROUP BY` queries.
8. Review scanned data and cost awareness.
9. Record how partitions reduce scanned data.
10. Save SQL snippets.

### Checkpoint

You should be able to explain how Glue Data Catalog and Athena support schema discovery and serverless analytics.

## Lab 4 - Glue ETL, Data Quality, and Data Transformation

### Objectives

- Design raw-to-curated transformations.
- Review Glue ETL job settings.
- Apply data quality rules.
- Choose output formats.

### Procedure

1. Open Glue ETL jobs.
2. Review visual ETL and script job options.
3. Design a source from S3 raw data.
4. Add transforms such as select fields, rename, drop nulls, or cast types.
5. Choose S3 curated output.
6. Select Parquet if assigned.
7. Review worker type, bookmarks, retries, and logs.
8. Define data quality rules.
9. Compare Glue, EMR, Lambda, and Athena CTAS for transformations.
10. Save your notes.

### Checkpoint

You should be able to describe how AWS data pipelines clean, validate, and transform data for analytics.

## Lab 5 - Data Modeling with Redshift, DynamoDB, OpenSearch, and RDS

### Objectives

- Compare data stores.
- Match query patterns to services.
- Review modeling choices.
- Understand scaling and backup considerations.

### Procedure

1. Review Redshift cluster and serverless concepts.
2. Review distribution and sort key awareness.
3. Review DynamoDB partition keys, sort keys, and indexes.
4. Review OpenSearch search and log analytics use cases.
5. Review RDS relational use cases.
6. Create a service selection table.
7. Sketch a Redshift fact/dimension model.
8. Sketch a DynamoDB key design.
9. Identify OpenSearch indexed fields.
10. Save your notes.

### Checkpoint

You should be able to match data modeling choices to workload requirements.

## Lab 6 - Pipeline Orchestration with Step Functions, MWAA, and EventBridge

### Objectives

- Compare orchestration services.
- Design pipeline dependencies.
- Add retries and failure handling.
- Identify monitoring points.

### Procedure

1. Review Step Functions state machines, tasks, retries, catches, and executions.
2. Review MWAA DAG and task concepts.
3. Review Glue Workflows.
4. Review EventBridge schedules and targets.
5. Create an orchestration service comparison table.
6. Design a daily pipeline for ingest, crawl, transform, quality check, query validation, and notification.
7. Add retry and failure paths.
8. Identify metrics and logs to monitor.
9. Save your design.

### Checkpoint

You should be able to design and explain a data pipeline orchestration workflow.

## Lab 7 - Security, Governance, Lake Formation, KMS, and Data Lifecycle

### Objectives

- Apply security controls for data platforms.
- Review Lake Formation permissions.
- Use KMS and lifecycle concepts.
- Plan governance and retention.

### Procedure

1. Review IAM roles for Glue, Athena, S3, and Lake Formation.
2. Review S3 bucket policies, access points, object ownership, and encryption.
3. Review KMS key policies and grants.
4. Review Lake Formation administrators, databases, tables, permissions, and LF-Tags.
5. Compare IAM/S3 policies with Lake Formation permissions.
6. Review Macie sensitive data discovery use cases.
7. Design lifecycle transitions for raw, curated, analytics, and archive zones.
8. Define retention and deletion rules.
9. Review CloudTrail audit concepts.
10. Save your notes.

### Checkpoint

You should be able to explain AWS data security, governance, encryption, lifecycle, and audit controls.

## Lab 8 - Monitoring, Cost Optimization, Reliability, and Exam Review

### Objectives

- Plan data pipeline monitoring.
- Review cost and reliability patterns.
- Map labs to exam domains.
- Complete timed practice.

### Procedure

1. Review CloudWatch metrics, logs, alarms, and dashboards.
2. Identify monitoring points for S3, Glue, Athena, Kinesis, Step Functions, and Redshift.
3. Review CloudTrail audit events.
4. Create a cost-control checklist.
5. Identify cost drivers such as scanned data, worker runtime, storage class, stream shards, and warehouse capacity.
6. Create a reliability checklist covering retries, idempotency, dead-letter queues, partitioning, backup, and disaster recovery.
7. Map each lab to exam domains.
8. Complete a timed 30-question practice set.
9. Mark weak topics and create a revision plan.
10. Clean up temporary resources.

### Checkpoint

You should be ready to explain AWS data engineering services and scenario choices under exam conditions.

## Final Submission Checklist

- Lab notes or screenshots
- Ingestion, transformation, modeling, orchestration, and governance comparison tables
- SQL snippets or pseudocode
- Security and lifecycle design notes
- Monitoring and cost-control checklist
- Timed practice score
- Weak-topic revision plan

## Suggested Course Flow

| Segment | Focus | Labs |
| --- | --- | --- |
| Segment 1 | S3 data lake, IAM, ingestion patterns | Labs 1-2 |
| Segment 2 | Catalog, Athena, ETL, data quality, modeling | Labs 3-5 |
| Segment 3 | Orchestration, governance, operations, exam review | Labs 6-8 |

## Clean Up

1. Delete temporary S3 buckets, objects, and query results if instructed.
2. Delete crawlers, jobs, streams, and databases created for labs if instructed.
3. Stop or delete provisioned data services that may incur cost.
4. Keep budget alerts active until the trainer confirms cleanup.
5. Save notes for final revision.
