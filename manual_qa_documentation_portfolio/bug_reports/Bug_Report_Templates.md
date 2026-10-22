# Manual QA Defect Report Templates

These are templates only. They are not confirmed defects. Complete one only after observing a reproducible mismatch against a requirement or agreed expectation.

## Bug Report Template

- **Defect ID:** BUG-XXX
- **Title:** [Feature] Short, specific description of the problem
- **Application / build:** [Name and version/build]
- **Environment:** [OS, browser/version, viewport]
- **Test Case ID:** [Related test case]
- **Severity:** [Critical / High / Medium / Low]
- **Priority:** [P1 / P2 / P3 / P4]
- **Status:** New
- **Preconditions:** [Required setup]
- **Steps to reproduce:**
  1. [Step 1]
  2. [Step 2]
  3. [Step 3]
- **Expected result:** [Requirement-based expected behavior]
- **Actual result:** [Exact observed behavior]
- **Reproducibility:** [e.g., 3/3 attempts]
- **Impact:** [User/business impact]
- **Evidence:** [Screenshot/video/log; remove personal or sensitive data]
- **Additional notes:** [Relevant context]

## Sample Example — Illustrative Only

**Title:** [Cart] Cart total does not update after quantity change  
**Status:** Illustrative example — not an observed defect  
**Severity:** Medium (provisional)  
**Preconditions:** Cart contains one product with a known unit price.  
**Steps to reproduce:**
1. Add the product to the cart.
2. Change quantity from 1 to 2.
3. Review the displayed subtotal.

**Expected result:** Subtotal recalculates to unit price × quantity according to the application's rounding rules.  
**Actual result:** [Replace with what you actually observe; do not claim this issue exists without testing.]  
**Evidence:** [Attach screenshot from actual execution.]

## Severity guidance
- **Critical:** Application unavailable, severe data loss, or major business/security impact.
- **High:** Core workflow blocked with no reasonable workaround.
- **Medium:** Important functionality incorrect but a workaround exists.
- **Low:** Minor visual, content, or low-impact usability issue.

Severity describes impact; priority describes how urgently the team should address the issue.
