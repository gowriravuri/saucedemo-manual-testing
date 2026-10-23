# Test Summary Report: SauceDemo

> Fill every `<...>` from the **Dashboard** sheet of the workbook after execution. Delete this note before submitting.

## 1. Overview
| | |
|---|---|
| Application | SauceDemo (https://www.saucedemo.com) |
| Test period | <start date> to <end date> |
| Tester | <Your Name> |
| Test type | Manual functional testing |

## 2. Scope
**Tested:** login, inventory, sorting, product details, cart, checkout, logout, reset app state, direct URL access.
**Not tested:** performance/load, security penetration, API, accessibility, mobile apps.

## 3. Environment
OS: <...> | Browsers: Chrome <version>, Firefox <version> | Users: standard_user, locked_out_user, problem_user, performance_glitch_user, error_user, visual_user

## 4. Test Execution Summary
| Metric | Count |
|---|---|
| Total test cases | 40 |
| Executed | <n> |
| Passed | <n> |
| Failed | <n> |
| Blocked | <n> |
| Not Run | <n> |
| **Pass rate** | <n>% |

Test types: Positive 22, Negative 13, Boundary 5.

*(Insert pie chart: pass / fail / blocked)*

## 5. Defect Summary
| Severity | Count |
|---|---|
| Critical | <n> |
| Major | <n> |
| Minor | <n> |
| Trivial | <n> |
| **Total** | <n> |

Open: <n> | Closed: <n> | Reopened: <n>

Defects by module: Login <n>, Inventory <n>, Cart <n>, Checkout <n>, Other <n>

*(Insert bar chart: defects by severity)*

Top defects: SD-<n> <title>; SD-<n> <title>; SD-<n> <title>

## 6. Requirements Coverage
17 requirements, <n> covered by at least one test case = <n>% coverage. Requirements with failures: <REQ-xx, ...>. See RTM sheet.

## 7. Retest and Regression
**Retest approach:** SauceDemo's code cannot be modified, so `standard_user` was used as the "fixed build" and each defect's steps were re-run. This is a simulated fix verification, not a real developer fix.
- Defects retested: <n> | Closed: <n> | Reopened: <n>
- Regression: <n> cases re-run, <n> passed, <n> failed

## 8. Risks and Known Issues
- <e.g. Unfixed Major defects: SD-x, SD-y>
- Requirements were reverse-engineered, so expected results carry assumptions (e.g. REQ-17).
- Public demo site behaviour may change over time.

## 9. Lessons Learned and Recommendations
- <What worked: e.g. testing the same flow across user types found most defects>
- <What you would improve: e.g. automate the regression suite>
- <Recommendation to dev team>

## 10. Exit Criteria Check
| Criterion | Met? |
|---|---|
| 100% test cases executed | <Yes/No> |
| All requirements covered | <Yes/No> |
| No open Critical/High defects | <Yes/No> |
| Retest and regression done | <Yes/No> |

**Recommendation:** <Ready / Not ready for release, because ...>

Prepared by: <Your Name>   Date: <DD-MMM-YYYY>
