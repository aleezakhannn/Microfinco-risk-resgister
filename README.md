# MicroFinCo ISO 27001 Risk Register

A fictional risk register for MicroFinCo, built from the findings of an ISO/IEC 27001 Annex A gap analysis. Each gap (a control marked Partial or Not) is turned into a risk, scored by impact and likelihood, and given a suggested mitigation.

## Files

- [risk_register.csv](risk_register.csv): the risk register (12 risks)
- [iso27001_gap_analysis.csv](iso27001_gap_analysis.csv): the source gap analysis (35 controls)

## Risk Register Columns

| Column | Description |
|---|---|
| Risk ID | Unique ID (R-001, R-002, ...) |
| Description | Short description of the risk and the related Annex A control |
| Impact | Severity if the risk occurs, 1 (low) to 5 (high) |
| Likelihood | Chance of the risk occurring, 1 (rare) to 5 (almost certain) |
| Score | Impact x Likelihood (maximum 25) |
| Mitigation | Suggested action aligned with the control recommendation |

## Scoring Method

- **Score = Impact x Likelihood**
- Rows are sorted by score, highest first, so the most urgent risks appear at the top.
- Suggested reading of scores: 15-25 high, 8-14 medium, below 8 low.

## Summary

- **Gap analysis source:** 35 controls evaluated (14 Implemented, 14 Partial, 7 Not)
- **Risks derived:** 12, taken from Partial and Not controls
- **Highest score:** 20 (lack of MFA for privileged accounts, no incident response plan)
- **Lowest score:** 8 (business continuity plan never tested)

## Limitations

This is a training exercise. MicroFinCo, its evidence, and all scores are fictional. Scores are illustrative and not based on a real risk assessment. Not every gap from the analysis was converted into a risk.