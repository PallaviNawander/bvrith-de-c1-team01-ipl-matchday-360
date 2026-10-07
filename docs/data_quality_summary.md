# Data Quality Summary

**Week:** 6  
**Purpose:** Summarize data quality rules, failures and business impact.

---

## 1. Quality Rule Results

The Week 6 notebook implements the following IPL-specific data quality rules.

| Rule ID | Rule Name | Severity | Passed Count | Failed Count | Business Impact |
|---|---|---|---:|---:|---|
| DQ-IPL-001 | Required ID / duplicate check | High | Not separately aggregated | Not separately aggregated | Missing or duplicate identifiers can make records unreliable and distort downstream metrics |
| DQ-IPL-002 | Referential integrity check | High | Not separately aggregated | Not separately aggregated | Invalid references can cause incorrect joins between matches, venues, players, and deliveries |
| DQ-IPL-003 | Team integrity check | High | Not separately aggregated | Not separately aggregated | Invalid or inconsistent team relationships can produce incorrect match and team-level metrics |
| DQ-IPL-004 | Cricket sequence check | Medium | Not separately aggregated | Not separately aggregated | Invalid innings, over, ball, or duplicate sequence values can affect delivery-level analysis |
| DQ-IPL-005 | Runs validation | High | Not separately aggregated | Not separately aggregated | Invalid run values can produce incorrect scoring and performance metrics |
| DQ-IPL-006 | Wicket consistency check | High | Not separately aggregated | Not separately aggregated | Inconsistent wicket information can affect player and bowler performance metrics |
| DQ-IPL-007 | Match result / winner consistency | High | Not separately aggregated | Not separately aggregated | Incorrect winner information can distort team win and match outcome metrics |
| DQ-IPL-008 | Innings reconciliation | High | Not separately aggregated | Not separately aggregated | Mismatches between calculated and declared innings scores can make scoring metrics unreliable |

### Overall DQ Results

| Entity | Candidate Count | Trusted Count | Quarantine Count | Reconciliation |
|---|---:|---:|---:|---|
| Matches | 500 | 476 | 24 | PASS |
| Deliveries | 119879 | 0 | 119879 | PASS |
| Players | 250 | 250 | 0 | PASS |
| Venues | 16 | 16 | 0 | PASS |

The reconciliation check confirms that:

**Candidate Count = Trusted Count + Quarantine Count**

for all four entities.

---

## 2. Failed Record Examples

| Rule ID | Sample Record ID | Failure Reason | Action / Handling |
|---|---|---|---|
| DQ-IPL-003 | `SRC-DLV-0000001` | Team integrity check failed | Record routed to Quarantine for investigation and rework |
| DQ-IPL-003 | `SRC-MAT-00005` | Match teams are invalid or identical | Match routed to Quarantine |

The delivery example belongs to match `M2022-001` and has
`DQ-IPL-003` recorded as its failed rule.

---

## 3. What Should Block Gold Metrics?

The project routes failed records to Quarantine and allows only PASS records into Trusted Silver.

Therefore, any record failing a DQ rule should be prevented from directly contributing to Gold metrics until it is corrected or otherwise resolved.

The following rules should block the affected records from Gold processing:

- **DQ-IPL-001** — Missing or duplicate identifiers can make records unreliable.
- **DQ-IPL-002** — Invalid references can produce incorrect joins.
- **DQ-IPL-003** — Invalid team relationships can affect match and team metrics.
- **DQ-IPL-004** — Invalid cricket sequence information can affect delivery analysis.
- **DQ-IPL-005** — Invalid run values can affect scoring metrics.
- **DQ-IPL-006** — Inconsistent wicket information can affect player and bowling metrics.
- **DQ-IPL-007** — Inconsistent match result information can affect team performance metrics.
- **DQ-IPL-008** — Innings score mismatches can affect scoring and match-level metrics.

---

## 4. Quality Summary

The Week 6 DQ process successfully classified records into Trusted Silver and Quarantine datasets and performed reconciliation checks. The match dataset contained 500 candidate records, of which 476 passed and 24 were quarantined. The delivery dataset contained 119879 candidate records and all 119879 were routed to Quarantine, making delivery-level Gold metrics unsuitable until the failures are resolved. All 250 player records and all 16 venue records passed the implemented checks. Failed examples show that team integrity and innings reconciliation issues are present in the delivery data. The notebook also records a match-level team integrity failure for `M2022-005`. The delivery quarantine should therefore be reviewed carefully before using delivery-based data for Gold metrics and dashboard calculations.
