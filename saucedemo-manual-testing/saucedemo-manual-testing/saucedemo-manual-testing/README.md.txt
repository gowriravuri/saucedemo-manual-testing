# SauceDemo Manual Testing Project

End-to-end manual QA project on [SauceDemo](https://www.saucedemo.com): test planning, test case design, requirements traceability, execution, defect management in JIRA, retest, regression and reporting.

## Project at a glance
| Item | Value |
|---|---|
| Application under test | https://www.saucedemo.com |
| Requirements | 17 (100% covered by at least one test case) |
| Test cases | 40 (22 positive, 13 negative, 5 boundary) |
| Executed | 40 of 40 (100%) |
| Passed / Failed / Blocked | 34 / 6 / 0 |
| **Pass rate** | **85%** |
| Defects logged (JIRA) | 6 (2 Critical, 4 Major) |
| Defect status after retest | 4 Closed, 2 Reopened |
| Regression | 6 cases run: 4 passed, 2 failed |
| Release recommendation | **Not ready**: empty-cart defects still open |
| Tools | JIRA, Excel / Google Sheets, Chrome, Git / GitHub |

## Key findings
| Defect | Area | Severity | Status |
|---|---|---|---|
| KAN-5| Cart: checkout page opens with an empty cart (TC26) | Major | Reopened |
| KAN-6 | Checkout: order completes with no items (TC27) | Major | Reopened |
| KAN-7 | Inventory: wrong product images for problem_user (TC37) | Major | Closed |
| KAN-8 | Inventory: sorting does not work for problem_user (TC38) | Major | Closed |
| KAN-9 | Checkout: entered data not retained for problem_user (TC39) | Critical | Closed |
| KAN-10 | Cart: add/remove fails for error_user (TC40) | Critical | Closed |

## Deliverables
| # | Deliverable | Location |
|---|---|---|
| 1 | One-page test plan | [`01-test-plan/Test_Plan.md`](01-test-plan/Test_Plan.md) |
| 2 | Requirements, test cases, RTM, execution results, dashboard, defect log, retest and regression | [`02-test-design-and-execution/SauceDemo_Test_Workbook.xlsx`](02-test-design-and-execution/SauceDemo_Test_Workbook.xlsx) |
| 3 | Defect template and screenshots | [`03-defects/`](03-defects/) |
| 4 | Test summary report | [`04-reports/Test_Summary_Report.md`](04-reports/Test_Summary_Report.md) |

## Workbook sheets
`Requirements` | `Test Cases` (with execution and regression results) | `RTM` | `Dashboard` | `Defect Log` | `Retest & Regression`

## Approach
- Black-box manual testing using equivalence partitioning, boundary value analysis and error guessing.
- Requirements were reverse-engineered from observed behaviour because the site has no specification.
- Tests were run with `standard_user`, `locked_out_user`, `problem_user` and `error_user`.
- SauceDemo's code cannot be changed, so retest used `standard_user` as the simulated "fixed build". This is a simulated fix check, not a real developer fix.
- The two empty-cart defects are not user-specific, so they stayed open after retest.

## Limitations
- Regression covered 6 of 40 test cases (15%), not the full suite.
- `visual_user` and `performance_glitch_user` were not tested.
- Some expected results are assumptions (for example, REQ-17: empty cart blocks checkout).

## JIRA board
<Add a screenshot: `![JIRA board](03-defects/screenshots/jira-board.png)`>

## Author
<Your Name> | <LinkedIn URL>
