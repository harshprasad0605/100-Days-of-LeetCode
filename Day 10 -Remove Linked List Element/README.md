# LeetCode 203 - Remove Linked List Elements

## Problem

Given the head of a linked list and an integer `val`, remove all nodes whose value is equal to `val`.

Return the new head of the linked list.

### Example

**Input:**
```text
head = [1,2,6,3,4,5,6], val = 6
```

**Output:**
```text
[1,2,3,4,5]
```

---

## Approach

This problem can be solved using **Linked List Traversal and Pointer Manipulation**.

### Steps

1. Remove matching nodes from the beginning of the list.
2. Use `curr` to traverse the remaining list.
3. Keep `prev` pointing to the previous node.
4. If `curr.val == val`, skip the current node using `prev.next = curr.next`.
5. Otherwise, move `prev` to `curr`.
6. Continue until the end of the list.
7. Return the updated `head`.

## Complexity Analysis

Let `n` be the number of nodes.

- **Time Complexity:** `O(n)`
- **Space Complexity:** `O(1)`

Each node is visited at most once and only a constant number of pointers are used.

## Key Concepts

- Linked Lists
- Linked List Traversal
- Pointer Manipulation
- Node Deletion
- Handling Head Nodes
- Constant Space
- Problem Solving

## LeetCode

**Problem:** 203. Remove Linked List Elements

**Difficulty:** Easy

**Language:** Java

**Topics:** Linked List, Recursion
