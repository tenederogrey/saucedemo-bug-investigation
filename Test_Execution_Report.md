# Test Execution Report

## Test Information

**Application**
SauceDemo

**Testing Type**
Manual Functional Testing

**Executed By**
Greyanne Tenedero

---

## Test Summary

The checkout workflow was executed using manually designed test cases to validate user input and expected application behavior.

One validation defect was identified during execution involving whitespace-only input within required fields.

---

## Execution Results

| Test Case | Description | Status |
|------------|-------------|--------|
| TC-001 | Login | Pass |
| TC-002 | Add Product to Cart | Pass |
| TC-003 | Proceed to Checkout | Pass |
| TC-004 | Checkout Information Validation | Fail |
| TC-005 | Complete Checkout | Pass |

---

## Defects Found

| Bug ID | Severity | Status |
|---------|----------|--------|
| BUG-001 | Medium | Open |

---

## Overall Result

- Total Test Cases: 5
- Passed: 4
- Failed: 1
- Blocked: 0

---

## Observations

The application behaved as expected throughout most of the checkout workflow. However, validation for required customer information fields did not correctly reject whitespace-only input.

The issue was successfully reproduced multiple times and documented with supporting evidence.

---

## Conclusion

The checkout process is generally functional but requires improved validation logic to prevent invalid customer information from being accepted.