# Lab 4 - Glue ETL, Data Quality, and Data Transformation

## Objectives

- Review Glue ETL job concepts.
- Design a transform from raw to curated data.
- Understand PySpark and visual ETL options.
- Add data quality checks and output-format decisions.

## Scenario

Raw data often needs cleaning, validation, transformation, and conversion to analytics-friendly formats. You will design or run a small ETL workflow.

## Steps

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

## Deliverables

- ETL design notes or job screenshot
- Raw-to-curated transformation checklist
- Data quality rule list
- Output format decision notes

## Checkpoint

You should be able to describe how Glue ETL transforms and validates data before analytics consumption.
