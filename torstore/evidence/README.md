# Tor Store Test Evidence

This directory is intended for sanitized evidence supporting the Tor Store web testing report.

## Evidence types

The project may include:

- screenshots of reproduced defects;
- Chrome DevTools Network screenshots;
- Console and Issues screenshots;
- responsive-layout screenshots;
- cropped comparisons between the website and design requirements;
- sanitized response fragments;
- short screen recordings.

## Recommended naming convention

- `TS-BUG-001-header-mockup-mismatch.png`
- `TS-BUG-002-javascript-resource-404.png`
- `TS-BUG-003-search-result-counter.png`
- `TS-BUG-004-social-links-navigation.png`
- `TS-BUG-005-csp-issue.png`
- `TS-BUG-006-form-label-accessibility.png`
- `TS-BUG-007-main-page-mockup-mismatch.png`

## Security and privacy checks

Before evidence is committed, it must be checked for:

- email addresses and passwords;
- session cookies;
- authentication tokens;
- API keys;
- personal information;
- browser history and unrelated tabs;
- private URLs;
- request headers containing authorization data;
- confidential company or course materials.

## Repository rules

- Raw HAR files are not committed because they may contain cookies and authorization data.
- Large videos are stored externally.
- Screenshots should be cropped to the relevant product area.
- Sensitive values must be hidden or replaced with placeholders.
- Each evidence item should reference the related Bug ID.
- Design materials should not be published without permission.

## Current status

Evidence references are recorded in the Excel report.

Additional screenshots should be added only after their contents, relevance and publication safety are verified.
