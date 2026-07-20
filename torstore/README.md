# Tor Store Web Application Testing

Independent practical project covering manual black-box testing and test design for the **Tor Store** web application.

The project demonstrates functional testing, documented smoke execution, UI comparison with a supplied design mockup, negative test design, initial responsive checks and technical analysis with Chrome DevTools.

## Overview

| Parameter | Value |
|---|---|
| Application | Tor Store |
| Platform | Web |
| Environment | Public test environment |
| Tested target | `ts.red-promo.ru` |
| Report updated | 2026-05-19 |
| Approach | Manual black-box testing |
| Browser | Google Chrome |
| Operating system | Not recorded |
| Report language | English |

## Test scope

The documentation covers:

- home page and header;
- navigation and catalog;
- product cards;
- Favorites;
- cart and quantity controls;
- checkout test design;
- Search;
- callback and authentication forms;
- Contacts and footer;
- UI comparison with a design mockup;
- negative scenarios;
- initial responsive checks;
- Chrome DevTools Network, Console and Issues;
- accessibility observations.

Some negative, cart, checkout and responsive scenarios were designed but not fully executed. Their statuses remain `Not Run` or `In Progress`.

## Test documentation

| Artifact | Quantity |
|---|---:|
| Smoke test cases | 22 |
| Functional test cases | 51 |
| Functional checklist items | 34 |
| UI and mockup checks | 10 |
| Negative test scenarios | 11 |
| Structured bug reports | 7 |

## Smoke execution results

| Status | Quantity |
|---|---:|
| Passed | 4 |
| Failed | 5 |
| In Progress | 1 |
| Not Run | 12 |

The report uses `Passed` only when an actual result was observed. Unexecuted and incomplete checks remain explicitly marked.

## Key findings

### Functional and navigation

- `BUG-003` — Search displays an incorrect product count and a contradictory empty-result message.
- `BUG-004` — Social media icons redirect to the Contacts page instead of the corresponding external services.

### Technical

- `BUG-002` — Required JavaScript resource `select22.min.js` returns `404 Not Found`.
- `BUG-005` — Content Security Policy blocks JavaScript string evaluation.
- `BUG-006` — Form controls are not correctly associated with their labels.

### UI and design

- `BUG-001` — Header menu items and telephone number do not match the supplied design mockup.
- `BUG-007` — Main-page sections, banners, contact information and footer partially differ from the mockup.

## Traceability

The report links:

- product areas;
- functional test cases;
- smoke scenarios;
- Bug IDs;
- execution statuses;
- QA review comments.

This separates confirmed results, failed behavior, incomplete execution, UI mismatches and technical findings.

## Tools and techniques

- Google Chrome;
- Chrome DevTools Network;
- Chrome DevTools Console and Issues;
- manual functional testing;
- test-case and checklist design;
- positive and negative testing;
- initial responsive testing;
- design-mockup comparison;
- bug reporting;
- severity and priority assessment;
- traceability matrix.

## Artifacts

- [Tor Store Web Testing Report](artifacts/torstore-web-testing-report.xlsx)
- [Evidence publication rules](evidence/README.md)

## Limitations

- the complete functional suite was not executed;
- cart and checkout flows require additional controlled execution;
- responsive testing was not completed for all target widths;
- a full browser and operating-system compatibility matrix was not tested;
- the source code and server-side implementation were unavailable;
- formal requirements were limited;
- part of the UI validation used a supplied design mockup;
- the tested website may change after the recorded execution;
- the design PDF is not distributed in this repository.

## Disclaimer

This is an independent practical QA portfolio project.

The tested website, visual materials, product names and trademarks belong to their respective owners. The repository does not distribute proprietary source code or confidential materials.
