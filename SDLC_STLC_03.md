2\. SDLC & STLC ⭐⭐⭐
===================

This topic is important, but we will keep it **practical and interview-focused**.

* * * * *

1\. SDLC Phases
===============

**SDLC = Software Development Life Cycle**

| Phase | What Happens |
| --- | --- |
| **Requirement Analysis** | Business requirements are gathered and understood. |
| **Planning** | Timeline, resources, cost, and approach are planned. |
| **Design** | Application architecture and design are prepared. |
| **Development** | Developers write the application code. |
| **Testing** | QA tests the application and reports defects. |
| **Deployment** | Application is released to users/production. |
| **Maintenance** | Bugs are fixed and enhancements are added. |

### Flow:

**Requirement → Planning → Design → Development → Testing → Deployment → Maintenance**

* * * * *

2\. STLC Phases
===============

**STLC = Software Testing Life Cycle**

| Phase | What Happens |
| --- | --- |
| **Requirement Analysis** | QA understands what needs to be tested. |
| **Test Planning** | Testing scope, effort, resources, and approach are planned. |
| **Test Case Development** | Test scenarios, test cases, and test data are prepared. |
| **Test Environment Setup** | Required environment is prepared for testing. |
| **Test Execution** | Test cases are executed and defects are reported. |
| **Test Closure** | Testing results and learnings are documented. |

### Flow:

**Requirement Analysis → Test Planning → Test Case Development → Environment Setup → Test Execution → Test Closure**

* * * * *

3\. Requirement Analysis ⭐⭐⭐⭐⭐
==============================

### What happens?

QA studies the requirements and understands:

-   What functionality needs to be tested?
-   What are the acceptance criteria?
-   Are there any unclear requirements?
-   What are the possible risks?

### QA Activities

-   Review requirements/user stories.
-   Attend requirement discussions.
-   Identify unclear or missing requirements.
-   Ask questions to BA/PO/Developer.
-   Identify testable requirements.
-   Start identifying test scenarios.

### Example:

**Requirement:** User should be able to login.

QA should clarify:

-   Which credentials are valid?
-   What happens with an invalid password?
-   Is there a password length requirement?
-   Is account locking required after multiple failed attempts?

### Deliverables:

-   Requirement understanding
-   Clarification questions
-   High-level test scenarios / requirement traceability information

* * * * *

4\. Test Planning ⭐⭐⭐⭐
======================

### What happens?

The testing approach is planned.

### QA Activities

-   Identify testing scope.
-   Estimate testing effort.
-   Identify resources.
-   Identify risks.
-   Decide testing types required.

### Example:

For an **e-commerce checkout feature**, testing may include:

-   Functional testing
-   Payment testing
-   Integration testing
-   Regression testing

### Deliverables:

-   Test Plan
-   Test Strategy (depending on project)

* * * * *

5\. Test Case Development ⭐⭐⭐⭐⭐
===============================

### What happens?

QA prepares test cases and test data.

### QA Activities

-   Create test scenarios.
-   Write test cases.
-   Prepare positive and negative test cases.
-   Prepare test data.
-   Review test cases.
-   Update RTM if used.

### Example:

**Feature:** Login

Test cases:

-   Login with valid credentials.
-   Login with invalid password.
-   Login with empty username.
-   Login with empty password.

### Deliverables:

-   Test Scenarios
-   Test Cases
-   Test Data
-   RTM (if applicable)

* * * * *

6\. Test Environment Setup ⭐⭐⭐
==============================

### What happens?

The environment required for testing is prepared.

### Example:

QA may need:

-   Application URL
-   QA/Staging environment
-   Database access
-   Test accounts
-   Required browser/device

### QA Activities

-   Verify environment availability.
-   Verify application deployment.
-   Prepare test accounts/data.
-   Perform basic smoke testing.

### Deliverables:

-   Ready test environment
-   Environment configuration details

* * * * *

7\. Test Execution ⭐⭐⭐⭐⭐
========================

### What happens?

QA executes test cases and verifies actual vs expected results.

### QA Activities

-   Execute test cases.
-   Mark test cases as Pass/Fail.
-   Report defects.
-   Retest fixed defects.
-   Perform regression testing.
-   Update test execution status.

### Example:

**Expected:** User should login successfully.

**Actual:** Error message appears with valid credentials.

👉 Test case = **Fail**\
👉 QA logs a **Defect**

### Deliverables:

-   Test Execution Report
-   Defect Reports
-   Updated Test Cases

* * * * *

8\. Test Closure ⭐⭐⭐
====================

### What happens?

Testing activities are officially completed.

### QA Activities

-   Check test execution completion.
-   Prepare test summary.
-   Review open defects.
-   Collect testing metrics.
-   Document lessons learned.

### Deliverables:

-   Test Summary Report
-   Test Metrics
-   Test Closure Report

* * * * *

9\. Entry Criteria & Exit Criteria ⭐⭐⭐⭐
=======================================

Entry Criteria
--------------

Conditions that must be completed **before starting testing**.

### Example:

Before testing starts:

-   Requirements are available.
-   Application is deployed.
-   Test environment is ready.
-   Test cases are prepared.

* * * * *

Exit Criteria
-------------

Conditions that must be completed **before completing testing**.

### Example:

Before testing is completed:

-   Planned test cases are executed.
-   Critical defects are fixed.
-   Regression testing is completed.
-   Test results are reviewed.

### Easy Difference:

| Entry Criteria | Exit Criteria |
| --- | --- |
| Conditions to **start testing** | Conditions to **finish testing** |
| Before testing | After testing |

* * * * *

🔥 QA Activities in Each STLC Phase ⭐⭐⭐⭐⭐
=========================================

This is the most important part for your interview.

| STLC Phase | What QA Does | Main Deliverables |
| --- | --- | --- |
| **Requirement Analysis** | Understand requirements, identify gaps, ask questions | Clarifications, Test Scenarios |
| **Test Planning** | Define scope, effort, risks, and testing approach | Test Plan |
| **Test Case Development** | Create test cases and prepare test data | Test Cases, Test Data, RTM |
| **Environment Setup** | Verify environment and application availability | Ready Test Environment |
| **Test Execution** | Execute tests, report defects, retest, regression | Defect Reports, Execution Report |
| **Test Closure** | Prepare summary, metrics, and lessons learned | Test Summary Report |

* * * * *

⭐ Best Interview Answer
=======================

### **"What exactly do you do as a QA during each phase?"**

> First, I understand the requirements and acceptance criteria and clarify any unclear requirements. Then, I identify test scenarios, prepare test cases and test data. Once the test environment is ready, I execute the test cases and compare actual results with expected results. If I find any issues, I log defects and track them until they are fixed. After the fix, I perform retesting and regression testing where required. Finally, I review the test results, open defects, and prepare the required test summary or reports.

### 🔥 Quick Memory Flow

**Understand → Plan → Write → Setup → Execute → Report → Retest → Regression → Close**
