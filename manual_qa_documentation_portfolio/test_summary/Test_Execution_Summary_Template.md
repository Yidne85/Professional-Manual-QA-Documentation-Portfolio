# TEST EXECUTION SUMMARY REPORT

## ShopEase Demo — E-commerce Web Application

### 1. Document Information

| Field            | Details                                                         |
| ---------------- | --------------------------------------------------------------- |
| Project Name     | ShopEase Demo                                                   |
| Document ID      | QA-TSR-001                                                      |
| Document Version | 1.0                                                             |
| Prepared By      | Yidnekachew Tafese                                              |
| Role             | QA Engineer                                                     |
| Testing Type     | Manual Functional, Negative, Regression, and End-to-End Testing |
| Test Cycle       | Cycle 1                                                         |
| Execution Status | In Progress — One Test Pending                                  |
| Test Environment | Record the actual demo URL, browser, and operating system       |
| Execution Date   | Record the actual execution date                                |
| Document Status  | Draft — Pending Completion of TC-015                            |

**Project note:** This document summarizes the test results supplied for an independent QA portfolio project. The results should be supported by the actual execution records and screenshots before the report is published as verified testing evidence.

---

### 2. Executive Summary

Manual testing was performed across the core functionality of the ShopEase Demo e-commerce application. The testing covered product browsing, product details, search, category filtering, shopping cart operations, checkout validation, order placement, navigation, responsive UI, and the core purchase journey.

A total of **18 test cases** were defined. Of these, **17 passed**, while **one remains pending** because the actual result for TC-015, which tests duplicate checkout submission, has not been recorded.

The completed tests indicate that the tested functionality behaved as expected according to the supplied results. However, the test cycle is not yet complete, and the duplicate submission scenario requires further verification.

#### Execution Metrics

| Metric                         | Result |
| ------------------------------ | -----: |
| Total Test Cases               |     18 |
| Passed                         |     17 |
| Failed                         |      0 |
| Blocked                        |      0 |
| Pending / Not Executed         |      1 |
| Executed                       |     17 |
| Execution Progress             | 94.44% |
| Pass Rate Among Executed Tests |   100% |
| Confirmed Defects Reported     |      0 |
| Open Test Cases                |      1 |

**Calculation:**

Execution Progress = 17 ÷ 18 × 100 = **94.44%**

Pass Rate = 17 ÷ 17 × 100 = **100%**

The 100% pass rate applies only to the 17 tests recorded as passed. It does not mean the entire application is defect-free.

---

### 3. Testing Objectives

The objectives of this test cycle were to:

1. Verify that product listings and product details display correctly.
2. Validate product search and category filtering.
3. Confirm that shopping cart operations work as expected.
4. Verify cart quantity updates and subtotal calculations.
5. Validate required checkout fields and email format.
6. Verify the order confirmation workflow using demo data.
7. Assess navigation and mobile viewport usability.
8. Validate the core purchase journey through regression and end-to-end testing.
9. Identify functional issues and document reproducible defects.

---

### 4. Scope of Testing

The following application modules were covered.

| Module                        | Coverage                                                                                | Overall Result |
| ----------------------------- | --------------------------------------------------------------------------------------- | -------------- |
| Product Listing               | Product listing loads correctly                                                         | Pass           |
| Product Details               | Product information displays correctly                                                  | Pass           |
| Search                        | Existing and nonexistent product searches                                               | Pass           |
| Filtering                     | Product category filtering                                                              | Pass           |
| Shopping Cart                 | Add, duplicate add, update quantity, remove, invalid quantity, and subtotal calculation | Pass           |
| Checkout                      | Required fields, email validation, and order confirmation                               | Pass           |
| Checkout Duplicate Submission | Repeated submission behavior                                                            | Pending        |
| Navigation                    | Return from product details to listing                                                  | Pass           |
| Responsive UI                 | Key content and controls at a mobile viewport                                           | Pass           |
| Regression / End-to-End       | Core purchase journey                                                                   | Pass           |

