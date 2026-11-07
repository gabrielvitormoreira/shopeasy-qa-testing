# ShopEasy — Software Requirements

This document describes the functional requirements of the ShopEasy application.

## REQ-001 — User Registration

**Description:**

The system must allow new users to create an account.

**Input Fields:**

- Name
- Email
- Password

**Business Rules:**

- The name must contain between 2 and 50 characters.
- The email must have a valid format.
- The password must contain between 8 and 20 characters.

**Acceptance Criteria:**

- The user must be able to register with valid information.
- The system must reject invalid email formats.
- The system must reject passwords shorter than 8 characters.
- The system must reject passwords longer than 20 characters.
- The system must display an appropriate validation message when the information is invalid.
- The system must confirm successful registration.

## REQ-002 — User Login

**Description:**

The system must allow registered users to log in to their accounts.

**Input Fields:**

- Email
- Password

**Business Rules:**

- The email must have a valid format.
- The password must not be empty.
- Only registered users with valid credentials can log in.

**Acceptance Criteria:**

- The user must be able to log in with valid credentials.
- The system must reject unregistered email addresses.
- The system must reject incorrect passwords.
- The system must display an appropriate error message when the credentials are invalid.
- The system must grant access to the user's account after a successful login.

  ## REQ-003 — Shopping Cart

**Description:**

The system must allow users to add products to a shopping cart and manage the selected items.

**Functional Rules:**

- Users must be able to add products to the cart.
- Users must be able to remove products from the cart.
- Users must be able to change product quantities.
- The system must update the total price when the cart is modified.

**Acceptance Criteria:**

- The user must be able to add a product to the cart.
- The user must be able to remove a product from the cart.
- The user must be able to increase or decrease product quantities.
- The system must calculate the total price correctly.
- The system must display the updated cart information after each modification.
- The system must display an empty cart when no products have been added.
- The system must not allow product quantities lower than 1.
- When the user adds the same product again, the system must increase its quantity in the shopping cart.

  ## REQ-004 — Order Checkout

**Description:**

The system must allow users to complete a purchase by confirming the products in their shopping cart and providing the required delivery information.

**Input Fields:**

- Full Name
- Delivery Address
- Payment Method

**Business Rules:**

- The shopping cart must contain at least one product.
- All required delivery information must be provided.
- The user must select a payment method.
- The system must calculate the final order amount correctly.

**Acceptance Criteria:**

- The user must be able to proceed to checkout with a non-empty shopping cart.
- The system must reject checkout attempts when the cart is empty.
- The system must require all mandatory delivery information.
- The system must require a payment method.
- The system must display the correct final order amount.
- The system must display an order confirmation after a successful purchase.
- ## Open Questions
- **REQ-004:** Should the system reject a Delivery Address field containing only whitespace characters?

- ## Testing Techniques Applied

The following testing techniques were considered during the design of test cases for REQ-001 — User Registration:

- **Equivalence Partitioning (EP):** Used to divide input data into valid and invalid groups for Name and Password fields.
- **Boundary Value Analysis (BVA):** Used to verify values at and around the minimum and maximum limits of Name and Password fields.

These techniques help improve test coverage and identify potential validation defects.

- **Positive and Negative Testing:** Applied to REQ-004 — Order Checkout to verify successful order submission and validation of mandatory checkout fields.
