# Test Plan: SauceDemo (https://www.saucedemo.com)

| | |
|---|---|
| **Version** | 1.0 |
| **Author / Tester** | <Your Name> |
| **Date** | <DD-MMM-YYYY> |
| **Duration** | 5 days |

## 1. Objective
Verify that the core e-commerce flows of SauceDemo (login, inventory, cart, checkout, logout) work as specified, and report defects with clear evidence.

## 2. Scope
**In scope:** Login and error handling, inventory display and sorting, product details, cart add/remove/persistence, checkout (3 steps), logout, Reset App State, direct-URL access control.
**Out of scope:** Performance and load testing, penetration testing, API testing, accessibility audit, mobile native apps.

## 3. Test Approach
Manual, black-box testing. Techniques: equivalence partitioning, boundary value analysis, error guessing, exploratory testing. Test types: functional, negative, boundary, UI, smoke, retest, regression. Requirements were reverse-engineered from observed behaviour (no spec exists) and are listed in the workbook (Requirements sheet).

## 4. Test Environment
| Item | Value |
|---|---|
| OS | <Windows 11 / macOS ...> |
| Browsers | Chrome (latest, primary), Firefox (latest, secondary) |
| URL | https://www.saucedemo.com |
| Users | standard_user, locked_out_user, problem_user, performance_glitch_user, error_user, visual_user (password: secret_sauce) |

## 5. Test Data
Valid checkout: John / Doe / 500081. Invalid: empty fields, special characters, 300-character strings. Products: 6 items priced 7.99 to 49.99; tax rate 8%.

## 6. Entry Criteria
Site reachable; requirements and test cases reviewed; JIRA project and workbook ready.

## 7. Exit Criteria
100% of test cases executed; every requirement has at least one test case; no open Critical or High defects (or documented as known issues); retest and regression completed; summary report signed off.

## 8. Defect Management
Tool: JIRA (project key SD). Workflow: Open, In Progress, Ready for Retest, Closed / Reopened.
Severity: **Critical** (main flow blocked), **Major** (major feature broken, workaround exists), **Minor** (small functional issue), **Trivial** (cosmetic).
Priority: High, Medium, Low.

## 9. Deliverables
Test plan, requirements, 40 test cases, RTM, execution results, defect log with screenshots, retest and regression results, test summary report.

## 10. Risks and Mitigations
| Risk | Mitigation |
|---|---|
| Public demo site may change or go down | Record date and browser version; save screenshots |
| Buggy users behave inconsistently by design | Repeat a failing step twice before logging |
| No developer to fix bugs | Simulate fixes: retest using standard_user as the "fixed build" (documented in report) |

## 11. Schedule
| Day | Activity |
|---|---|
| 1 | Setup, exploration, requirements, test plan |
| 2 | Test cases and RTM |
| 3-4 | Execution and defect logging |
| 5 | Retest, regression, summary report, GitHub upload |
