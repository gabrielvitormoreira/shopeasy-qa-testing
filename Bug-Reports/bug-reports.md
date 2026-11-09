# ShopEasy — Bug Reports

This document contains bug reports created during the ShopEasy QA testing project.

## Project Information

- Project: ShopEasy
- Type: Fictional E-commerce Application
- Purpose: QA Portfolio Project

## BUG-001 — Invalid Email Format Accepted on Login

**Requirement:** REQ-002 — User Login

**Test Case:** TC-019 — Invalid Email Format

### Environment
Not specified — simulated scenario.

### Preconditions
The user is on the ShopEasy login page.

### Steps to Reproduce
1. Enter an invalid email address in the Email field.
2. Enter a password in the Password field.
3. Click the Login button.

### Test Data
- Email: `gabriel.qa.test.com`
- Password: `Teste1234`

### Expected Result
The system should prevent the login attempt and display an error message indicating that the email format is invalid.

### Actual Result
In this simulated scenario, the system allows the login form to be submitted with an invalid email format.

### Severity
Medium

### Priority
High

### Status
New

### Evidence
Not available — simulated scenario.

### Note
This is a hypothetical defect created for portfolio practice. It was not observed in a real application or verified through test execution.

## BUG-002 — Product Quantity Can Be Set to Zero

**Requirement:** REQ-003 — Shopping Cart

**Test Case:** TC-026 — Attempt to Set Product Quantity to Zero

### Environment
Not specified — simulated scenario.

### Preconditions
The user has at least one product in the shopping cart.

### Steps to Reproduce
1. Add a smartphone to the shopping cart.
2. Locate the product quantity field in the shopping cart.
3. Change the product quantity to 0.

### Test Data
- Product: Smartphone
- Quantity: 0

### Expected Result
The system should prevent the product quantity from being set to zero and maintain the minimum quantity of 1.

### Actual Result
In this simulated scenario, the system accepts the product quantity of zero.

### Severity
Medium

### Priority
Medium

### Status
New

### Evidence
Not available — simulated scenario.

### Note
This is a hypothetical defect created for portfolio practice. It was not observed in a real application or verified through test execution.

## BUG-003 — Checkout Allowed with Empty Cart

**Requirement:** REQ-004 — Order Checkout

**Test Case:** TC-031 — Attempt to Checkout with Empty Cart

### Environment
Not specified — simulated scenario.

### Preconditions
The shopping cart is empty.

### Steps to Reproduce
1. Access the shopping cart.
2. Click the Checkout button.

### Test Data
- Shopping Cart: Empty
- Products: 0

### Expected Result
The system should prevent the user from proceeding with checkout and display a message indicating that the shopping cart is empty.

### Actual Result
In this simulated scenario, the system allows the user to proceed with checkout even though the shopping cart is empty.

### Severity
High

### Priority
High

### Status
New

### Evidence
Not available — simulated scenario.

### Note
This is a hypothetical defect created for portfolio practice. It was not observed in a real application or verified through test execution.

## BUG-004 — Checkout Allowed with Empty Full Name

**Requirement:** REQ-004 — Order Checkout

**Test Case:** TC-033 — Checkout with Empty Full Name

### Environment
Not specified — simulated scenario.

### Preconditions
The user has products in the shopping cart and is on the checkout page.

### Steps to Reproduce
1. Access the checkout page with products in the shopping cart.
2. Leave the Full Name field empty.
3. Enter a valid delivery address and select a payment method.
4. Click the Place Order button.

### Test Data
- Full Name: Empty
- Delivery Address: 123 Test Street
- Payment Method: Credit Card

### Expected Result
The system should prevent order submission and display an error message indicating that the Full Name field is required.

### Actual Result
In this simulated scenario, the system allows the user to submit the order without providing a Full Name.

### Severity
High

### Priority
High

### Status
New

### Evidence
Not available — simulated scenario.

### Note
This is a hypothetical defect created for portfolio practice. It was not observed in a real application or verified through test execution.

## BUG-005 — Checkout Allowed with Empty Delivery Address

**Requirement:** REQ-004 — Order Checkout

**Test Case:** TC-034 — Checkout with Empty Delivery Address

### Environment
Not specified — simulated scenario.

### Preconditions
The user has products in the shopping cart and is on the checkout page.

### Steps to Reproduce
1. Access the checkout page with products in the shopping cart.
2. Leave the Delivery Address field empty.
3. Enter a valid Full Name and select a Payment Method.
4. Click the Place Order button.

### Test Data
- Full Name: Gabriel Moreira
- Delivery Address: Empty
- Payment Method: Credit Card

### Expected Result
The system should prevent order submission and display an error message indicating that the Delivery Address field is required.

### Actual Result
In this simulated scenario, the system allows the user to submit the order without providing a Delivery Address.

### Severity
High

### Priority
High

### Status
New

### Evidence
Not available — simulated scenario.

### Note
This is a hypothetical defect created for portfolio practice. It was not observed in a real application or verified through test execution.

## BUG-006 — Checkout Allowed Without Payment Method

### Bug ID
BUG-006

### Title
Checkout Allowed Without Payment Method

### Requirement
REQ-004 — Order Checkout

### Test Case
TC-035 — Checkout Without Selecting a Payment Method

### Environment
Not specified — simulated scenario.

### Preconditions
The user has products in the shopping cart and is on the checkout page.

