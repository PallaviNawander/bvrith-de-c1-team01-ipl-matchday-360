# Week 03 Log — Databricks Setup + Data Exploration

**Week:** 3
**Date range:** 24 July – 30 July 
**Team:** [Team name / 01]
**Project:** IPL Matchday 360

---

## 1. Sprint Goal

The goal of this week was to set up the Databricks environment and explore the IPL dataset to understand its structure, schema, and data characteristics.

The focus was on loading the sample data, inspecting schemas, checking row counts, and identifying potential data quality issues to prepare for the upcoming Bronze ingestion stage.

---

## 2. Work Completed

| Task                                                                 | Owner     | Status | Evidence                            |
| -------------------------------------------------------------------- | --------- | ------ | ----------------------------------- |
| Set up / accessed the Databricks workspace                           | [Student] | Done   | Databricks workspace                |
| Loaded sample IPL data into Databricks                               | [Student] | Done   | `week03_databricks_data_loaded.png` |
| Explored dataset schemas and column types                            | [Student] | Done   | `week03_schema_and_row_count.png`   |
| Checked row counts                                                   | [Student] | Done   | `01_data_exploration.ipynb`         |
| Performed initial data profiling and checked nulls / quality signals | [Student] | Done   | `01_data_exploration.ipynb`         |
| Updated Week 3 documentation                                         | [Student] | Done   | `weekly_logs/week03_log.md`         |

---

## 3. Key Decisions

* Used the IPL Matchday 360 project data for the initial Databricks exploration.
* Performed schema, row-count, and basic data-quality checks before beginning Bronze ingestion.
* Kept the exploration focused on understanding the raw data rather than applying transformations at this stage.

---

## 4. Blockers / Risks

| Blocker                                         | Impact | Help Needed |
| ----------------------------------------------- | ------ | ----------- |
| No major blocker encountered during the sprint. | —      | None        |

---

## 5. Evidence Added to GitHub

* `notebooks/01_data_exploration.ipynb` — Databricks data loading and profiling notebook.
* `screenshots/week03_databricks_data_loaded.png` — Data loading evidence.
* `screenshots/week03_schema_and_row_count.png` — Schema, row count, and profiling evidence.
* `weekly_logs/week03_log.md` — Week 3 sprint log and AI Transparency Note.

---

## 6. AI Transparency Note

| Question                            | Response                                                                                                                                                                                   |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Where AI helped                     | AI assistance was used to understand the Week 3 requirements, clarify Databricks and Spark SQL concepts, and support the structuring of the exploration notebook and weekly documentation. |
| What we changed after AI suggestion | The suggested approach was adapted to the actual IPL Matchday 360 project structure, datasets, and Databricks workflow.                                                                    |
| What we verified manually           | Data loading, schemas, row counts, profiling results, screenshots, and notebook outputs were verified against the actual Databricks execution.                                             |
| What we can explain without AI      | We can explain how the data was loaded, how its schema and row count were inspected, how basic profiling was performed, and why these checks are required before Bronze ingestion.         |

---

## 7. Next Week Preparation

* Prepare the raw IPL datasets for Bronze ingestion.
* Create or update the Bronze ingestion notebook.
* Load the raw source data into Bronze tables.
* Add ingestion metadata.
* Compare raw and Bronze record counts.