The duplicate checkout submission test remains outstanding. Therefore, that specific behavior has not yet been verified.

---

### 5. Test Execution Results by Module

The following summary groups the 18 test cases by their primary module.

| Module                  |  Total | Passed | Failed | Pending |
| ----------------------- | -----: | -----: | -----: | ------: |
| Product Listing         |      1 |      1 |      0 |       0 |
| Product Details         |      1 |      1 |      0 |       0 |
| Search                  |      2 |      2 |      0 |       0 |
| Filtering               |      1 |      1 |      0 |       0 |
| Shopping Cart           |      5 |      5 |      0 |       0 |
| Checkout                |      4 |      3 |      0 |       1 |
| Navigation              |      1 |      1 |      0 |       0 |
| UI / Responsive         |      1 |      1 |      0 |       0 |
| Regression / End-to-End |      1 |      1 |      0 |       0 |
| **Total**               | **18** | **17** |  **0** |   **1** |

*Note: TC-015 is assigned to the Checkout module and is the only pending test case.*

---

### 6. Detailed Test Results

#### 6.1 Product Listing and Product Details

**Test cases:** TC-001, TC-002

The supplied results indicate that the product listing loaded without blocking errors and that the selected product's name, price, image, and description were displayed correctly.

**Assessment:** Passed.

#### 6.2 Search and Filtering

**Test cases:** TC-003, TC-004, TC-005

The supplied results indicate that searching for an existing product returned matching results, searching for an unmatched string displayed a no-results message, and category filtering displayed products matching the selected category.

**Assessment:** Passed.

#### 6.3 Shopping Cart

**Test cases:** TC-006, TC-007, TC-008, TC-009, TC-010, TC-011

The supplied results indicate that:

* Products were added to the cart successfully.
* Adding the same product twice followed the expected cart behavior.
* Updating a product quantity recalculated the subtotal and total.
* Invalid quantities were rejected or corrected.
* Removing a product updated the cart totals.
* Subtotal calculations followed the application's pricing rules.

**Assessment:** Passed.

#### 6.4 Checkout

**Test cases:** TC-012, TC-013, TC-014, TC-015

The supplied results indicate that the checkout form blocked submission when required fields were empty, rejected an invalid email address, and displayed an order confirmation after a valid demo checkout.

However, TC-015 has no recorded actual result or final status.

**Assessment:** Three tests passed; one remains pending.

#### 6.5 Navigation and Responsive UI

**Test cases:** TC-016, TC-017

The supplied results indicate that navigation back to the product listing worked as expected and that key content and primary controls remained visible and usable at the specified mobile viewport.

**Assessment:** Passed.

#### 6.6 Regression and End-to-End Testing

**Test case:** TC-018

The supplied result indicates that the core purchase journey completed successfully and that product information, quantity, and totals remained consistent throughout the workflow.

**Assessment:** Passed.

---

### 7. Outstanding Test Case

#### TC-015 — Prevent Duplicate Checkout Submission on Repeated Click

| Field        | Details          |
| ------------ | ---------------- |
| Test Case ID | TC-015           |
| Module       | Checkout         |
| Priority     | Medium           |
| Test Type    | Negative Testing |
| Status       | Pending          |
| Defect ID    | Not assigned     |
| Evidence     | Not provided     |

**Objective:** Verify that repeated checkout submission does not unintentionally create duplicate orders.

**Required follow-up:**

1. Prepare valid demo checkout details.
2. Submit the checkout form once.
3. Attempt a second submission quickly, if the interface permits.
4. Inspect the resulting confirmation, order history, or available order records.
5. Verify whether one order or multiple orders were created.
6. Record the actual result and capture supporting evidence.
7. Update the test status to Pass or Fail based on the observed behavior and the application's requirements.

A second click alone does not establish a defect. The test must verify the actual outcome against the expected behavior.

---

### 8. Defect Summary

| Severity  | Defects Reported |
| --------- | ---------------: |
| Critical  |                0 |
| Major     |                0 |
| Moderate  |                0 |
| Minor     |                0 |
| **Total** |            **0** |

