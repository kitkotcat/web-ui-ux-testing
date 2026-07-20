# Tor Store Web Application Testing

Manual black-box testing and test design for the **Tor Store** web application.

The project demonstrates functional testing, partial smoke execution, negative testing, UI comparison with a supplied design mockup, responsive checks and technical analysis with Chrome DevTools.

## Application under test

| Parameter | Value |
|---|---|
| Application | Tor Store |
| Platform | Web |
| Test environment | Training/test website |
| Target recorded in report | `ts.red-promo.ru` |
| Report updated | 2026-05-19 |
| Test approach | Manual black-box testing |
| Browser | Chrome |
| Operating system | Not recorded in the source artifact |

## Test scope

The documentation covers:

- Home page and header;
- navigation and catalog;
- product cards;
- Favorites;
- cart and quantity controls;
- checkout;
- Search;
- callback and authentication forms;
- Contacts and footer;
- responsive layout;
- design mockup comparison;
- negative and security-oriented inputs;
- Network, Console, Issues and accessibility observations.

## Test documentation

| Artifact | Quantity |
|---|---:|
| Smoke test cases | 22 |
| Functional test cases | 51 |
| Functional checklist items | 34 |
| UI and mockup checks | 10 |
| Negative test scenarios | 11 |
| Structured bug reports | 7 |

## Smoke execution summary

| Status | Quantity |
|---|---:|
| Passed | 4 |
| Failed | 5 |
| In Progress | 1 |
| Not Run | 12 |

The larger functional suite is primarily a test-design artifact. Scenarios that were not actually executed remain marked `Not Run` rather than being presented as successful checks.

## Main findings

### Functional and navigation defects

- `BUG-003` — Search displays an incorrect result count and contradictory empty-result message.
- `BUG-004` — Social media icons redirect to the Contacts page instead of the corresponding external services.

### Technical defects

- `BUG-002` — Required JavaScript resource `select22.min.js` returns `404 Not Found`.
- `BUG-005` — Content Security Policy blocks JavaScript string evaluation.
- `BUG-006` — Form controls are not correctly associated with their labels.

### UI and design defects

- `BUG-001` — Header menu items and telephone number do not match the supplied design mockup.
- `BUG-007` — Main page sections, banners, contact information and footer partially differ from the mockup.

## Traceability

The report links:

- product areas and requirements;
- functional test cases;
- smoke scenarios;
- Bug IDs;
- current execution status;
- review comments.

This makes it possible to distinguish:

- implemented and verified behaviour;
- failed behaviour;
- incomplete execution;
- UI mismatches;
- technical findings.

## Tools and techniques

- Chrome;
- Chrome DevTools Network;
- Chrome DevTools Console and Issues;
- responsive viewport testing;
- manual functional testing;
- positive and negative testing;
- exploratory testing;
- design comparison;
- test-case and checklist preparation;
- bug-report preparation;
- severity and priority assessment;
- traceability matrix.

## Test artifact

The complete report is available here:

- [Tor Store Web Testing Report](artifacts/torstore-web-testing-report.xlsx)

The workbook contains:

- project summary;
- smoke test cases;
- functional test cases;
- functional checklist;
- UI and mockup validation;
- negative testing;
- bug reports;
- traceability matrix;
- QA review notes;
- tools overview.

## Evidence

Evidence handling and publication rules are documented here:

- [Evidence overview](evidence/README.md)

## Limitations

- The complete functional suite was not executed.
- Cart and checkout flows require additional controlled execution.
- Responsive testing was started but not completed for all target widths.
- Browser and operating-system compatibility testing was not performed as a full matrix.
- The source code and server-side implementation were unavailable.
- Formal requirements were limited; part of the UI validation used a supplied design mockup.
- The tested website may change after the recorded test execution.
- The design PDF is not distributed in this repository.

## Disclaimer

This is an independent educational QA portfolio project.

The tested website, visual materials, product names and trademarks belong to their respective owners. The repository does not distribute proprietary source code or confidential project materials.
