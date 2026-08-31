# LeetCode 160 - Intersection of Two Linked Lists

## Problem

Given the heads of two singly linked lists `headA` and `headB`, return the node at which the two linked lists intersect.

If the two linked lists have no intersection, return `null`.

The linked lists must retain their original structure after the function returns.

### Example

```text
A: a1 -> a2
           \
            c1 -> c2 -> c3
           /
B: b1 -> b2 -> b3
```

The two linked lists intersect at node `c1`.

---

## Approach

This problem can be solved using the **Two Pointer Technique**.

The main idea is to make both pointers travel the same total distance.

### Steps

1. Initialize two pointers, `a` and `b`, at `headA` and `headB`.
2. Move both pointers one node at a time.
3. When pointer `a` reaches the end of List A, redirect it to `headB`.
4. When pointer `b` reaches the end of List B, redirect it to `headA`.
5. Continue until `a == b`.
6. If the lists intersect, both pointers meet at the intersection node.
7. If they do not intersect, both pointers eventually become `null`.

After switching heads, both pointers travel the same combined distance, so any difference in the original list lengths is cancelled out.


## Complexity Analysis

Let `m` be the length of List A and `n` be the length of List B.

- **Time Complexity:** `O(m + n)`
- **Space Complexity:** `O(1)`

The algorithm uses only two pointers and does not modify either linked list.

## Key Concepts

- Two Pointer Technique
- Linked Lists
- Intersection of Linked Lists
- Pointer Manipulation
- Constant Space
- Problem Solving

## LeetCode

**Problem:** 160. Intersection of Two Linked Lists

**Difficulty:** Easy

**Language:** Java

**Topics:** Linked List, Two Pointers
