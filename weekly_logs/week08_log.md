# Week 08 Log — IPL Matchday 360

**Week:** 8  
**Date range:** [Add actual Week 8 dates]  
**Team:** [Add team name / number]  
**Project:** IPL Matchday 360

---

## 1. Sprint Goal

Build the first Power BI dashboard draft using Gold-layer outputs only.

Export dashboard-ready Gold data from Databricks, connect it to Power BI, and create an initial dashboard with KPI cards, comparison visuals, and a slicer.

---

## 2. Work Completed

| Task | Owner | Status | Evidence |
|---|---|---|---|
| Created Gold export notebook | [Student] | Done | `notebooks/06_powerbi_export.ipynb` |
| Verified Gold-layer tables for dashboard use | [Student] | Done | `06_powerbi_export.ipynb` |
| Exported dashboard-ready Gold data | [Student] | Done | `06_powerbi_export.ipynb` |
| Created first Power BI dashboard draft | [Student] | Done | `dashboard/powerbi_dashboard.pbix` |
| Added KPI and comparison visuals | [Student] | Done | `screenshots/week08_powerbi_draft.png` |
| Verified Gold-only dashboard connection | [Student] | Done | `screenshots/week08_gold_connection.png` |

---

## 3. Key Decisions

- Power BI was connected to dashboard-ready Gold outputs rather than raw or Bronze data.
- The first dashboard focused on KPI cards, team performance comparison, season filtering, and win-percentage analysis.
- Large raw/detailed datasets were not used directly in Power BI to keep the PBIX focused and manageable.

---

## 4. Blockers / Risks

| Blocker | Impact | Help Needed |
|---|---|---|
| [Add actual blocker, if any] | [Impact] | [Help needed] |

If there were no blockers:

> No major blocker was recorded during Week 8.

---

## 5. Evidence Added to GitHub

- `notebooks/06_powerbi_export.ipynb`
- `dashboard/powerbi_dashboard.pbix`
- `screenshots/week08_powerbi_draft.png`
- `screenshots/week08_gold_connection.png`
- `weekly_logs/week08_log.md`

---

## 6. AI Transparency Note

| Question | Response |
|---|---|
| Where AI helped | AI was used to explain the Power BI export workflow, suggest notebook structure, and assist with troubleshooting SQL/PySpark and dashboard setup. |
| What we changed after AI suggestion | The team adapted the suggested export and dashboard structure to the actual Gold tables available in the Databricks workspace. |
| What we verified manually | Gold table names, table contents, exported data, Power BI connections, dashboard visuals, KPI values, and screenshots were checked manually. |
| What we can explain without AI | The team can explain the Gold-only dashboard approach, the purpose of the exported Gold tables, KPI fields, Power BI visuals, slicers, and how the dashboard connects to the prepared data. |

---

## 7. Next Week Preparation

- Refine the Power BI dashboard layout and visual design.
- Add useful filters and improve dashboard storytelling.
- Document the key insights obtained from the Gold metrics.
