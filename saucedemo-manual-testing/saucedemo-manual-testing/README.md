# SauceDemo Manual Testing Project

End-to-end manual QA project on [SauceDemo](https://www.saucedemo.com): test planning, test case design, traceability, execution, defect management in JIRA, retest/regression and reporting.

## Project at a glance
| Item | Value |
|---|---|
| Application under test | https://www.saucedemo.com |
| Test cases | 40 (22 positive, 13 negative, 5 boundary) |
| Requirements | 17, all covered by at least one test case |
| Defects logged (JIRA) | <n> (<n> Critical, <n> Major, <n> Minor, <n> Trivial) |
| Pass rate | <n>% |
| Tools | JIRA, Excel/Google Sheets, Chrome DevTools, Git/GitHub |

## Deliverables
| # | Deliverable | Location |
|---|---|---|
| 1 | One-page test plan | [`01-test-plan/Test_Plan.md`](01-test-plan/Test_Plan.md) |
| 2 | Requirements, test cases, RTM, execution results, dashboard, defect log, retest/regression | [`02-test-design-and-execution/SauceDemo_Test_Workbook.xlsx`](02-test-design-and-execution/SauceDemo_Test_Workbook.xlsx) |
| 3 | Defect template and screenshots | [`03-defects/`](03-defects/) |
| 4 | Test summary report | [`04-reports/Test_Summary_Report.md`](04-reports/Test_Summary_Report.md) |

## Workbook sheets
`Requirements` | `Test Cases` (with execution results) | `RTM` (live traceability) | `Dashboard` (live metrics) | `Defect Log` | `Retest & Regression`

## Approach
Black-box manual testing using equivalence partitioning, boundary value analysis and error guessing. Requirements were reverse-engineered from observed behaviour because the site has no specification. Retesting used `standard_user` as the simulated "fixed build" for defects found with the intentionally buggy users (`problem_user`, `error_user`, `visual_user`, `performance_glitch_user`).

## JIRA board
<Insert screenshot of your JIRA board/backlog here: `![JIRA board](03-defects/screenshots/jira-board.png)`>

## Author
<Your Name> | <LinkedIn URL>
