# Contractor badge expiry review

**Exercise date:** 3 November 2026 · **Owner:** Site Security Manager · **Scope:** Three synthetic contractor approvals expiring on 2 November. Each badge has one approval window. Times are UTC. HDIIA is fictional.

## Decision

Keep FAC-01 open. One of three badges has verified on-time deactivation (33.3%). Badge B exceeded its authorised window by 84 minutes. The status of badge C at expiry is undetermined.

## Repeat the test

1. Start with all three rows in [approvals.csv](approvals.csv). Starting with deactivations would silently exclude C.
2. Match the badge ID to [deactivations.csv](deactivations.csv). Preserve unmatched approvals. Confirm unique IDs and consistent timestamps before comparison.
3. Subtract approved expiry from actual deactivation. At or before expiry passes; a positive interval is late. A missing record requires follow-up.
4. Compare the results below. An assertion from the guarding team that C was disabled is a synthetic interview statement. It does not establish the time of deactivation.

| Badge | Difference | Finding | Action |
|---|---:|---|---|
| A | −1 min | Timely | Retain the matched approval and event. |
| B | +84 min | Late | Confirm deactivation, review entry events during the interval and investigate the delay. |
| C | Unknown | Insufficient evidence | Verify current badge state and request an attributable, timestamped historical record. |

No entry events were supplied. Actual use during B’s exposure window is unknown. A current disabled state for C would resolve present exposure; its historical timeliness still requires dated evidence.

## Remediation and retest

Access Administration owns the proposed configuration change. Test automatic expiry with a new temporary badge and retain the approval and timestamped expiry event. Site Security independently reviews the next period for completeness and rechecks exceptions. Record B's original late result even after correction. If C's history cannot be recovered, record the evidence gap and escalate to the risk owner. Closure requires recorded disposition of both exceptions and a successful retest. All actions are proposed; no remediation execution is asserted.

## Interpretation

This deliberately small exercise demonstrates a test method. It cannot establish the frequency of failures across a real facility. References: [NIST control catalogue](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final) and [ENISA technical guidance](https://www.enisa.europa.eu/publications/nis2-technical-implementation-guidance).
