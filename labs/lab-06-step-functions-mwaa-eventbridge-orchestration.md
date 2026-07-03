# Lab 6 - Pipeline Orchestration with Step Functions, MWAA, and EventBridge

## Objectives

- Understand orchestration and scheduling choices.
- Compare Step Functions, MWAA, Glue Workflows, and EventBridge.
- Design pipeline dependencies, retries, and failure handling.
- Create a simple workflow diagram.

## Scenario

Data pipelines need scheduling, sequencing, dependency management, error handling, and monitoring. This lab teaches orchestration design patterns.

## Steps

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

## Deliverables

- Orchestration service comparison table
- Daily pipeline design
- Retry and failure-handling notes
- Monitoring points

## Checkpoint

You should be able to design a simple data pipeline orchestration flow and justify the orchestration service choice.
