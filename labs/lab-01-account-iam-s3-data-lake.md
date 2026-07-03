# Lab 1 - Account Safety, IAM, S3 Data Lake, and Data Formats

## Objectives

- Configure a safe AWS learning baseline.
- Review IAM roles, policies, and least privilege for data workloads.
- Create an S3 data lake folder structure if permitted.
- Compare CSV, JSON, and Parquet formats.

## Scenario

You are preparing an AWS data engineering workspace. The first step is to create secure access patterns and a clear S3 data lake structure.

## Steps

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

## Deliverables

- IAM and least-privilege notes
- S3 data lake prefix structure
- Data format comparison table
- Encryption and cost safety notes

## Checkpoint

You should be able to explain how IAM, S3 prefixes, encryption, and file formats support a data lake foundation.
