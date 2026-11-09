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
