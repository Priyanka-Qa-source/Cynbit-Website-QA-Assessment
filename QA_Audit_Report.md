Bug & Issue Report – Cynbit Website
1. Report Overview
Field	Details
Project	Cynbit Website QA Audit
Website	https://www.cynbit.in/
Tester	Priyanka
Test period	November 2026
Report type	Manual testing defect and observation report


2. Bug Summary
Bug ID	Title	Area	Severity	Priority	Status
BUG-01	Contact form accepts an invalid email address	Contact Us form	Medium	P2	Identified; requires developer review


3. BUG-01: Contact Form Accepts an Invalid Email Address
Description: The contact form accepted the value priya123, which is not a valid email address format, and displayed a success message.
Preconditions
- Cynbit website is accessible.
- Contact Us page is available.
Steps to Reproduce
1. Open https://www.cynbit.in/.
2. Navigate to the Contact Us page.
3. Enter a valid name.
4. Enter priya123@example.com in the email field.
5. Enter a message.
6. Click the Submit button.
7. Observe the form response.
Expected Result
The form should reject the invalid email format and display a clear validation message. It should not submit the enquiry until a valid email address is entered.
Actual Result
The form accepted priya123@example.com and displayed a success message during a later test. An earlier attempt showed browser validation requiring an @ symbol, so the behavior appeared inconsistent across attempts.
Severity and Priority
- Severity: Medium (provisional). Incorrect email validation may prevent users from receiving a response to their enquiry.
- Priority: P2 (provisional). The issue should be reviewed and corrected, although it does not prevent all users from using the contact form.
Suggested Fix
- Validate email format consistently on both the client side and server side.
- Prevent submission when the email format is invalid.
- Display a clear validation message beside the email field.
- Re-test invalid and valid email formats across supported browsers.

4. Additional Observation – Page Loading
Observation ID: OBS-01
Area: Website performance
Observation: The website was reported to take a long time to load.
Expected: Pages should load within a reasonable time under normal network conditions.
Actual: Loading felt slow during manual testing.
Status: Requires further investigation; not classified as a confirmed defect.
Evidence: No measured load time or performance audit report was recorded.

5. Verification Notes
- Valid form submission and email delivery were checked separately and reported successful.
- The invalid-email finding relates specifically to the form accepting an incorrectly formatted email value.
- A form success message alone should not be treated as proof of email delivery.
