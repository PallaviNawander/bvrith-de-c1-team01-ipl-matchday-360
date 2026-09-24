# Week 09 Log — Power BI Dashboard Development

**Week:** 9  
**Date range:** 18 Sep 2026 – 24 Sep 2026  
**Team:**  Team 01  
**Project:** IPL Matchday 360

---

## 1. Sprint Goal

Build and validate the Power BI dashboard for IPL Matchday 360 using the available Gold-layer outputs and supporting dimension/fact tables.

Create three dashboard pages covering the overall IPL overview, team and match analysis, and venue/data quality insights.

---

## 2. Work Completed

| Task | Owner | Status | Evidence |
|---|---|---|---|
| Created Executive Overview page | Team | Done | Power BI dashboard screenshot |
| Added KPI cards for matches, seasons, teams, and venues | Team | Done | Power BI dashboard screenshot |
| Created Matches by Season visual | Team | Done | Power BI dashboard screenshot |
| Created Team Wins visual | Team | Done | Power BI dashboard screenshot |
| Created Team & Match Analysis page | Team | Done | Power BI dashboard screenshot |
| Added Team Matches, Total Wins, and Win Percentage measures | Team | Done | Power BI report |
| Created Team Performance table | Team | Done | Power BI dashboard screenshot |
| Created Venue & Data Quality page | Team | Done | Power BI dashboard screenshot |
| Added No Result Matches and Tie Matches measures | Team | Done | Power BI report |
| Added Data Quality & Match Summary table | Team | Done | Power BI dashboard screenshot |
| Added season filters and dashboard formatting | Team | Done | Power BI dashboard |

---

## 3. Key Decisions

- Designed the Power BI dashboard as three pages: Executive Overview, Team & Match Analysis, and Venue & Data Quality.
- Used the available populated Gold tables and supporting dimension/fact tables instead of building visuals from empty player and bowling Gold tables.
- Kept the dashboard focused on match, team, venue, and data-quality insights for the current dataset.

---

## 4. Blockers / Risks

| Blocker | Impact | Help Needed |
|---|---|---|
| Player batting and bowling Gold tables currently contain no rows | Player and bowling analysis could not be included in the dashboard | Populate and validate the required Gold tables |
| Some data-quality fields may contain blank values | KPI cards may require blank handling | Validate Gold-layer outputs |
| Dashboard validation depends on the correctness of the underlying Gold and supporting tables | Incorrect source data could affect dashboard insights | Final data-quality validation |

---

## 5. Evidence Added to GitHub

- Power BI dashboard/report updated
- Dashboard screenshots added to `screenshots/`
- Dashboard Insights documentation updated
- Week 09 sprint log updated

---

## 6. AI Transparency Note

| Question | Response |
|---|---|
| Where AI helped | AI helped with Power BI dashboard planning, visual selection, DAX measure creation, layout suggestions, and troubleshooting Power BI configuration issues. |
| What we changed after AI suggestion | The team adapted the suggested dashboard structure and measures to match the actual tables, columns, and available data in the project. |
| What we verified manually | KPI values, table fields, relationships, visual outputs, filters, and Gold-table values were checked manually in Power BI. |
| What we can explain without AI | The team can explain the dashboard structure, data flow, KPI calculations, DAX measures, visualizations, filters, and the insights shown by the dashboard. |

---

## 7. Next Week Preparation

- Validate the complete Power BI dashboard against the Gold-layer outputs.
- Capture and organize final dashboard screenshots.
- Start preparing for the streaming step of the project.
