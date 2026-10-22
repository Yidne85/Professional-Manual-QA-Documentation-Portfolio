# Professional Manual QA Documentation Portfolio

## Project Overview
This independent portfolio project demonstrates a structured manual QA workflow for a fictional e-commerce web application called **ShopEase Demo**. It includes a test plan, test cases, sample defect reports, and a test execution summary template.

**Project type:** Independent QA portfolio project  
**Application:** Fictional e-commerce web application (ShopEase Demo)  
**Testing approach:** Manual functional, negative, boundary, usability, and regression-oriented testing  
**Status:** Documentation template; execute against a demo application or use it as a sample specification before claiming execution results.

> Transparency note: ShopEase Demo is fictional. The artifacts are sample QA documentation and do not represent work performed for a real client.

## Project Goals
- Translate requirements into testable scenarios.
- Create clear, traceable test cases with preconditions, steps, and expected results.
- Document defects with reproducible steps and impact.
- Summarize test execution and communicate release risks.
- Demonstrate professional QA communication and documentation.

## Scope
### In scope
- Product listing and product details
- Search and filtering
- Add-to-cart behavior
- Cart quantity and total calculations
- Required-field validation at checkout
- Order confirmation behavior
- Basic UI and usability checks
- Regression checks for key purchase flows

### Out of scope
- Real payments or real personal data
- Production security penetration testing
- Load and stress testing
- Third-party shipping/payment provider integrations
- Testing against a live production system

## Deliverables
| Artifact | Location | Purpose |
|---|---|---|
| Test Plan | `test_plan/Manual_QA_Test_Plan.md` | Scope, approach, risks, entry/exit criteria |
| Test Cases | `test_cases/Manual_QA_Test_Cases.csv` | Executable manual test cases |
| Test Case Guide | `test_cases/Test_Case_Execution_Guide.md` | How to record execution consistently |
| Bug Report Templates | `bug_reports/Bug_Report_Templates.md` | Reproducible defect reporting |
| Test Summary Template | `test_summary/Test_Execution_Summary_Template.md` | Results, coverage, risks, recommendation |
| Evidence folder | `evidence/` | Add screenshots after actual execution |

## How to Use
1. Review the test plan and the fictional requirements.
2. Choose a demo e-commerce site that you are authorized to test, or use these artifacts as a documentation sample.
3. Adapt the test cases to the site's actual behavior and terms.
4. Execute each applicable case manually.
5. Record actual results and mark Pass, Fail, Blocked, or Not Run.
6. For each confirmed defect, create a bug report and attach sanitized evidence.
7. Complete the test summary using real execution data.
8. Add screenshots to `evidence/` only after capturing them from actual test runs.

## Test Case Format
Each case includes an ID, feature, title, priority, preconditions, test data, steps, expected result, and type. Record the actual result and execution status during a real run.

## Defect Severity Guidance
- **Critical:** Core system unavailable, data loss, or severe business/security impact.
- **High:** Major core workflow blocked with no reasonable workaround.
- **Medium:** Important feature incorrect but workaround exists.
- **Low:** Minor visual, wording, or low-impact usability issue.

Severity should reflect impact, not personal preference. Priority should reflect urgency to fix.

## Portfolio Disclosure
This is an independent sample project built to demonstrate manual QA documentation skills. No actual execution results or real application defects are claimed by these templates. Replace sample details with verified findings before presenting execution results.
