# Bug Report

## Bug ID

BUG-001

---

## Title

Checkout Information accepts whitespace-only values.

---

## Module

Checkout

---

## Environment

- Application: SauceDemo
- Browser: Google Chrome
- OS: Windows 11

---

## Severity

Medium

---

## Priority

Medium

---

## Status

Open

---

## Description

The checkout information form allows users to continue when the First Name and Last Name fields contain only whitespace characters.

Required fields should reject whitespace-only values because they do not represent valid user input.

---

## Preconditions

- User is logged into SauceDemo.
- At least one product has been added to the cart.

---

## Steps to Reproduce

1. Log in.
2. Add a product to the cart.
3. Proceed to Checkout.
4. Enter spaces in the First Name field.
5. Enter spaces in the Last Name field.
6. Enter a valid Postal Code.
7. Click **Continue**.

---

## Expected Result

The application should prevent checkout and display a validation message indicating that the required fields cannot contain only spaces.

---

## Actual Result

The application accepts whitespace-only values and proceeds to the next checkout step.

---

## Business Impact

Allowing invalid customer information may result in poor data quality, incomplete order records, and unreliable customer information.

---

## Recommendation

Trim leading and trailing whitespace before validation and reject inputs that become empty after trimming.

---

## Evidence

See the screenshots inside the **Screenshots** folder.

- 01_Add_To_Cart.png
- 02_Checkout.png
- 03_Bug_Reproduced.png
- 04_Finish_Info.png
- 05_Complete_Checkout.png