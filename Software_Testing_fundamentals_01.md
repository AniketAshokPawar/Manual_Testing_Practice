Software Testing Fundamentals ⭐⭐⭐
===================================

1\. What is Software Testing?
-----------------------------

Software Testing is the process of checking whether an application works as expected and identifying defects before it reaches users.

### Example:

Login functionality:

-   Enter valid username + password → User should login ✅
-   Enter invalid password → Proper error message should appear ✅

We test both expected and unexpected scenarios.

* * * * *

2\. Why do we need Testing?
---------------------------

We need testing to:

-   Find defects before users find them.
-   Verify the application meets requirements.
-   Improve product quality.
-   Reduce business and financial risk.
-   Ensure important features work correctly.

### Simple interview answer:

> Testing helps us identify defects and verify that the application works according to requirements before it is released to users.

* * * * *

3\. Verification vs Validation ⭐⭐⭐⭐⭐
====================================

| Verification | Validation |
| --- | --- |
| Checks whether we are building the product correctly | Checks whether we are building the correct product |
| Mostly static activities | Dynamic activities |
| No code execution required | Application/code is executed |
| Requirement reviews, design reviews | Actual software testing |

### Easy example:

**Requirement:** Login button should be available.

👉 **Verification:** Check requirement/design documents and confirm the Login button is specified.

👉 **Validation:** Open the application and verify whether the Login button actually works.

### Easy trick:

**Verification = Are we building the product right?**\
**Validation = Are we building the right product?**

* * * * *


| Term | What It Is | Who Generates / Finds It | Example |
| --- | --- | --- | --- |
| **Error** | A **human mistake** or misunderstanding in logic, syntax, or requirements. | Developers, Analysts, Architects, etc. | A developer miscalculates a tax formula or writes incorrect logic. |
| **Bug** | An **informal technical flaw** in the software causing unexpected behavior. | Usually identified by QA during testing. | Clicking the Submit button crashes the page due to a missing function call. |
| **Defect** | A **variance between actual application behavior and expected/business requirements**. | QA, Business Analysts, or End Users can identify it. | The requirement says the background should be green, but the application displays blue. |
| **Failure** | When the application **fails to perform its expected function during execution**. | Observed by QA or End Users. | The payment process fails when a user tries to complete a transaction. |



7\. 7 Testing Principles ⭐⭐⭐⭐⭐
==============================

These are important. Don't just memorize them---understand the meaning.

1️⃣ Testing shows the presence of defects
-----------------------------------------

Testing can prove that defects exist, but cannot prove that the application has **zero defects**.

### Example:

You test 100 scenarios and all pass. There could still be an untested scenario containing a defect.

* * * * *

2️⃣ Exhaustive testing is impossible
------------------------------------

Testing every possible combination is practically impossible.

### Example:

A login page can have unlimited combinations of username, password, browsers, devices, etc.

So, we select important test cases based on risk and priority.

* * * * *

3️⃣ Early testing
-----------------

Testing should start as early as possible.

### Example:

Finding a requirement issue before development is much cheaper than finding it after production release.

* * * * *

4️⃣ Defect clustering
---------------------

A small number of modules usually contain most defects.

### Example:

If the Payment module has many bugs, we should focus more testing there.

* * * * *

5️⃣ Pesticide paradox
---------------------

Running the same test cases repeatedly may eventually stop finding new defects.

So, test cases should be reviewed and updated regularly.

### Example:

Always testing only valid login credentials may miss new login issues. Add new negative and edge-case scenarios.

* * * * *

6️⃣ Testing is context dependent
--------------------------------

Different applications require different testing approaches.

### Example:

A banking application requires more security testing than a simple informational website.

* * * * *

7️⃣ Absence-of-errors fallacy
-----------------------------

Even if the application has no known defects, it can still fail if it does not meet user requirements.

### Example:

An application works perfectly, but users cannot complete the main business process.

👉 **No bugs ≠ Successful product**

* * * * *

8\. What is SDLC? ⭐⭐⭐⭐⭐
=======================

**SDLC = Software Development Life Cycle**

It describes the phases involved in developing software.

### Common SDLC phases:

**1\. Requirement Gathering**\
Understand business requirements.

**2\. Planning**\
Plan timeline, resources, cost, and approach.

**3\. Design**\
Prepare application architecture and design.

**4\. Development**\
Developers write code.

**5\. Testing**\
QA tests the application.

**6\. Deployment**\
Application is released.

**7\. Maintenance**\
Fix issues and make improvements after release.

### Easy flow:

**Requirement → Planning → Design → Development → Testing → Deployment → Maintenance**

* * * * *

9\. What is STLC? ⭐⭐⭐⭐⭐
=======================

**STLC = Software Testing Life Cycle**

It describes the testing activities performed by the QA team.

### Common STLC phases:

**1\. Requirement Analysis**\
Understand requirements and identify what needs testing.

**2\. Test Planning**\
Define testing approach, scope, resources, and timeline.

**3\. Test Case Development**\
Create test scenarios, test cases, and test data.

**4\. Test Environment Setup**\
Prepare the environment required for testing.

**5\. Test Execution**\
Execute test cases and report defects.

**6\. Test Closure**\
Prepare reports, metrics, and lessons learned.

### Easy flow:

**Requirement Analysis → Test Planning → Test Case Development → Environment Setup → Execution → Closure**

* * * * *

10\. Role of QA in SDLC ⭐⭐⭐⭐⭐
=============================

This is an important interview question.

QA should be involved throughout the SDLC---not only after development is completed.

### Requirement Phase

-   Review requirements.
-   Identify missing or unclear requirements.
-   Raise questions.

### Planning Phase

-   Provide testing estimates.
-   Identify testing scope and risks.

### Design Phase

-   Review design from a testing perspective.
-   Identify possible test scenarios.

### Development Phase

-   Prepare test cases.
-   Prepare test data.
-   Review requirements and changes.

### Testing Phase

-   Execute test cases.
-   Report defects.
-   Perform retesting.
-   Perform regression testing.
-   Automate suitable test cases.

### Deployment Phase

-   Perform final validation/smoke testing.

### Maintenance Phase

-   Test bug fixes and new changes.
-   Perform regression testing.

### ⭐ Best interview answer

> QA should be involved from the beginning of SDLC. QA reviews requirements, identifies risks, prepares test cases and test data, executes testing, reports defects, performs retesting and regression testing, and supports release validation.
