# LeetCode 21 - Merge Two Sorted Lists

## Problem

Given the heads of two sorted singly linked lists `list1` and `list2`, merge them into **one sorted linked list** by splicing together the nodes of the two lists.

Return the head of the merged linked list.

### Example

**Input:**
```text
list1 = [1,2,4]
list2 = [1,3,4]
```

**Output:**
```text
[1,1,2,3,4,4]
```

---

## Approach

This problem can be solved using a **Two Pointer + Linked List** approach.

### Steps

1. Handle cases where either list is empty.
2. Use two pointers to traverse both lists.
3. Compare the current node values.
4. Attach the smaller node to the merged list.
5. Move the pointer from the list whose node was selected.
6. Continue until one list becomes empty.
7. Attach the remaining nodes from the other list.
8. Return the head of the merged list.

The existing nodes are reused, so no new list of nodes is required.

## Complexity Analysis

Let `m` and `n` be the lengths of the two linked lists.

- **Time Complexity:** `O(m + n)`
- **Space Complexity:** `O(1)`

## Key Concepts

- Linked Lists
- Two Pointer Technique
- Merging Sorted Lists
- Pointer Manipulation
- Constant Space
- Problem Solving

## LeetCode

**Problem:** 21. Merge Two Sorted Lists

**Difficulty:** Easy

**Language:** Java

**Topics:** Linked List, Two Pointers