No failed test cases or confirmed defects were included in the supplied execution results.

**Important:** This means no defects were reported in the provided results. It does not prove that no defects exist in the application. TC-015 is pending and must be completed before its behavior can be assessed.

---

### 9. Evidence Summary

Evidence filenames supplied in the test records include:

| Test Case | Evidence File  | Status  |
| --------- | -------------- | ------- |
| TC-001    | `test_001.png` | Pass    |
| TC-002    | `test_002.png` | Pass    |
| TC-003    | `test_003.png` | Pass    |
| TC-004    | `test_004.png` | Pass    |
| TC-005    | `test_005.png` | Pass    |
| TC-006    | `test_006.png` | Pass    |
| TC-007    | `test_007.png` | Pass    |
| TC-008    | `test_008.png` | Pass    |
| TC-009    | `test_009.png` | Pass    |
| TC-010    | Not provided   | Pass    |
| TC-011    | `test_011.png` | Pass    |
| TC-012    | `test_012.png` | Pass    |
| TC-013    | `test_013.png` | Pass    |
| TC-014    | `test_014.png` | Pass    |
| TC-015    | Not provided   | Pending |
| TC-016    | `test_015.png` | Pass    |
| TC-017    | `test_016.png` | Pass    |
| TC-018    | Not provided   | Pass    |

The filenames above are based on the supplied test records. Their contents have not been independently reviewed as part of this summary.

Before publishing the portfolio, confirm that each referenced image exists, depicts the corresponding test execution, and does not contain sensitive information.

---

### 10. Risks and Limitations

The following limitations should be considered:

1. **Outstanding test:** Duplicate checkout submission has not been verified.
2. **Evidence review:** The screenshot files have not been independently inspected as part of this report.
3. **Testing scope:** The report covers only the 18 listed test cases.
4. **Security testing:** No security assessment or penetration testing was included.
5. **Performance testing:** No load or stress testing was performed.
6. **Payment processing:** The checkout scenario used demo data; real financial transactions were not tested.
7. **Environment coverage:** Browser and operating system coverage should be documented using the actual test environment.

These limitations should be considered when interpreting the results.

---

### 11. Entry and Exit Criteria

#### Entry Criteria

* The demo application is accessible.
* The relevant features are available.
* Test cases and expected results are defined.
* Required test data is available.

#### Exit Criteria

The test cycle can be considered complete when:

* All 18 test cases have recorded outcomes.
* Failed tests, if any, have corresponding defect reports where appropriate.
* Supporting evidence is available for the relevant results.
* Outstanding risks and limitations are documented.
* The final execution metrics are reviewed.

At present, the test cycle remains in progress because TC-015 is pending.

---

### 12. Overall Quality Assessment

**Current assessment: Incomplete test cycle; no failed tests reported among the executed cases.**

The supplied results show that the main product browsing, search, filtering, shopping cart, checkout validation, navigation, responsive UI, and end-to-end purchase scenarios passed.

The outstanding duplicate checkout submission scenario remains unverified. The assessment should be updated after that test is completed.

The results provide encouraging evidence for the tested workflows, but the limited scope and pending scenario prevent a definitive conclusion about the overall quality of the application.

---

### 13. Final Recommendation

**Recommendation: Complete the remaining test before final sign-off.**

The 17 passed test cases provide positive results for the tested functionality. However, TC-015 should be executed and documented before the test cycle is marked complete.

After the outstanding test is resolved:

* Update the final test execution metrics.
* Review all evidence.
* Record any confirmed defects.
* Reassess outstanding risks.
* Update the final quality assessment and recommendation.

This recommendation applies only to the scope covered by this independent manual QA test cycle.

---

### 14. Sign-Off

| Role          | Name               | Status             |
| ------------- | ------------------ | ------------------ |
| QA Engineer   | Yidnekachew Tafese | Pending final test |
| QA Reviewer   | Not assigned       | Not applicable     |
| Product Owner | Not assigned       | Not applicable     |

**Project Type:** Independent QA Portfolio Demonstration

**Document End**
