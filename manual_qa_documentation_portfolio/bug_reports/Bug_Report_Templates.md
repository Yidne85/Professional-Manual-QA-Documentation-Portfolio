# Bug Report: BUG-001

**Bug Title:** Checkout Form Accepts an Invalid Email Address

**Project:** ShopEase Demo — E-commerce Web Application
**Module:** Checkout
**Bug Type:** Functional / Input Validation
**Severity:** Major
**Priority:** High
**Status:** New
**Environment:** Web application, Chrome browser on Windows 11
**Test Type:** Negative Testing

### Description

The checkout form may accept an incorrectly formatted email address without displaying a validation message. This could allow customers to proceed with invalid contact information.

This defect must be reproduced on the selected demo application before being reported as an actual finding.

### Preconditions

1. The ShopEase Demo website is accessible.
2. At least one product is available.
3. The product can be added to the shopping cart.
4. The customer can access the checkout page.

### Steps to Reproduce

1. Open the ShopEase Demo website.
2. Navigate to a product details page.
3. Add the product to the shopping cart.
4. Open the shopping cart.
5. Proceed to checkout.
6. Enter a valid name and other required information.
7. Enter `john.doe@` in the email address field.
8. Complete any other required checkout fields with valid data.
9. Click the checkout submission button.

### Test Data

| Field       | Input           |
| ----------- | --------------- |
| Full Name   | John Doe        |
| Email       | john.doe@       |
| Address     | 123 Main Street |
| City        | Addis Ababa     |
| Postal Code | 1000            |

*The values above are illustrative test data.*

### Expected Result

* The application rejects the incorrectly formatted email address.
* A clear validation message appears near the email field.
* The customer cannot proceed until the email address is corrected.
* The form preserves the other valid information already entered.

### Actual Result

**Not yet verified.** Record the application's actual behavior after executing the test. Do not report a failure unless the application accepts the invalid address or otherwise violates its expected behavior.

### Business Impact

If invalid email addresses are accepted, customers may not receive order confirmations, delivery notifications, or other important communications.

### Recommended Evidence

* Screenshot of the checkout form containing the invalid email.
* Screenshot of the validation message, if displayed.
* Screen recording showing the reproduction steps, if useful.

### Suggested Regression Tests

* Submit an empty email field.
* Submit `john.doe@`.
* Submit `john.doe.example.com`.
* Submit a valid address such as `john.doe@example.com`.
* Submit an email address containing leading or trailing spaces.

### Acceptance Criteria for the Fix

The application validates email input consistently and prevents checkout submission when the address format is invalid.
