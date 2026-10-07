# Gold Metrics Definition

## 1. Gold Team Match Summary

**Table:** `workspace.default.gold_team_match_summary`

**Grain:** One row per team and season.

### Metrics

- `matches_played` — Number of distinct matches played by the team.
- `matches_won` — Number of completed matches won by the team.
- `no_result_matches` — Number of matches recorded as no-result.
- `tie_matches` — Number of tied matches.
- `completed_matches` — Matches played minus no-result matches.
- `win_percentage` — Matches won divided by completed matches × 100.

---

## 2. Gold Player Batting Summary

**Table:** `workspace.default.gold_player_batting_summary`

**Grain:** One row per player.

### Metrics

- `runs_scored` — Total runs scored by the player.
- `balls_faced` — Total balls faced.
- `boundaries` — Total boundaries.
- `sixes` — Total sixes.
- `strike_rate` — Runs scored × 100 divided by balls faced.

---

## 3. Gold Bowler Performance Summary

**Table:** `workspace.default.gold_bowler_performance_summary`

**Grain:** One row per player.

### Metrics

- `wickets_taken` — Total wickets taken.
- `legal_balls_bowled` — Total legal balls bowled.
- `chargeable_runs` — Total chargeable runs conceded.
- `overs` — Legal balls converted into cricket overs.
- `economy_rate` — Chargeable runs × 6 divided by legal balls bowled.

---

## 4. Gold Venue Phase Summary

**Table:** `workspace.default.gold_venue_phase_summary`

**Grain:** One row per venue and innings phase.

### Metrics

- `runs` — Total runs scored.
- `legal_balls` — Number of legal deliveries.
- `deliveries` — Number of deliveries.
- `run_rate` — Runs × 6 divided by legal balls.

### Innings Phases

- Powerplay: overs below 6
- Middle: overs 6 to below 15
- Death: overs 15 and above

---

## 5. Gold DQ and Live Summary

**Table:** `workspace.default.gold_dq_and_live_summary`

**Grain:** One row per season.

### Metrics

- `total_matches` — Distinct matches for the season.
- `team_wins` — Total team wins.
- `no_result_matches` — Number of no-result matches.
- `tie_matches` — Number of tied matches.
- `summary_status` — Validation status for the summary.
