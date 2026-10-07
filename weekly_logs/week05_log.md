# Week 05 Log — IPL Matchday 360

**Week:** 5
**Date range:** 7th August to 13th August
**Team:** Team 01
**Project:** IPL Matchday 360

---

## 1. Sprint Goal

Transform the Bronze IPL data into clean Silver tables with standardized fields and appropriate data types. Validate the Silver tables and document a clear raw-to-Silver transformation mapping.

---

## 2. Work Completed

| Task                                                               | Owner     | Status | Evidence                                       |
| ------------------------------------------------------------------ | --------- | ------ | ---------------------------------------------- |
| Read Bronze IPL tables from the workspace                          | [Student] | Done   | `notebooks/03_silver_transformations.ipynb`    |
| Created Silver tables for deliveries, matches, players, and venues | [Student] | Done   | `notebooks/03_silver_transformations.ipynb`    |
| Standardized and cleaned Silver fields                             | [Student] | Done   | `notebooks/03_silver_transformations.ipynb`    |
| Checked Silver schemas and data types                              | [Student] | Done   | `screenshots/week05_silver_schema.png`         |
| Validated Bronze-to-Silver record counts                           | [Student] | Done   | `notebooks/03_silver_transformations.ipynb`    |
| Documented a raw-to-Silver transformation mapping                  | [Student] | Done   | `screenshots/week05_raw_to_silver_mapping.png` |

---

## 3. Key Decisions

* Used the Bronze tables in `workspace.default` as the source for the Silver transformations.
* Applied cleaning and standardization while preserving the required record-level information in the Silver layer.

---

## 4. Blockers / Risks

| Blocker         | Impact          | Help Needed |
| --------------- | --------------- | ----------- |
| None identified | No major impact | None        |

---

## 5. Evidence Added to GitHub

* `notebooks/03_silver_transformations.ipynb`
* `screenshots/week05_silver_schema.png`
* `screenshots/week05_raw_to_silver_mapping.png`
* `weekly_logs/week05_log.md`

---

## 6. AI Transparency Note

| Question                            | Response                                                                                                                                   |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Where AI helped                     | AI helped with understanding Silver-layer standardization, transformation logic, and organizing the evidence required for the sprint.      |
| What we changed after AI suggestion | We reviewed the suggested transformation approach and adapted it to the actual Bronze tables and columns used in the project.              |
| What we verified manually           | We manually checked the Silver table schemas, sample records, and Bronze-to-Silver record counts in Databricks.                            |
| What we can explain without AI      | We can explain the purpose of the Silver layer, field standardization, data cleaning, data-type handling, and Bronze-to-Silver validation. |

---

## 7. Next Week Preparation

* Run meaningful data-quality checks on the Silver data.
* Prepare null, duplicate, range, and reference checks and capture failed examples.
