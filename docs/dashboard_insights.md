# Dashboard Insights

**Week:** 9  
**Purpose:** Explain what the Power BI dashboard shows.

---

## 1. Dashboard Pages

| Page | Purpose | Main Visuals |
|---|---|---|
| Page 1: Executive Overview | High-level summary of IPL matches, seasons, teams, and venues | KPI cards, Matches by Season, Team Wins, Season filter |
| Page 2: Team & Match Analysis | Compare team performance and match activity across seasons | Team Wins, Matches by Season, Team Performance table, Win Percentage, Season filter |
| Page 3: Venue & Data Quality | Analyze match distribution across venues and provide a summary of data quality | Matches by Venue, Data Quality & Match Summary, KPI cards, Season filter |

---

## 2. Key Insights

1. The dashboard covers **476 IPL matches** across **5 seasons**, involving **10 teams** and **16 venues**.

2. The Executive Overview provides a quick summary of the tournament dataset through KPI cards and season-wise match trends.

3. The Matches by Season visual allows users to compare the number of matches played across the available seasons.

4. The Team Wins analysis provides a comparison of team performance based on the number of matches won.

5. The Team & Match Analysis page combines team match counts, total wins, and win percentage to provide a more detailed view of team performance.

6. The season filter allows users to interactively analyze match and team performance for a particular season.

7. The Venue & Data Quality page shows how matches are distributed across the available IPL venues.

8. The Data Quality & Match Summary section provides information such as total matches, team wins, tie matches, no-result matches, and summary status from the Gold-layer data.

---

## 3. How the Dashboard Uses Gold Tables

| Dashboard Page | Gold Table Used | Important Fields |
|---|---|---|
| Page 1: Executive Overview | `gold_team_match_summary` | `season`, `team_id`, team performance fields |
| Page 2: Team & Match Analysis | `gold_team_match_summary` | `season`, `team_id`, team match and win information |
| Page 3: Venue & Data Quality | `gold_dq_and_live_summary` | `season`, `summary_status`, `team_wins`, `tie_matches`, `no_result_matches`, `total_matches` |

---

## 4. Power BI Validation

- [ ] Dashboard connects to Gold outputs and required dimension tables only.
- [ ] Filters work correctly.
- [ ] KPI totals match the underlying dataset checks.
- [ ] Screenshots are saved in `screenshots/`.
- [ ] Dashboard story is explainable by all students.
