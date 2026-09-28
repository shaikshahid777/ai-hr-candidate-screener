# Validation Report

## Test Matrix

| Test | Scenario | Expected Rule | Result |
|---|---|---|---|
| 01 | Strong candidate | Rule 6 | ✅ PASS |
| 02 | Vague / unclear resume tasks | Rule 5 | ✅ PASS |
| 03 | No experience + 3 relevant certifications | Rule 3 | ✅ PASS |
| 04 | Missing email and phone | Rule 1 | ✅ PASS |
| 05 | 2+ year experience shortfall + no relevant certification | Rule 2 | ✅ PASS |
| 06 | Candidate matches multiple open positions | Rule 4 | ✅ PASS |

## Validation Notes

The tests were designed as dedicated scenarios so that the intended rule could be demonstrated against explicit document evidence.

The multiple-options scenario correctly identified a strongest skill match and listed an alternative position fit. The other scenarios demonstrated the required STRONG, BORDERLINE, and WEAK classifications and corresponding actions.
