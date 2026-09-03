# LeetCode 83 - Remove Duplicates from Sorted List

## Problem

Given the head of a **sorted linked list**, delete all duplicates so that each element appears only once.

Return the linked list after removing the duplicates. The list should remain sorted.

### Example

**Input:**
```text
head = [1,1,2]
```

**Output:**
```text
[1,2]
```

Another example:

```text
Input:  [1,1,2,3,3]
Output: [1,2,3]
```

---

## Approach

This problem can be solved using a **Two Pointer / Linked List Traversal approach**.

Since the linked list is already sorted, duplicate values will always appear next to each other.

### Steps

1. Start with `curr` at the head of the list.
2. Keep `prev` at the last unique node.
3. Traverse the list.
4. If `curr.val == prev.val`, skip the duplicate using `prev.next = curr.next`.
5. Otherwise, move `prev` to `curr`.
6. Continue until the end of the list.
7. Return the original `head`.

Because the list is sorted, we only need to compare the current node with the previous unique node.

## Complexity Analysis

Let `n` be the number of nodes.

- **Time Complexity:** `O(n)` — each node is visited once.
- **Space Complexity:** `O(1)` — only a constant number of pointers are used.

## Key Concepts

- Linked Lists
- Two Pointer Technique
- Duplicate Removal
- Pointer Manipulation
- Sorted Data
- Constant Space
- Problem Solving

## LeetCode

**Problem:** 83. Remove Duplicates from Sorted List

**Difficulty:** Easy

**Language:** Java

**Topics:** Linked List, Two Pointers
