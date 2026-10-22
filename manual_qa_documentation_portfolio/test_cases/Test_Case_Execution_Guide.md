# Manual Test Case Execution Guide

## Status values
- **Pass:** Actual result matches the expected result.
- **Fail:** Actual result differs from the expected result and the mismatch is reproducible or sufficiently evidenced.
- **Blocked:** Execution cannot proceed because of an environment, access, dependency, or setup issue.
- **Not Run:** Test has not been executed.

## Execution rules
1. Read the preconditions and test data before starting.
2. Follow steps in order unless the test explicitly allows variation.
3. Record the actual result using observable behavior, not assumptions.
4. Attach screenshots or other evidence for failures where practical.
5. Create a separate defect report for each distinct issue.
6. Do not mark unexecuted tests as passed.
7. If the actual application differs from the fictional specification, document the discrepancy and revise the expected result only after the requirement is clarified.

## Recommended naming for evidence
`TC-XXX_short-description_browser_date.png`

Example: `TC-006_add-product-to-cart_chrome_2026-10-22.png`
