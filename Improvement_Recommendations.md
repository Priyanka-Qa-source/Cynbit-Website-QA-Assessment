Improvement Recommendations – Cynbit Website
1. Introduction
This document lists practical recommendations based on the manual testing observations recorded during the Cynbit website QA assessment. These are recommendations for review and do not imply that every listed area has a confirmed defect.
2. Recommendations
2.1 Improve Contact Form Email Validation
Observation: The contact form accepted an invalid email value (priya123) and displayed a success message during a later test.

Recommendations:
- Apply consistent email-format validation before accepting a form submission.
- Validate the email on both the client side and server side.
- Display a clear message when the email format is invalid.
- Prevent submission until the email format is corrected.
- Retest common invalid formats, including values without @ and values with missing domain information.
2.2 Provide Clear Form Submission Feedback
- Show a clear confirmation when an enquiry has been successfully processed.
- Keep form validation messages specific and easy to understand.
- Ensure the success message reflects the actual result of the submission process.
- Continue verifying the email-delivery workflow using an authorized test mailbox.
2.3 Review Page-Loading Performance
Observation: The website was reported to feel slow while loading.

Recommendations:
- Measure page-load time under consistent network conditions.
- Review image sizes and optimize large assets where appropriate.
- Review scripts and other resources that may delay page rendering.
- Compare mobile and desktop performance results before prioritizing changes.
2.4 Continue Responsive Layout Testing
- Check additional mobile, tablet, and desktop screen sizes.
- Verify that menus, forms, buttons, and text remain usable at different viewport widths.
- Check portrait and landscape orientations.
- Ensure that users do not need unnecessary horizontal scrolling.
2.5 Extend Accessibility Testing
Basic keyboard navigation was checked during this assessment. Further checks are recommended:
- Verify visible focus indicators.
- Check logical keyboard focus order.
- Confirm form fields have clear labels.
- Ensure validation errors are understandable.
- Review text contrast and alternative text for meaningful images.
2.6 Maintain Navigation and Website Content
- Recheck header and footer links periodically.
- Verify that call-to-action buttons continue to open the correct destinations.
- Check for broken links and missing content.
- Keep navigation labels consistent and understandable.
3. Suggested Future Test Activities
1. Retest invalid email validation after any fix.
2. Test boundary values for form fields, including minimum and maximum input lengths.
3. Verify form behavior across supported browsers.
4. Measure page-loading performance and record results.
5. Extend accessibility checks beyond basic keyboard navigation.
6. Retain screenshots and test evidence for reported defects.
4. Conclusion
The assessment found that most tested website functions worked as expected. The main functional improvement area is consistent email-format validation in the contact form. Page-loading performance should also be measured objectively to determine whether optimization is needed., usability, accessibility and overall user experience.
