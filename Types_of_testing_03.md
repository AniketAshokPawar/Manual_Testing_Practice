4\. Testing Types ⭐⭐⭐⭐⭐ VVIP
============================

Keep one simple concept in mind:

-   **Functional Testing** → Checks **what the application does**.
-   **Non-Functional Testing** → Checks **how well the application performs**.

* * * * *

Functional Testing
==================

1\. Smoke Testing ⭐⭐⭐⭐⭐
-----------------------

Checks whether the **major/critical functionalities are working** after a new build is deployed.

### Example:

After deployment, check:

-   Application opens
-   Login works
-   Main page loads
-   Important functionality is accessible

👉 If Smoke Testing fails, detailed testing usually does not start.

**Keyword:** **Build verification**

* * * * *

2\. Sanity Testing ⭐⭐⭐⭐⭐
------------------------

Checks whether a **specific functionality or recent change works properly**.

### Example:

A bug is fixed in the **Forgot Password** feature.

QA mainly tests:

-   Forgot Password flow
-   Related functionality

👉 Sanity Testing is **narrow and focused**.

**Keyword:** **Specific change verification**

* * * * *

3\. Regression Testing ⭐⭐⭐⭐⭐
----------------------------

Checks whether **existing functionality is affected by new changes or bug fixes**.

### Example:

Developer changes the Login functionality.

QA tests:

-   Login
-   Logout
-   Forgot Password
-   Related user functionality

👉 We check whether the new change has broken existing features.

**Keyword:** **Existing functionality**

* * * * *

4\. Retesting ⭐⭐⭐⭐⭐
-------------------

Testing a **specific defect again after it is fixed**.

### Example:

Bug:

> Login button is not working.

Developer fixes it.

QA tests the **same Login button again**.

👉 **Retesting = Verify the bug fix.**

**Keyword:** **Same defect**

* * * * *

🔥 Regression vs Retesting
--------------------------

| Retesting | Regression Testing |
| --- | --- |
| Tests the specific fixed defect | Tests existing/related functionality |
| Verifies whether the bug is fixed | Checks whether changes caused new issues |
| Focused | Broader |
| Example: Test Login button after fix | Test Login, Logout, Forgot Password after login changes |

* * * * *

5\. Integration Testing ⭐⭐⭐⭐
----------------------------

Checks whether **different modules/components work correctly together**.

### Example:

**Login Module → Authentication API → Database**

Verify that all these components work together correctly.

Another example:

**Shopping Cart → Payment Gateway**

👉 We test the interaction between modules.

* * * * *

6\. System Testing ⭐⭐⭐⭐
-----------------------

Testing the **complete integrated application as a whole**.

### Example:

For an e-commerce application, test:

**Login → Search Product → Add to Cart → Payment → Order Confirmation**

👉 The complete system is tested against requirements.

* * * * *

7\. End-to-End (E2E) Testing ⭐⭐⭐⭐⭐
----------------------------------

Tests a **complete real user workflow from start to finish**, including integrated systems.

### Example:

> User registers → Logs in → Adds product to cart → Makes payment → Receives order confirmation email.

👉 E2E testing focuses on the **complete business/user flow**.

### System Testing vs E2E

| System Testing | E2E Testing |
| --- | --- |
| Tests the complete application | Tests complete user/business workflow |
| Focuses on system functionality | Focuses on user journey |
| May test internal modules | Usually includes external/integrated systems |

* * * * *

8\. Acceptance Testing / UAT ⭐⭐⭐⭐
---------------------------------

Checks whether the application meets **business requirements and user needs**.

### UAT = User Acceptance Testing

Usually performed by:

-   Client
-   Customer
-   Business users
-   End users

### Example:

Business user verifies:

> "Can I successfully complete the order process as expected?"

If satisfied → Application can be accepted for release.

* * * * *

Non-Functional Testing
======================

1\. Performance Testing ⭐⭐⭐
---------------------------