### Steps to Reproduce
1. Access the checkout page with products in the shopping cart.
2. Leave the Payment Method field empty.
3. Click the Place Order button.

### Test Data
- Full Name: Gabriel Moreira
- Delivery Address: 123 Test Street
- Payment Method: Empty

### Expected Result
The system should prevent order submission and display an error message indicating that a payment method is required.

### Actual Result
In this simulated scenario, the system allows the user to submit the order without selecting a payment method.

### Severity
High

### Priority
High

### Status
New

### Evidence
Not available — simulated scenario.

**Note:** This is a hypothetical defect created for portfolio practice. It has not been observed or verified in a real application.

## BUG-007 — Checkout Allowed with Whitespace-Only Delivery Address

### Bug ID
BUG-007

### Title
Checkout Allowed with Whitespace-Only Delivery Address

### Requirement
REQ-004 — Order Checkout

### Test Case
TC-039 — Checkout with Whitespace-Only Delivery Address

### Environment
Not specified — simulated scenario.

### Preconditions
The user has products in the shopping cart and is on the checkout page.

### Steps to Reproduce
1. Access the checkout page with products in the shopping cart.
2. Enter only whitespace characters in the Delivery Address field.
3. Click the Place Order button.

### Test Data
- Full Name: Gabriel Moreira
- Delivery Address: `"     "` (whitespace characters only)
- Payment Method: Credit Card

### Expected Result
The system should prevent order submission and display an error message indicating that a valid delivery address is required.

### Actual Result
In this simulated scenario, the system allows the user to submit the order with a Delivery Address field containing only whitespace characters.

### Severity
High

### Priority
High

### Status
New

### Evidence
Not available — simulated scenario.

**Note:** This is a hypothetical defect created for portfolio practice. The validation rule is still pending confirmation and the defect has not been observed or verified in a real application.

## BUG-008 — Registration Allows Password Above Maximum Length

### Bug ID
BUG-008

### Title
Registration Allows Password Above Maximum Length

### Requirement
REQ-001 — User Registration

### Test Case
TC-004 — Password Above Maximum Length (>20)

### Environment
Not specified — simulated scenario.

### Preconditions
The user is on the ShopEasy registration page.

### Steps to Reproduce
1. Access the ShopEasy registration page.
2. Enter a password with 21 characters in the Password field.
3. Click the Register button.

### Test Data
- Password: `Password1234567890123`
- Length: 21 characters.

### Expected Result
The system should prevent user registration and display an error message indicating that the password must not exceed 20 characters.

### Actual Result
In this simulated scenario, the system accepts a password with 21 characters during registration.

### Severity
Medium

### Priority
Medium

### Status
New

### Evidence
Not available — simulated scenario.

**Note:** This is a hypothetical defect created for portfolio practice. It has not been observed or verified in a real application.

## BUG-009 — Registration Allows Password Below Minimum Length

### Bug ID
BUG-009

### Title
Registration Allows Password Below Minimum Length

### Requirement
REQ-001 — User Registration

### Test Case
TC-003 — Password Below Minimum Length (<8)

### Environment
Not specified — simulated scenario.

### Preconditions
The user is on the ShopEasy registration page.

### Steps to Reproduce
1. Access the ShopEasy registration page.
2. Enter a password with 6 characters in the Password field.
3. Click the Register button.

### Test Data
- Password: `Test12`
- Length: 6 characters.

### Expected Result
The system should prevent user registration and display an error message indicating that the password must contain at least 8 characters.

### Actual Result
In this simulated scenario, the system accepts a password with only 6 characters during registration.

### Severity
Medium

### Priority
Medium

### Status
New

### Evidence
Not available — simulated scenario.

**Note:** This is a hypothetical defect created for portfolio practice. It has not been observed or verified in a real application.

## BUG-010 — Login Accepts Email Containing Only Whitespace

### Bug ID
BUG-010

### Title
Login Accepts Email Containing Only Whitespace

### Requirement
REQ-002 — User Login

### Test Case
TC-020 — Email Field with Only Whitespace

### Environment
Not specified — simulated scenario.

### Preconditions
The user is on the ShopEasy login page.

### Steps to Reproduce
1. Access the ShopEasy login page.
2. Enter only whitespace characters in the Email field.
3. Click the Login button.

### Test Data
- Email: `"     "` (whitespace characters only)
- Password: `Teste1234`

### Expected Result
The system should prevent the login attempt and display an error message indicating that a valid email address is required.

### Actual Result
In this simulated scenario, the system accepts an email field containing only whitespace characters when the user submits the login form.

### Severity
Medium

### Priority
Medium

### Status
New

### Evidence
Not available — simulated scenario.

**Note:** This is a hypothetical defect created for portfolio practice. It has not been observed or verified in a real application.

## Bug Report Template

### Bug ID
BUG-XXX

### Title
[Short description of the defect]

### Environment
[Browser, operating system, device]

### Preconditions
[Conditions required to reproduce the issue]

### Steps to Reproduce
1. [Step 1]
2. [Step 2]
3. [Step 3]

### Expected Result
[What should happen]

### Actual Result
[What happened]

### Severity
[Critical / High / Medium / Low]

### Priority
[High / Medium / Low]

### Status
[New / In Progress / Fixed / Retest / Closed]

### Evidence
[Screenshots, videos, or other supporting evidence]
