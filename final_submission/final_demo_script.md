# Final Demo Script

**Week:** 12
**Project:** IPL Matchday 360
**Team:** ZENAIZ × BVRIT Hyderabad
**Time Target:** 10–15 minutes

## 1. Opening — 1 minute

* Introduce the team members: Dhanalakshmi, Mounika Punna, and Pallavi Nawander.
* Introduce IPL Matchday 360 and explain the engineering problem the project addresses.
* Summarize the outcome: a data engineering pipeline that transforms raw IPL data into structured, quality-checked data for analytics, along with a streaming simulation.

## 2. Architecture Walkthrough — 2 minutes

Explain the overall architecture:

**Raw Sources → Bronze → Silver → Data Quality → Gold → Power BI → Streaming Simulation**

Briefly describe the purpose of each stage, from raw data ingestion to standardized data, quality validation, analytical outputs, dashboard visualization, and simulated streaming events.

## 3. Dataset and Source Design — 2 minutes

* Show the source files used in the project.
* Explain the dataset structure, keys, and assumptions.
* Identify the controlled data quality issues introduced for validation.
* Explain how the pipeline handles valid and invalid records.

## 4. Databricks Pipeline — 4 minutes

* Demonstrate raw data ingestion and Bronze table creation.
* Show Silver tables and explain standardization and transformations.
* Demonstrate the data quality checks and explain how invalid records are handled.
* Show the Gold tables and explain the metrics derived from the validated data.

## 5. Power BI Dashboard — 2 minutes

* Open the IPL Matchday 360 dashboard.
* Explain the KPI cards, trends, filters, and key insights.
* Show how the dashboard presents the processed analytical data.

## 6. Streaming Simulation — 2 minutes

* Show the JSON event files used in the simulation.
* Explain the Auto Loader / Structured Streaming workflow.
* Demonstrate the streaming output and the live-health metric.
* Clarify that the implementation is a simulation and describe its processing behavior accurately.

## 7. Closing — 1 minute

* Summarize the team's learning across data ingestion, transformation, data quality, analytics, and streaming.
* Mention the project's limitations and potential future improvements.
* Thank the mentors and reviewers.
