6\. Test Case & Test Scenario ⭐⭐⭐⭐⭐
===================================

1\. What is a Test Scenario?
----------------------------

A **high-level condition/functionality that needs to be tested**.

### Example:

For a Login page:

-   Verify login with valid credentials.
-   Verify login with invalid credentials.
-   Verify login with blank credentials.
-   Verify Forgot Password functionality.

👉 **Scenario = What to test?**

* * * * *

2\. What is a Test Case?
------------------------

A **detailed set of steps, test data, and expected results** used to verify a specific functionality.

👉 **Test Case = How to test it?**

### Easy difference:

| Test Scenario | Test Case |
| --- | --- |
| High-level | Detailed |
| What to test? | How to test? |
| Usually one-line | Contains steps, data, expected result, etc. |
| Example: Verify login functionality | Enter username → Enter password → Click Login → Verify dashboard |

* * * * *

3\. Test Scenario vs Test Case ⭐⭐⭐⭐⭐
====================================

Imagine a **Login** feature.

### Scenario:

> Verify login functionality.

From this one scenario, we can create multiple test cases:

1.  Login with valid credentials.
2.  Login with invalid username.
3.  Login with invalid password.
4.  Login with blank username.
5.  Login with blank password.
6.  Login with both fields blank.

So:

**1 Scenario → Multiple Test Cases**

* * * * *

4\. Test Case Document Format ⭐⭐⭐⭐⭐
===================================

Yes, this is the format you're talking about.

A typical test case can contain:

| Test Case ID | Test Case Description | Preconditions | Test Steps | Test Data | Expected Result | Actual Result | Status/Result | Priority | Severity | Environment | Comments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| TC_LOGIN_001 | Verify login with valid credentials | User is registered and on Login page | 1\. Enter username2. Enter password3. Click Login | Username: `user@test.com`Password: `Test@123` | User should login successfully and be redirected to Dashboard | User logged in and redirected to Dashboard | **Pass** | High | --- | QA / Chrome | --- |
| TC_LOGIN_002 | Verify login with invalid password | User is registered and on Login page | 1\. Enter valid username2. Enter invalid password3. Click Login | Username: `user@test.com`Password: `Wrong@123` | Appropriate error message should be displayed and user should not login | Error message displayed and user remained on Login page | **Pass** | High | --- | QA / Chrome | --- |

You don't necessarily need **every field in every company**. The format varies by organization/tool.

* * * * *

5\. Example Test Case ⭐⭐⭐⭐⭐
===========================

Let's take a simple **Login** page.

### Requirement:

> Registered user should be able to login using valid username and password.

| Field | Example |
| --- | --- |
| **Test Case ID** | TC_LOGIN_001 |
| **Test Case Description** | Verify user can login with valid credentials |
| **Preconditions** | User is registered and is on the Login page |
| **Test Steps** | 1\. Enter valid username 2. Enter valid password 3. Click Login |
| **Test Data** | Username: `user@test.com` Password: `Test@123` |
| **Expected Result** | User should be successfully logged in and redirected to Dashboard |
| **Actual Result** | User logged in and redirected to Dashboard |
| **Status** | Pass |
| **Priority** | High |
| **Comments** | --- |

### If login doesn't work:

**Expected:** User should be redirected to Dashboard.\
**Actual:** Error message "Invalid credentials" is displayed.\
**Status:** **Fail**

Then QA would generally create a **defect/bug**.

* * * * *

9\. Positive Test Case ⭐⭐⭐⭐
===========================

Tests the application with **valid/expected input**.

### Example:

**Valid username + valid password**

Expected:

> User should successfully login.

* * * * *

10\. Negative Test Case ⭐⭐⭐⭐
============================

Tests the application with **invalid/unexpected input**.

### Examples:

-   Invalid username
-   Invalid password
-   Blank username
-   Blank password
-   Invalid email format

Expected:

> Application should reject the input and display an appropriate error message.

* * * * *

🔥 Interview Scenario: "Write Test Cases for Login"
===================================================

Don't immediately start writing random cases.

Think in categories:

### Positive

1.  Valid username + valid password.

### Negative

1.  Invalid username + valid password.
2.  Valid username + invalid password.
3.  Invalid username + invalid password.
4.  Blank username.
5.  Blank password.
6.  Both fields blank.

### Validation

1.  Password masking.
2.  Username/email format validation.
3.  Login button behavior.
4.  Error message validation.

### Other

1.  Forgot Password.
2.  Remember Me, if available.
3.  Account lock after multiple failed attempts, if required.

That's how you show the interviewer that you can **derive test cases logically from a requirement**, rather than just memorizing them.

* * * * *

⭐ Quick Revision
================

**Scenario = What to test?**

**Test Case = How to test it?**

**Test Data = With what data?**

**Expected Result = What should happen?**

**Actual Result = What happened?**

**Status = Pass / Fail / Blocked**

And remember the basic flow:

> **Requirement → Scenario → Test Case → Test Data → Execute → Compare Expected vs Actual → Pass/Fail → Defect if required**
