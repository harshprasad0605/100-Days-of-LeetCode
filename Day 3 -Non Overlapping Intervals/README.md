# LeetCode 435 - Non-overlapping Intervals

## Problem

Given an array of intervals `intervals`, where `intervals[i] = [starti, endi]`, return the **minimum number of intervals that must be removed** to make the remaining intervals non-overlapping.

Intervals that only touch at a point are considered non-overlapping. For example, `[1,2]` and `[2,3]` do not overlap.

### Example

**Input:**
```text
intervals = [[1,2],[2,3],[3,4],[1,3]]
```

**Output:**
```text
1
```

**Explanation:** Remove `[1,3]`. The remaining intervals are non-overlapping.

---

## Approach

This problem is solved using a **Greedy Algorithm**.

The main idea is to keep the interval that ends earliest. When two intervals overlap, the interval with the smaller ending point leaves more room for future intervals.

### Steps

1. Sort all intervals by their ending point in ascending order.
2. Store the ending point of the last interval that was kept.
3. Traverse the remaining intervals.
4. If the current interval starts before `lastEnd`, the intervals overlap, so remove the current interval.
5. Otherwise, keep the current interval and update `lastEnd`.
6. Return the number of removed intervals.

This greedy strategy maximizes the number of non-overlapping intervals that can be kept.


## Complexity Analysis

Let `n` be the number of intervals.

- **Time Complexity:** `O(n log n)` because of sorting.
- **Space Complexity:** `O(n)` auxiliary space for Java's sorting implementation.

## Key Concepts

- Greedy Algorithm
- Interval Scheduling
- Sorting
- Overlapping Intervals
- 2D Arrays
- Optimization
- Problem Solving

## LeetCode

**Problem:** 435. Non-overlapping Intervals

**Difficulty:** Medium

**Language:** Java

**Topics:** Greedy, Sorting, Intervals
