# LeetCode 19 - Remove Nth Node From End of List

## Problem

Given the head of a linked list, remove the `n`th node from the end of the list and return its head.

### Example 1

**Input:**
```text
head = [1,2,3,4,5], n = 2
```

**Output:**
```text
[1,2,3,5]
```

The 2nd node from the end is `4`, so it is removed.

### Example 2

**Input:**
```text
head = [1], n = 1
```

**Output:**
```text
[]
```

### Example 3

**Input:**
```text
head = [1,2], n = 1
```

**Output:**
```text
[1]
```

---

## Approach

This solution uses **Two Pointers**.

### Steps

1. Initialize two pointers, `ptr` and `temp`, at the head.
2. Move `ptr` `n` positions ahead.
3. If `ptr` becomes `null`, the node to remove is the head, so return `head.next`.
4. Move `ptr` and `temp` together until `ptr` reaches the last node.
5. At this point, `temp` points to the node just before the node that must be removed.
6. Skip the target node using `temp.next = temp.next.next`.
7. Return the original head.

The two pointers maintain a fixed distance of `n`, allowing the target node to be located without calculating the complete list length.

## Complexity Analysis

Let `L` be the number of nodes.

- **Time Complexity:** `O(L)`
- **Space Complexity:** `O(1)`

## Key Concepts

- Linked Lists
- Two Pointers
- Pointer Manipulation
- Node Deletion
- Edge Case Handling
- Constant Space

## LeetCode

**Problem:** 19. Remove Nth Node From End of List

**Difficulty:** Medium

**Language:** Java

**Topics:** Linked List, Two Pointers
