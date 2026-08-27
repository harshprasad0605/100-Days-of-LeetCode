# LeetCode 1710 - Maximum Units on a Truck

## Problem

You are given a 2D integer array `boxTypes`, where:

- `boxTypes[i][0]` is the number of boxes of type `i`.
- `boxTypes[i][1]` is the number of units in each box of type `i`.

You are also given an integer `truckSize`, which represents the maximum number of boxes that can be loaded onto the truck.

The goal is to return the **maximum total number of units** that can be loaded onto the truck.

### Example

**Input:**
```text
boxTypes = [[1,3],[2,2],[3,1]]
truckSize = 4
```

**Output:**
```text
8
```

**Explanation:**

- Take 1 box with 3 units.
- Take 2 boxes with 2 units each.
- Take 1 box with 1 unit.

Total units = `3 + 2 + 2 + 1 = 8`.

---

## Approach

This problem can be solved using a **Greedy Algorithm**.

The main idea is to always choose boxes that provide the **maximum number of units per box** first.

### Steps

1. Sort `boxTypes` in descending order based on units per box.
2. Iterate through the sorted box types.
3. Take as many boxes as possible from the current type.
4. If the truck cannot fit all boxes of the current type, take only the remaining available capacity.
5. Add the corresponding units to the answer.
6. Stop when the truck is full.

Since taking a box with more units is always better than taking a box with fewer units, this greedy strategy gives the maximum possible total units.

## Complexity Analysis

Let `n` be the number of box types.

- **Time Complexity:** `O(n log n)`  
  Sorting the box types takes `O(n log n)` time, followed by an `O(n)` traversal.

- **Space Complexity:** `O(n)`  
  The sorting operation may require additional space depending on the Java implementation.

## Key Concepts

- Greedy Algorithm
- Sorting
- 2D Arrays
- Custom Comparator
- Optimization
- Problem Solving

## LeetCode

**Problem:** 1710. Maximum Units on a Truck

**Difficulty:** Easy

**Language:** Java

**Topic:** Greedy
