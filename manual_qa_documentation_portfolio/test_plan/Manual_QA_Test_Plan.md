# Manual QA Test Plan — ShopEase Demo

**Document version:** 1.0  
**Status:** Sample plan for a fictional application  
**Prepared by:** [Your name]  
**Date:** [Enter date]

## 1. Purpose
Define the scope, strategy, resources, risks, and completion criteria for manual testing of a fictional e-commerce web application.

## 2. Application Overview
ShopEase Demo allows users to browse products, search/filter listings, add items to a cart, update quantities, and complete a checkout form.

## 3. Objectives
- Verify that critical shopping workflows behave according to requirements.
- Identify functional defects and confusing user experiences.
- Validate input handling and calculation accuracy.
- Provide a concise, evidence-based view of product quality and release risk.

## 4. Scope
### In scope
- Product listing and product details
- Search and category filtering
- Cart add/remove/update
- Quantity validation and subtotal/total calculation
- Checkout required fields and format validation
- Order confirmation
- Basic layout and usability checks on desktop and mobile viewport sizes
- Regression of critical purchase journey

### Out of scope
- Real payment processing
- Production data or personal information
- Security penetration testing
- Load/stress testing
- External provider integrations unless explicitly available in the chosen demo

## 5. Test Approach
Testing will be performed manually using requirement-based, positive, negative, boundary-value, exploratory, usability, and regression techniques.

### Test levels and types
- Functional testing
- UI/usability checks
- Input validation
- Integration-oriented checks across product, cart, and checkout
- Regression testing of critical flows

## 6. Test Environment
- Application URL: [Enter authorized demo URL]
- Browser(s): [e.g., Chrome, Firefox]
- OS: [Enter OS]
- Viewports: desktop and mobile-sized viewport
- Test account: [Use a demo account only, if required]
- Test data: fictional product names and non-sensitive sample checkout values

## 7. Entry Criteria
- Application is accessible.
- Test scope and expected behavior are understood.
- Required demo data and test account are available.
- Environment is stable enough to begin testing.

## 8. Exit Criteria
- All high-priority test cases have an execution status.
- Failures have reproducible steps and evidence where possible.
- Critical/high defects are documented and communicated.
- Test summary states coverage, outstanding risks, and recommendation.
- No result is reported as executed unless it was actually observed.

## 9. Deliverables
- Test plan
- Test case inventory and execution record
- Defect reports
- Screenshots or other evidence
- Test execution summary

## 10. Risks and Mitigations
| Risk | Impact | Mitigation |
|---|---|---|
| Demo site behavior differs from assumptions | Invalid expected results | Confirm behavior and adapt cases before execution |
| Public demo is unavailable | Testing blocked | Record blocked status and retry later |
| Test data persists between runs | Inconsistent results | Reset cart/session and document setup |
| Browser differences | UI/functionality inconsistency | Run critical flows in agreed browsers |
| Unclear requirements | Disputed defects | Record assumptions and request clarification |

## 11. Defect Management
Each defect should include a concise title, environment, preconditions, steps, expected result, actual result, severity, reproducibility, and evidence. Do not report a behavior as a defect unless it contradicts a stated requirement or agreed expectation.

## 12. Reporting
Report execution counts by Pass, Fail, Blocked, and Not Run. Summarize defects by severity, list unresolved risks, and provide a recommendation based on observed evidence.

## 13. Assumptions
This plan uses a fictional product specification for portfolio demonstration. Update the plan to match the actual application and requirements before execution.