Checks the application's **speed, responsiveness, stability, and performance**.

### Example:

Check how quickly a page loads or an API responds.

Performance Testing includes:

-   Load Testing
-   Stress Testing
-   Spike Testing
-   Endurance Testing

* * * * *

2\. Load Testing ⭐⭐⭐
--------------------

Checks application performance under **expected or normal/high user load**.

### Example:

Test an application with **1,000 concurrent users**.

Check:

-   Response time
-   Stability
-   Errors

👉 **Expected load**

* * * * *

3\. Stress Testing ⭐⭐⭐
----------------------

Checks how the application behaves **beyond its expected capacity**.

### Example:

Application supports 1,000 users.

Test with **5,000 users**.

Check:

-   When does it fail?
-   Does it crash?
-   Does it recover?

👉 **Beyond capacity**

* * * * *

🔥 Load vs Stress Testing
-------------------------

| Load Testing | Stress Testing |
| --- | --- |
| Expected/normal high load | Beyond expected capacity |
| Checks performance | Finds breaking point |
| Example: 1,000 users | Example: 5,000 users |

* * * * *

4\. Security Testing ⭐⭐⭐
------------------------

Checks whether the application and its data are protected from unauthorized access and security vulnerabilities.

### Example:

-   Unauthorized user cannot access admin pages.
-   Passwords are protected.
-   User cannot access another user's data.

👉 Focus: **Security + Data Protection**

* * * * *

5\. Usability Testing ⭐⭐⭐
-------------------------

Checks whether the application is **easy and convenient to use**.

### Example:

-   Is navigation easy?
-   Are buttons clearly visible?
-   Are error messages understandable?
-   Can users easily complete their tasks?

👉 Focus: **User experience**

* * * * *

6\. Compatibility Testing ⭐⭐⭐
-----------------------------

Checks whether the application works correctly across different:

-   Browsers
-   Operating systems
-   Devices
-   Screen sizes

### Example:

Test application on:

-   Chrome
-   Firefox
-   Edge
-   Windows
-   Mobile devices

👉 Focus: **Works everywhere**

* * * * *

7\. Accessibility Testing ⭐⭐⭐
-----------------------------

Checks whether the application can be used by people with disabilities.

### Example:

Check whether:

-   Screen readers can read content.
-   Keyboard navigation works.
-   Images have proper alt text.
-   Text has sufficient contrast.

👉 Focus: **Accessible to everyone**

* * * * *

🔥 Quick Revision Table
=======================

| Testing Type | Main Purpose |
| --- | --- |
| **Smoke** | Check major functionality/build stability |
| **Sanity** | Check specific change or functionality |
| **Regression** | Check existing functionality after changes |
| **Retesting** | Verify a specific bug fix |
| **Integration** | Check interaction between modules |
| **System** | Test complete application |
| **E2E** | Test complete user workflow |
| **UAT** | Verify business/user requirements |
| **Performance** | Check speed and stability |
| **Load** | Check performance under expected load |
| **Stress** | Check beyond expected capacity |
| **Security** | Check protection from vulnerabilities |
| **Usability** | Check ease of use |
| **Compatibility** | Check across browsers/devices/OS |
| **Accessibility** | Check usability for people with disabilities |

* * * * *

⭐ Interview Focus --- Must Remember
=================================

### Functional Testing:

> **Smoke → Is the build stable?**\
> **Sanity → Does the specific change work?**\
> **Retesting → Is the specific bug fixed?**\
> **Regression → Did the change break anything else?**

### Non-Functional Testing:

> **Performance → How fast/stable?**\
> **Load → Expected users**\
> **Stress → Beyond capacity**\
> **Security → Is it protected?**\
> **Usability → Is it easy to use?**\
> **Compatibility → Does it work everywhere?**\
> **Accessibility → Can everyone use it?**

🔥 **Most important for interviews:** Smoke, Sanity, Regression, Retesting, Integration, E2E, Load vs Stress.
