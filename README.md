# TGS-2025053209 - AWS Certified Data Engineer Associate Training

> Course: AWS Certified Data Engineer Associate Training  
> Course Code: TGS-2025053209  
> Register here: https://www.tertiarycourses.com.sg/wsq-aws-certified-data-engineer-associate-training.html

Hands-on AWS Certified Data Engineer Associate labs for learners preparing for the AWS Certified Data Engineer - Associate exam. The labs cover data ingestion, storage, transformation, orchestration, data modeling, lifecycle management, data quality, security, governance, monitoring, cost optimization, and exam-style review.

## Courseware

| Item | Description |
| --- | --- |
| [Learner Guide](LG-AWS-Certified-Data-Engineer-Associate-Training.md) | Detailed step-by-step guide for completing the labs and preparing final deliverables. |
| [Lab Guide](labs/README.md) | Lab catalogue grouped by AWS data engineering skill area. |
| [Tools Reference](labs/tools.md) | Recommended AWS tools, free tier notes, and learner setup checklist. |

## How to Use

1. Create or use an AWS account provided by your trainer.
2. Create a working folder named `TGS-2025053209-AWS-DEA-Labs`.
3. Complete the labs in sequence because later labs reuse S3, Glue, Athena, IAM, and pipeline concepts.
4. Record screenshots, SQL snippets, scripts, and configuration notes for each lab.
5. Delete paid resources when the lab asks you to clean up.

## Lab Catalogue

### Domain 1 - Data Ingestion and Storage

| Lab | Title | Focus |
| --- | --- | --- |
| [Lab 1](labs/lab-01-account-iam-s3-data-lake.md) | Account Safety, IAM, S3 Data Lake, and Data Formats | IAM, S3 buckets, prefixes, encryption, CSV/JSON/Parquet awareness |
| [Lab 2](labs/lab-02-data-ingestion-kinesis-dms-transfer.md) | Data Ingestion with Kinesis, DMS, Transfer, and Event Patterns | Batch vs streaming, Kinesis, DMS, DataSync, Transfer Family, EventBridge |

### Domain 2 - Transformation, Catalog, and Analytics

| Lab | Title | Focus |
| --- | --- | --- |
| [Lab 3](labs/lab-03-glue-catalog-crawlers-athena.md) | Glue Data Catalog, Crawlers, Athena, and Schema Discovery | Glue database, crawler, catalog tables, Athena SQL, partitions |
| [Lab 4](labs/lab-04-glue-etl-data-quality.md) | Glue ETL, Data Quality, and Data Transformation | Glue jobs, transforms, PySpark concepts, data quality checks, output formats |
| [Lab 5](labs/lab-05-redshift-dynamodb-opensearch-data-modeling.md) | Data Modeling with Redshift, DynamoDB, OpenSearch, and RDS | Warehouse, NoSQL, search, relational design, distribution/sort key awareness |

### Domain 3 - Orchestration, Governance, and Operations

| Lab | Title | Focus |
| --- | --- | --- |
| [Lab 6](labs/lab-06-step-functions-mwaa-eventbridge-orchestration.md) | Pipeline Orchestration with Step Functions, MWAA, and EventBridge | Workflow design, retries, scheduling, dependencies, failure handling |
| [Lab 7](labs/lab-07-security-governance-lake-formation-kms.md) | Security, Governance, Lake Formation, KMS, and Data Lifecycle | IAM, KMS, Lake Formation, data permissions, lifecycle, retention |
| [Lab 8](labs/lab-08-monitoring-cost-optimization-exam-review.md) | Monitoring, Cost Optimization, Reliability, and Exam Review | CloudWatch, CloudTrail, Glue metrics, cost controls, architecture review, timed practice |

## Reference

- AWS Certified Data Engineer - Associate: https://aws.amazon.com/certification/certified-data-engineer-associate/
- Course registration: https://www.tertiarycourses.com.sg/wsq-aws-certified-data-engineer-associate-training.html
- AWS Documentation: https://docs.aws.amazon.com/
- AWS Skill Builder: https://skillbuilder.aws/

## Free Tools Used

- AWS Free Tier eligible services where possible
- AWS Management Console
- AWS Glue
- Amazon Athena
- Amazon S3
- AWS Step Functions
- Amazon CloudWatch
- AWS Pricing Calculator
