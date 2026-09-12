# LeetCode 876 - Middle of the Linked List

## Problem

Given the head of a singly linked list, return the middle node of the linked list.

If there are two middle nodes, return the **second middle node**.

### Example 1

**Input:**
```text
head = [1,2,3,4,5]
```

**Output:**
```text
[3,4,5]
```

### Example 2

**Input:**
```text
head = [1,2,3,4,5,6]
```

**Output:**
```text
[4,5,6]
```

---

## Approach

This solution uses **Linked List Traversal**.

### Steps

1. Traverse the linked list once to calculate its length.
2. Find the middle position using `length / 2`.
3. Reset the pointer to `head`.
4. Move the pointer `length / 2` times.
5. Return the node reached.

Using integer division automatically gives the **second middle node** when the list contains an even number of nodes.

## Complexity Analysis

Let `n` be the number of nodes.

- **Time Complexity:** `O(n)`
- **Space Complexity:** `O(1)`

The list is traversed a constant number of times and only a few variables are used.

## Key Concepts

- Linked Lists
- List Traversal
- Finding the Middle Node
- Integer Division
- Pointer Manipulation
- Even and Odd Length Lists
- Constant Space

## Alternative Approach

A common alternative is the **Slow and Fast Pointer** technique:

- `slow` moves one node at a time.
- `fast` moves two nodes at a time.
- When `fast` reaches the end, `slow` points to the middle node.

This approach finds the middle in one traversal with `O(1)` extra space.

## LeetCode

**Problem:** 876. Middle of the Linked List

**Difficulty:** Easy

**Language:** Java

**Topics:** Linked List, Two Pointers
