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
