# Week 06 Log — Data Quality Checks

**Week:** 6  
**Date range:** 14th August to 20th August
**Team:** Team 01
**Project:** IPL Matchday 360

---

## 1. Sprint Goal

Run meaningful data quality checks on the IPL data, identify failed records, and separate trusted records from quarantined records. Validate that candidate records are fully accounted for between the trusted and quarantine datasets.

---

## 2. Work Completed

| Task | Owner | Status | Evidence |
|---|---|---|---|
| Applied data quality rules to matches, deliveries, players, and venues | [Student] | Done | `notebooks/04_data_quality_checks.ipynb` |
| Separated PASS records into Trusted Silver and FAIL records into Quarantine | [Student] | Done | `notebooks/04_data_quality_checks.ipynb` |
| Performed candidate vs trusted + quarantine reconciliation | [Student] | Done | `week06_dq_results.png` |
| Captured failed records and their DQ rule IDs/reasons | [Student] | Done | `week06_failed_records_sample.png` |
| Created and saved the Week 6 DQ summary | [Student] | Done | `workspace.default.dq_summary` |

---

## 3. Key Decisions

- Records passing the defined DQ checks were routed to Trusted Silver datasets.
- Records failing DQ checks were routed to corresponding Quarantine datasets so that failed records were retained for investigation and rework.

---

## 4. Blockers / Risks

| Blocker | Impact | Help Needed |
|---|---|---|
| [Add actual blocker, or write "None"] | [Add impact, or "N/A"] | [Add help needed, or "None"] |

---

## 5. Evidence Added to GitHub

- `notebooks/04_data_quality_checks.ipynb`
- `screenshots/week06_dq_results.png`
- `screenshots/week06_failed_records_sample.png`
- `docs/data_quality_summary.md`
- `src/data_quality_rules.py` [if updated]

---

## 6. AI Transparency Note

| Question | Response |
|---|---|
| Where AI helped | AI was used to help understand data quality checks, debug transformation logic, and structure parts of the DQ workflow. |
| What we changed after AI suggestion | We reviewed and adapted the suggested logic to match the IPL project tables, DQ rule structure, and Trusted/Quarantine workflow. |
| What we verified manually | We manually checked DQ outputs, failed-record examples, candidate/trusted/quarantine counts, and reconciliation results in Databricks. |
| What we can explain without AI | We can explain the purpose of DQ rules, the PASS/FAIL classification, quarantine handling, and candidate-to-trusted/quarantine reconciliation. |

---

## 7. Next Week Preparation

- Create dashboard-ready Gold tables and aggregations.
- Validate Gold metrics and document their definitions and grain.
