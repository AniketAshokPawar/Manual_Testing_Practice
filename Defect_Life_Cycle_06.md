Defect Life Cycle ⭐⭐⭐⭐⭐
=======================

The exact statuses can vary between companies/tools, but a common flow is:

**New → Assigned → Open → Fixed → Retest → Closed**

If the fix doesn't work:

**Retest → Reopen → Fixed → Retest → Closed**

Other possible statuses:

**Rejected / Duplicate / Deferred / Cannot Reproduce**

* * * * *

3\. Statuses Explained
----------------------

| Status | Meaning |
| --- | --- |
| **New** | QA has reported the defect. |
| **Assigned** | Defect is assigned to a developer/team for investigation. |
| **Open** | Developer has accepted/investigated the defect and work is in progress. |
| **Fixed** | Developer has fixed the defect and provided a new build for testing. |
| **Retest** | QA tests the specific defect again after the fix. |
| **Reopen** | QA finds that the defect is still occurring after the fix. |
| **Closed** | QA verifies the fix successfully and closes the defect. |
| **Rejected** | Developer/BA determines it is not a valid defect, e.g. working as designed. |
| **Duplicate** | Same issue has already been reported. |
| **Deferred** | Valid defect, but fixing it is postponed to a future release. |
| **Cannot Reproduce** | Developer/QA cannot reproduce the reported issue using the provided steps/data/environment. |

* * * * *

🔥 Example of Complete Defect Flow
==================================

Suppose QA finds:

> **Login fails with valid credentials.**

### Step 1 --- New

QA creates the defect.

⬇️

### Step 2 --- Assigned

Defect is assigned to Developer A.

⬇️

### Step 3 --- Open

Developer investigates the issue.

⬇️

### Step 4 --- Fixed

Developer fixes the login issue.

⬇️

### Step 5 --- Retest

QA tests login again.

### If it works:

**Retest → Closed ✅**

### If it still fails:

**Retest → Reopen → Developer fixes again → Retest**

* * * * *

4\. Rejected vs Duplicate vs Deferred vs Cannot Reproduce
=========================================================

These are commonly confusing.

| Status | When used |
| --- | --- |
| **Rejected** | It's not actually a defect / working as expected |
| **Duplicate** | Same defect already exists |
| **Deferred** | Valid defect, but fixing is postponed |
| **Cannot Reproduce** | Team cannot reproduce the reported issue |

### Example:

**QA:** "Button should be red."

**Developer:** "Requirement says blue."

👉 **Rejected**

* * * * *

**QA:** Reports "Login button doesn't work."

Another tester already reported the same issue.

👉 **Duplicate**

* * * * *

**QA:** Finds a minor UI issue before release.

Team decides to fix it in the next release.

👉 **Deferred**

* * * * *

**QA:** Reports that application crashes when clicking Save.

Developer follows the exact steps but cannot reproduce it.

👉 **Cannot Reproduce**

* * * * *

5\. Severity vs Priority ⭐⭐⭐⭐⭐ VVIP
===================================

This is **very commonly asked**.

### Severity

**How much impact does the defect have on the application?**

Usually decided by **QA**.

### Priority

**How urgently should the defect be fixed?**

Usually decided by **business/product/development team**, depending on the organization.

### Easy memory:

> **Severity = Impact**\
> **Priority = Urgency**

* * * * *

6\. Four Severity/Priority Combinations
=======================================

🔴 High Severity + High Priority
--------------------------------

Major functionality is broken and needs immediate fixing.

### Example:

> Application crashes when users try to make a payment.

**Impact:** Very high\
**Urgency:** Very high

* * * * *

🟠 High Severity + Low Priority
-------------------------------

Major technical/functional issue, but not urgent because the affected functionality is rarely used or release timing makes it less urgent.

### Example:

> An admin-only report crashes, but that report isn't needed for the current release.

**Impact:** High\
**Urgency:** Low

* * * * *

### 🟠 High Severity + Low Priority

**Example:**

> **The application crashes when generating the yearly financial report, but the report feature is used only once a year and is not needed currently.**

### Why?

-   **High Severity:** The application/functionality crashes completely.
-   **Low Priority:** The feature is not currently needed, so it can be fixed later.

This example clearly shows the difference between **impact** and **urgency**.

🟡 Low Severity + High Priority
-------------------------------

Small technical/UI issue but important from a business perspective.

### Example:

> Company logo is incorrect on the homepage just before a major marketing launch.

**Impact:** Low\
**Urgency:** High

* * * * *

🟢 Low Severity + Low Priority
------------------------------

Minor issue with little business impact.

### Example:

> Small alignment issue in a rarely used settings page.

**Impact:** Low\
**Urgency:** Low

* * * * *

🔥 Severity vs Priority Table
=============================

|  | **High Priority** | **Low Priority** |
| --- | --- | --- |
| **High Severity** | Payment crashes | Rarely used critical function has issue |
| **Low Severity** | Wrong company logo before launch | Minor UI alignment issue |

* * * * *

⭐ Interview Question: "Who decides Severity and Priority?"
==========================================================

A safe answer:

> **QA generally assesses severity based on the technical/functional impact, while priority is decided based on business urgency, usually in discussion with the Product Owner, Business Analyst, Development and QA teams.**

Don't say **"QA always decides severity and PO always decides priority"** as an absolute rule because organizations have different processes.

* * * * *

🧠 Quick Revision
=================

### Defect Life Cycle

**New → Assigned → Open → Fixed → Retest → Closed**

If failed:

**Retest → Reopen → Fixed → Retest**

Other statuses:

-   **Rejected** → Not a valid defect
-   **Duplicate** → Already reported
-   **Deferred** → Fix later
-   **Cannot Reproduce** → Unable to reproduce

### Severity vs Priority

**Severity = How badly it affects the system**

**Priority = How urgently it should be fixed**
