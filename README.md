# Cynbit Website QA Assessment

## Project Overview
This repository contains the documentation for a manual quality audit of the Cynbit website, completed as part of the QA Testing Intern assessment.

| Project detail | Information |
|---|---|
| Website | https://www.cynbit.in/ |
| Assessment | Cynbit Website Quality Audit |
| Tester | Priyanka |
| Testing approach | Manual website testing |
| Test period | November 2026 |
| Browser | Google Chrome |
| Device coverage | Android mobile device and tablet layout |

## Repository Contents
- **[QA Audit Report](QA_Audit_Report.md):** Testing scope, environment, test cases, results, and conclusion.
- **[Bug & Issue Report](Bug_Issue_Report.md):** Reproduction details, expected and actual results, severity, and priority.
- **[Improvement Recommendations](Improvement_Recommendations.md):** Suggested improvements based on the testing observations.

## Testing Scope
The assessment covered:
- Homepage loading and website navigation
- Logo, header, footer, and call-to-action links
- Contact form required-field validation
- Invalid and valid email input
- Contact form submission and email delivery
- Long-message and special-character input
- Mobile and tablet responsiveness
- Basic keyboard navigation
- Image loading
- Browser console observation
- General page-loading experience

## Test Results

| Test ID | Test scenario | Result |
|---|---|---|
| TC01 | Homepage loading | PASS |
| TC02 | Website logo navigation | PASS |
| TC03 | About Us navigation | PASS |
| TC04 | Services navigation | PASS |
| TC05 | Products navigation | PASS |
| TC06 | Contact Us navigation | PASS |
| TC07 | Empty form validation | PASS |
| TC08 | Invalid email validation | FAIL |
| TC09 | Valid email submission and delivery | PASS |
| TC10 | Mobile responsiveness | PASS |
| TC11 | Mobile menu navigation | PASS |
| TC12 | Tablet responsiveness | PASS |
| TC13 | Basic keyboard navigation | PASS |
| TC14 | Page-loading performance | OBSERVATION |
| TC15 | Browser console check | PASS |
| TC16 | Footer links | PASS |
| TC17 | Image loading | PASS |
| TC18 | Join Us and Write Us buttons | PASS |
| TC19 | Long-message submission | PASS |
| TC20 | Special characters in message | PASS |

### Overall Result
- **Total test cases:** 20
- **Passed:** 18
- **Failed:** 1
- **Additional observation:** 1 (page loading felt slow)

The contact form accepted an invalid email value (`priya123`) and displayed a success message. This is documented as a defect because the expected behavior is to reject an invalid email format. Valid form submission and email delivery were verified separately. Long-message and special-character input checks were also completed successfully.

## Important Testing Notes
- A successful form-submission message and verified email delivery are recorded as separate checks.
- The invalid-email issue concerns acceptance of an incorrectly formatted email address; it does not mean the valid-email delivery test failed.
- The page-loading concern is recorded as an observation, not a confirmed performance defect, because no measured load time or performance audit result was captured.

