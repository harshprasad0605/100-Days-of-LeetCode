# LeetCode 455 - Assign Cookies

## Problem

Given two integer arrays:

- `g[i]` is the greed factor of child `i`.
- `s[j]` is the size of cookie `j`.

Each child can receive at most one cookie. A cookie can satisfy a child when `s[j] >= g[i]`.

Return the **maximum number of children** that can be satisfied.

### Example

**Input:**
```text
g = [1,2,3]
s = [1,1]
```

**Output:**
```text
1
```

**Explanation:** Only the child with greed factor `1` can be satisfied.

---

## Approach

This problem can be solved using a **Greedy + Two Pointer approach**.

The main idea is to satisfy the **least greedy child with the smallest possible cookie**.

### Steps

1. Sort the greed factors in ascending order.
2. Sort the cookie sizes in ascending order.
3. Use two pointers: one for children and one for cookies.
4. If the current cookie can satisfy the current child (`cookie >= greed`), assign it and move to the next child.
5. Always move to the next cookie.
6. Continue until we run out of cookies or children.
7. Return the number of satisfied children.

Using the smallest suitable cookie prevents larger cookies from being wasted and maximizes the number of satisfied children.


## Complexity Analysis

Let `n` be the number of children and `m` be the number of cookies.

- **Time Complexity:** `O(n log n + m log m)`
- **Space Complexity:** `O(log n + log m)` auxiliary space for Java's sorting operations.

## Key Concepts

- Greedy Algorithm
- Two Pointer Technique
- Sorting
- Arrays
- Optimization
- Problem Solving

## LeetCode

**Problem:** 455. Assign Cookies

**Difficulty:** Easy

**Language:** Java

**Topics:** Greedy, Two Pointers, Sorting
