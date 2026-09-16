# LeetCode 53 - Maximum Subarray

## Problem

Given an integer array `nums`, find the **subarray with the largest sum** and return its sum.

### Example

**Input:**
```text
nums = [-2,1,-3,4,-1,2,1,-5,4]
```

**Output:**
```text
6
```

**Explanation:** The subarray `[4,-1,2,1]` has the largest sum of `6`.

---

## Approach

This problem can be solved using **Kadane's Algorithm**.

### Steps

1. Initialize `maxSum` with the first element.
2. Maintain `currSum` for the best subarray sum ending at the current position.
3. Add each element to `currSum`.
4. Update `maxSum` with the larger value.
5. If `currSum` becomes negative, reset it to `0`.
6. Continue through the entire array.
7. Return `maxSum`.

The key idea is to discard a negative running sum because it would only reduce the sum of any future subarray.

## Complexity Analysis

Let `n` be the length of the array.

- **Time Complexity:** `O(n)`
- **Space Complexity:** `O(1)`

The array is traversed once and no additional data structures are used.

## Key Concepts

- Kadane's Algorithm
- Dynamic Programming
- Greedy Approach
- Arrays
- Subarrays
- Running Sum
- Optimization
- Problem Solving

## LeetCode

**Problem:** 53. Maximum Subarray

**Difficulty:** Medium

**Language:** Java

**Topics:** Array, Divide and Conquer, Dynamic Programming
