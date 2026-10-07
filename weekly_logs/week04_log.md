# Week 04 Log — IPL Matchday 360

**Week:** 4
**Date range:** 31st July to 6th August
**Team:** Team 01
**Project:** IPL Matchday 360

---

## 1. Sprint Goal

Create the Bronze layer by loading the raw IPL source data into Bronze tables while preserving the raw data. Add ingestion metadata such as the source file, ingestion timestamp, and ingestion run identifier, and reconcile the source and Bronze record counts.

---

## 2. Work Completed

| Task                                       | Owner     | Status | Evidence                                                                 |
| ------------------------------------------ | --------- | ------ | ------------------------------------------------------------------------ |
| Loaded raw IPL source files                | [Student] | Done   | `notebooks/02_bronze_ingestion.ipynb`                                    |
| Created Bronze tables for the IPL datasets | [Student] | Done   | `notebooks/02_bronze_ingestion.ipynb`, `week04_bronze_table_created.png` |
| Added Bronze ingestion metadata            | [Student] | Done   | `notebooks/02_bronze_ingestion.ipynb`, `week04_bronze_table_created.png` |
| Compared source and Bronze record counts   | [Student] | Done   | `week04_bronze_counts.png`                                               |

---

## 3. Key Decisions

* Preserved the raw source data in the Bronze layer without applying unnecessary transformations.
* Added ingestion metadata to the Bronze tables to track the source file, ingestion timestamp, and ingestion run.

---

## 4. Blockers / Risks

| Blocker                               | Impact                  | Help Needed                  |
| ------------------------------------- | ----------------------- | ---------------------------- |
| [Add actual blocker, or write "None"] | [Add impact, or "None"] | [Add help needed, or "None"] |

---

## 5. Evidence Added to GitHub

* `notebooks/02_bronze_ingestion.ipynb`
* `screenshots/week04_bronze_table_created.png`
* `screenshots/week04_bronze_counts.png`
* `weekly_logs/week04_log.md`

---

## 6. AI Transparency Note

| Question                            | Response                                                                                                      |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| Where AI helped                     | AI was used for guidance on Bronze ingestion logic, metadata handling, and organizing the required evidence.  |
| What we changed after AI suggestion | [Describe the changes actually made after reviewing the AI suggestion.]                                       |
| What we verified manually           | The Bronze tables, metadata columns, and source-versus-Bronze counts were checked in Databricks.              |
| What we can explain without AI      | We can explain the Bronze layer purpose, raw data preservation, ingestion metadata, and count reconciliation. |

---

## 7. Next Week Preparation

* Create and standardize the Silver tables from the Bronze layer.
* Check Silver schemas, data types, field names, and raw-to-Silver mappings.
