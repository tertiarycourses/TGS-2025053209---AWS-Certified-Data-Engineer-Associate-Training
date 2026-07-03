# Lab 7 - Security, Governance, Lake Formation, KMS, and Data Lifecycle

## Objectives

- Review data security controls for AWS data platforms.
- Understand Lake Formation permissions.
- Review KMS encryption and key policies.
- Apply lifecycle, retention, and data governance concepts.

## Scenario

Data engineering work must protect sensitive data, control access, encrypt assets, and manage data lifecycle. This lab focuses on governance and security service choices.

## Steps

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

## Deliverables

- Data governance service table
- Lake Formation permission notes
- KMS encryption notes
- Lifecycle and retention design

## Checkpoint

You should be able to explain how IAM, S3, KMS, Lake Formation, Macie, lifecycle rules, and audit logs protect data platforms.
