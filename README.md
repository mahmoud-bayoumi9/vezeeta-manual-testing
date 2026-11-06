# Vezeeta – Manual Testing Project

Manual test cases and bug reports for three modules of the [Vezeeta](https://www.vezeeta.com/) website (Egypt, English and Arabic versions).

> **Disclaimer:** This is an educational / portfolio project. It is not affiliated with or endorsed by Vezeeta. All test data (phone numbers, emails, accounts) is fictional.

## Project at a glance

| Module | Test cases | Pass | Fail | Not executed | Bugs logged |
|---|---|---|---|---|---|
| Contact Us form | 67 | 52 | 15 | 0 | 15 |
| Sign Up & Sign In | 94 (55 + 39) | 85 | 8 | 1 | 8 |
| Book a Doctor (search) | 42 | 40 | 1 | 1 | 1 |
| **Total** | **203** | **177** | **24** | **2** | **24** |

## Repository structure

```
.
├── README.md
├── test-cases/
│   ├── Contact_us.xlsx
│   ├── sigup_and_sign_in.xlsx
│   └── booking_doctor.xlsx
└── screenshots/          # evidence for the logged bugs
```

Each workbook contains:

- **Test Cases** – ID, title, precondition, environment, steps, test data, expected result, actual result, status and bug ID.
- **Bug Reports** – steps to reproduce, expected vs. actual result, severity, priority and status.
- **Summary** – execution statistics calculated by formulas (pass rate, results by test type, and by priority in the Book a Doctor workbook).

## What is covered

- **Functional (positive and negative):** required fields, valid and invalid data, error messages, duplicate accounts, wrong credentials, filters and dependent dropdowns.
- **Boundary value:** minimum and maximum lengths, phone number formats and lengths.
- **Security inputs:** SQL injection strings, script tags and special characters in input fields.
- **Usability and UI:** Enter and Tab behavior, double-click on submit, Back and refresh behavior, labels and error message styling.
- **Compatibility:** Chrome, Firefox, Edge, Android Chrome and iOS Safari.
- **Localization:** Arabic language, RTL layout and Arabic validation messages.
- **Performance and accessibility:** page and response time (assumed 3-second threshold), keyboard-only use and screen reader error association.

## Test environment

- Windows 10 – Chrome (primary), Firefox, Edge
- Android – Chrome, iOS – Safari, Chrome DevTools device mode
- Chrome DevTools (Network and Elements) for load time and accessibility checks

## Test design techniques used

Equivalence partitioning, boundary value analysis, error guessing, and negative testing.

## How to read the files

1. Open a workbook and start with the **Summary** sheet.
2. Go to **Test Cases** and filter the *Test Status* column by `Fail`.
3. Use the *Bug ID* column to jump to the matching row in **Bug Reports**.

## Assumptions and limitations

- Expected results follow common QA practice, not confirmed business requirements. Cases marked "confirm with BA" need verification against real requirements.
- Performance thresholds (3 seconds) are assumed values.
- The test type and priority classifications are suggested values.
- Test execution was manual only.



**Mahmoud Bayuomi NourEldeen** – QA Engineer (Manual Testing)

Feel free to open an issue or reach out through GitHub.
