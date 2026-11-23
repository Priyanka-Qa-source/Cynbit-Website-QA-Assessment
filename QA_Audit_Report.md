QA Audit Report – Cynbit Website
1. Project Information
Field	Details
Project name	Cynbit Website QA Audit
Website URL	https://www.cynbit.in/
Assessment	QA Testing Intern – Website Quality Audit
Tester	Priyanka
Test period	November 2026
Testing type	Manual functional and usability testing
Browser	Google Chrome
Device coverage	Android mobile device; tablet layout checked


2. Objective
The objective of this assessment was to review the website's main user journeys, check important functions, identify issues, and suggest practical improvements.
3. Scope of Testing
The following areas were checked:
1. Homepage access and navigation.
2. Logo, About Us, Services, Products, and Contact Us navigation.
3. Contact form validation and submission.
4. Valid email submission and email delivery.
5. Long-message and special-character handling.
6. Mobile and tablet responsiveness.
7. Basic keyboard navigation.
8. Footer links and call-to-action buttons.
9. Image loading and browser console.
10. General page-loading experience.
4. Test Environment
- Website: https://www.cynbit.in/
- Device: Android mobile device
- Browser: Google Chrome
- Device/layout coverage: Mobile and tablet layout
- Test period: November 2026
5. Test Cases and Results
  

## 5. Test Cases and Results

| Test ID | Test Scenario | Expected Result | Actual Result / Observation | Status |
|---|---|---|---|---|
| TC01 | Open the homepage | Homepage should load successfully | Homepage opened successfully | PASS |
| TC02 | Click the website logo | User should be taken to the homepage | Logo navigation worked | PASS |
| TC03 | Open About Us | About Us page or section should open | Opened successfully | PASS |
| TC04 | Open Services | Services page or section should open | Navigation was reported as successful | PASS |
| TC05 | Open Products | Products page or section should open | Opened successfully | PASS |
| TC06 | Open Contact Us | Contact Us page or section should open | Opened successfully | PASS |
| TC07 | Submit the form with required fields empty | Required-field validation should be displayed | Browser displayed a required-field validation message | PASS |
| TC08 | Enter invalid email `priya123` and submit | Form should reject the invalid email format | Form accepted the value and displayed a success message during a later test; behavior differed on an earlier attempt | FAIL – inconsistent validation |
| TC09 | Submit using valid email `alex@example.com` | Form should accept valid input and process the enquiry | Success feedback appeared and email delivery was verified | PASS |
| TC10 | Check the website on a mobile screen | Layout should fit the screen and remain usable | Mobile layout displayed properly | PASS |
| TC11 | Open mobile menu and navigate to About Us | Menu and navigation should work | Mobile menu navigation worked | PASS |
| TC12 | Check tablet layout | Content should display properly on a tablet-sized screen | Tablet layout displayed properly | PASS |
| TC13 | Navigate using the Tab key | Links and buttons should be reachable using the keyboard | Basic keyboard navigation worked | PASS |
| TC14 | Observe page-loading experience | Pages should load within a reasonable time | Website was reported to take a long time to load; no timing measurement was recorded | OBSERVATION |
| TC15 | Check browser console after refresh | No unexpected console errors should appear | No red console errors were reported | PASS |
| TC16 | Test footer links | Footer links should open their intended destinations | Tested footer links worked | PASS |
| TC17 | Check website images | Images should load correctly | Images were reported to load properly | PASS |
| TC18 | Test Join Us and Write Us buttons | Buttons should perform their intended action | Both buttons worked | PASS |
| TC19 | Submit a long message (approximately 500–1000 characters) | Form should handle long text without breaking | Long message was accepted successfully | PASS |
| TC20 | Submit a message containing special characters | Form should handle special characters without breaking | Special-character message was accepted successfully | PASS |


6. Test Execution Summary

| Result | Count |
|---|---:|
| PASS | 18 |
| FAIL | 1 |
| Observation requiring further investigation | 1 |
| **Total** | **20** |



7. Defect Identified
The contact form accepted an email value without an @ symbol (priya123) and displayed a success message. This does not meet the expected email-format validation behavior. See [Bug & Issue Report](Bug_Issue_Report.md) for reproduction details.
8. Additional Observation
The website was reported to load slowly. Since no objective load-time measurement or Lighthouse report was collected, this is recorded as an observation for further performance testing rather than a confirmed performance defect.
9. Conclusion
The manual assessment covered the main navigation, contact form, responsive layouts, and several user-facing elements. Most test cases passed. One issue was identified in invalid email validation, and page-loading performance should be measured further. The findings and recommendations are documented in the accompanying repository files.



