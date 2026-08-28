# LeetCode 452 - Minimum Number of Arrows to Burst Balloons

## Problem

You are given a 2D integer array `points`, where `points[i] = [xstart, xend]` represents a balloon whose horizontal diameter stretches from `xstart` to `xend`.

An arrow can be shot vertically from any point on the x-axis. An arrow bursts every balloon whose range contains the arrow's x-coordinate.

Return the **minimum number of arrows** required to burst all the balloons.

### Example

**Input:**
```text
points = [[10,16],[2,8],[1,6],[7,12]]
```

**Output:**
```text
2
```

**Explanation:**

- Shoot an arrow at `x = 6` to burst `[2,8]` and `[1,6]`.
- Shoot another arrow at `x = 12` to burst `[10,16]` and `[7,12]`.

Therefore, the minimum number of arrows is `2`.

---

## Approach

This problem can be solved using a **Greedy Algorithm**.

The key idea is to sort the balloons by their **ending x-coordinate**.

### Steps

1. Sort the intervals in ascending order of their ending coordinate.
2. Place the first arrow at the end of the first balloon.
3. Traverse the remaining balloons.
4. If the current balloon starts after the position of the last arrow, the current balloon cannot be burst by that arrow.
5. Shoot a new arrow at the current balloon's ending coordinate.
6. Continue until all balloons are processed.

By always placing the arrow at the earliest possible ending point, we maximize the number of balloons that can be burst with the same arrow.


## Complexity Analysis

Let `n` be the number of balloons.

- **Time Complexity:** `O(n log n)`  
  Sorting takes `O(n log n)` time, followed by an `O(n)` traversal.

- **Space Complexity:** `O(n)`  
  The sorting operation may require additional space depending on the Java implementation.

## Key Concepts

- Greedy Algorithm
- Interval Scheduling
- Sorting
- 2D Arrays
- Custom Comparator
- Optimization
- Problem Solving

## LeetCode

**Problem:** 452. Minimum Number of Arrows to Burst Balloons

**Difficulty:** Medium

**Language:** Java

**Topics:** Greedy, Intervals
