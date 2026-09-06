# LeetCode 2 - Add Two Numbers

## Problem

You are given two non-empty linked lists representing two non-negative
integers. The digits are stored in **reverse order**, and each node
contains a single digit. Add the two numbers and return the sum as a
linked list.

### Example

**Input:** `l1 = [2,4,3]`, `l2 = [5,6,4]`

**Output:** `[7,0,8]`

**Explanation:** `342 + 465 = 807`

## Approach

Use linked-list traversal with a **carry**. Traverse both lists
together, add the current digits and carry, store `sum % 10`, and update
`carry = sum / 10`. A dummy node makes result construction simple.
Continue while either list has nodes or a carry remains.

## Complexity Analysis

-   **Time Complexity:** `O(max(m, n))`
-   **Space Complexity:** `O(max(m, n))` for the output list.

## Key Concepts

-   Linked Lists
-   Carry Handling
-   Dummy Node
-   Pointer Manipulation
-   Mathematical Operations

## LeetCode

**Problem:** 2. Add Two Numbers

**Difficulty:** Medium

**Language:** Java

**Topics:** Linked List, Math, Recursion
