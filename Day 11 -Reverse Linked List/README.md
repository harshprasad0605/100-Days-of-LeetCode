# LeetCode 206 - Reverse Linked List

## Problem

Given the head of a singly linked list, reverse the list and return the reversed list.

### Example

**Input:**
```text
head = [1,2,3,4,5]
```

**Output:**
```text
[5,4,3,2,1]
```

---

## Approach

This problem can be solved using **Iterative Linked List Reversal**.

### Steps

1. Initialize `prev` as `null` and `curr` as `head`.
2. Store the next node in a temporary variable.
3. Reverse the current node's pointer using `curr.next = prev`.
4. Move `prev` to `curr`.
5. Move `curr` to the stored next node.
6. Continue until `curr` becomes `null`.
7. Return `prev`, which is the new head.

The key idea is to reverse each `next` pointer one at a time while keeping track of the remaining list.

## Complexity Analysis

Let `n` be the number of nodes.

- **Time Complexity:** `O(n)`
- **Space Complexity:** `O(1)`

Each node is visited exactly once and no extra data structure is used.

## Key Concepts

- Linked Lists
- Iterative Traversal
- Pointer Manipulation
- In-Place Reversal
- Two Pointers
- Constant Space
- Problem Solving

## LeetCode

**Problem:** 206. Reverse Linked List

**Difficulty:** Easy

**Language:** Java

**Topics:** Linked List, Recursion
