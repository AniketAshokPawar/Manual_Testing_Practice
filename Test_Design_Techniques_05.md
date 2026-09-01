Test Design Techniques ⭐⭐⭐⭐⭐ VVIP
=================================

These techniques help us **design effective test cases without testing every possible input**.

For interviews, focus mainly on **Equivalence Partitioning + Boundary Value Analysis**. The others are also commonly asked conceptually.

* * * * *

1\. Equivalence Partitioning (EP) ⭐⭐⭐⭐⭐
=======================================

### What is it?

We divide input values into **groups/partitions where the application is expected to behave similarly**, then test a representative value from each group.

### Example

**Age field accepts 18--60**

We can divide it into:

| Partition | Values | Example Test Value |
| --- | --- | --- |
| Invalid | `< 18` | 17 |
| Valid | `18--60` | 30 |
| Invalid | `> 60` | 61 |

Instead of testing every age from 1 to 100, we test **representative values from each partition**.

### Interview answer:

> Equivalence Partitioning divides input data into valid and invalid groups, and we test representative values from each group.

**Remember:**\
👉 **EP = Divide into groups**

* * * * *

2\. Boundary Value Analysis (BVA) ⭐⭐⭐⭐⭐
=======================================

### What is it?

We test values **at and around the boundaries**, because defects commonly occur at boundary conditions.

### Example

**Age = 18--60**

Test:

| Boundary | Values |
| --- | --- |
| Lower boundary | **17, 18, 19** |
| Upper boundary | **59, 60, 61** |

So the important values are:

**17, 18, 19, 59, 60, 61**

### Interview answer:

> Boundary Value Analysis focuses on testing values at and around the minimum and maximum boundaries.

**Remember:**\
👉 **BVA = Test edges**

* * * * *

🔥 EP vs BVA
============

| Equivalence Partitioning | Boundary Value Analysis |
| --- | --- |
| Divides data into groups | Focuses on boundaries |
| Tests representative values | Tests values around limits |
| Example: 17, 30, 61 | Example: 17, 18, 19, 59, 60, 61 |
| **Groups** | **Edges** |

### ⭐ Very common interview question:

**"For a field accepting 1--100, what values would you test?"**

Using **EP:**

> 0, 50, 101

Using **BVA:**

> 0, 1, 2, 99, 100, 101

* * * * *

3\. Decision Table Testing ⭐⭐⭐⭐
===============================

Used when the output depends on **multiple conditions/business rules**.

### Example:

Login requires:

-   Valid username
-   Valid password

| Username | Password | Expected |
| --- | --- | --- |
| Valid | Valid | Login successful |
| Valid | Invalid | Login failed |
| Invalid | Valid | Login failed |
| Invalid | Invalid | Login failed |

👉 We create combinations of conditions and verify the expected result.

### Interview answer:

> Decision Table Testing is used when different combinations of conditions produce different outcomes.

**Remember:**\
👉 **Decision Table = Conditions + combinations**

* * * * *

4\. State Transition Testing ⭐⭐⭐⭐
=================================

Used when application behavior changes based on its **current state or previous action**.

### Example: Account Lock

Suppose after **3 failed login attempts**, account gets locked.

| Action | State |
| --- | --- |
| 1st failed attempt | Active |
| 2nd failed attempt | Active |
| 3rd failed attempt | Locked |

Then test:

> Try logging in after the account is locked → Login should not be allowed.

Another common example:

**Order:**

`Placed → Shipped → Delivered → Cancelled`

We verify whether valid state transitions happen correctly.

### Interview answer:

> State Transition Testing verifies how the application behaves when it moves from one state to another based on user actions or events.

**Remember:**\
👉 **State = Current condition → Action → New condition**

* * * * *

5\. Use Case Testing ⭐⭐⭐
========================

Used to test **complete user/business scenarios**.

### Example: E-commerce

**Use case:** Place an order

Flow:

**Login → Search Product → Add to Cart → Checkout → Payment → Order Confirmation**

We test the complete business flow.

👉 This is especially relevant to **E2E testing**.

### Interview answer:

> Use Case Testing derives test cases from real user/business workflows to verify complete scenarios.

**Remember:**\
👉 **Use Case = User's real-world journey**

* * * * *

6\. Error Guessing ⭐⭐⭐⭐
=======================

This is based on the tester's **experience and knowledge of common mistakes** to predict where defects might occur.

There are no fixed rules/formulas.

### Example:

For a login page, an experienced tester may test:

-   Blank username
-   Blank password
-   Very long username
-   Special characters
-   Copy-paste password
-   Multiple failed login attempts
-   SQL injection-like input

Why?

Because these are **common areas where defects may occur**.

### Interview answer:

> Error Guessing is a testing technique where testers use their experience and knowledge of common defects to identify additional test cases.

**Remember:**\
👉 **Error Guessing = Tester experience**

* * * * *

🔥 All Techniques in One Table
==============================

| Technique | Main Idea | Easy Memory |
| --- | --- | --- |
| **Equivalence Partitioning** | Divide inputs into groups | **Groups** |
| **Boundary Value Analysis** | Test values around limits | **Edges** |
| **Decision Table** | Test combinations of conditions | **Combinations** |
| **State Transition** | Test state changes | **States** |
| **Use Case Testing** | Test real user/business workflows | **User journey** |
| **Error Guessing** | Predict defects using experience | **Experience** |

* * * * *

⭐ Most Important Interview Question
===================================

### "How would you test an age field that accepts 18--60?"

A strong answer:

> I would use Equivalence Partitioning and Boundary Value Analysis. For Equivalence Partitioning, I would divide the values into three groups: below 18, 18--60, and above 60, and test representative values like 17, 30, and 61. For Boundary Value Analysis, I would test values around the boundaries: 17, 18, 19, 59, 60, and 61.
