# LeetCode 24 - Swap Nodes in Pairs

## Problem

Given a linked list, swap every two adjacent nodes and return its head.

The node values must not be changed. Only the links between nodes may be modified.

### Example

**Input:**
```text
head = [1,2,3,4]
```

**Output:**
```text
[2,1,4,3]
```

---

## Approach

This problem can be solved using a **Dummy Node + Pointer Manipulation** approach.

### Steps

1. Create a dummy node pointing to `head`.
2. Use `prev` to track the node before the current pair.
3. Use `cur` to point to the first node of the current pair.
4. Check that both `cur` and `cur.next` exist.
5. Store the second node and the node after the pair.
6. Reverse the two nodes by changing their `next` pointers.
7. Connect `prev` to the second node.
8. Move the pointers to the next pair.
9. Return `dummy.next`.

Example:

```text
1 -> 2 -> 3 -> 4
```

becomes:

```text
2 -> 1 -> 4 -> 3
```

The values remain unchanged; only the links are modified.

## Complexity Analysis

Let `n` be the number of nodes.

- **Time Complexity:** `O(n)`
- **Space Complexity:** `O(1)`

Each node is processed once and only a constant number of pointers are used.

## Key Concepts

- Linked Lists
- Pointer Manipulation
- Dummy Node
- Node Swapping
- In-Place Operations
- Iterative Approach
- Constant Space
- Problem Solving

## Important Edge Cases

- Empty list
- Single-node list
- Odd number of nodes
- Even number of nodes

For an odd-sized list, the final node remains in its original position.

## LeetCode

**Problem:** 24. Swap Nodes in Pairs

**Difficulty:** Medium

**Language:** Java

**Topics:** Linked List, Recursion
