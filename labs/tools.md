# Tools Reference

## Required Tools

- AWS account or trainer-provided sandbox account
- Web browser
- Notes application or markdown editor

## Recommended AWS Services and Consoles

- IAM
- Amazon S3
- AWS KMS
- AWS Glue Data Catalog
- AWS Glue Crawlers
- AWS Glue ETL
- Amazon Athena
- Amazon Kinesis
- AWS Database Migration Service
- AWS DataSync
- AWS Transfer Family
- Amazon Redshift
- Amazon DynamoDB
- Amazon OpenSearch Service
- Amazon RDS
- AWS Step Functions
- Amazon Managed Workflows for Apache Airflow
- Amazon EventBridge
- AWS Lake Formation
- Amazon CloudWatch
- AWS CloudTrail
- AWS Budgets
- AWS Pricing Calculator

## Cost Safety

- Use trainer-provided accounts where available.
- Prefer small sample datasets.
- Avoid always-on services unless explicitly assigned.
- Delete temporary crawlers, jobs, databases, streams, and buckets after labs if instructed.
- Set budget alerts before using hands-on services.
- Check Billing and Cost Management after labs.

## Learner Tips

- Separate ingestion, storage, transformation, orchestration, and consumption concerns.
- Use S3 prefixes deliberately: raw, curated, and analytics zones.
- Know when a service is serverless, managed, batch, streaming, or event-driven.
- Practice explaining why one data service fits a use case better than another.
- Keep a weak-topic list for exam revision.
