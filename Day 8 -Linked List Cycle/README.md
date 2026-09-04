# LeetCode 141 - Linked List Cycle

## Problem

Given the head of a linked list, determine if the linked list has a cycle in it.

A cycle exists if there is some node in the list that can be reached again by continuously following the `next` pointer.

Return `true` if there is a cycle in the linked list. Otherwise, return `false`.

## Approach

This problem can be solved using **Floyd's Cycle Detection Algorithm**, also known as the **Slow and Fast Pointer technique**.

### Steps

1. Initialize `slow` and `fast` at the head.
2. Move `slow` one node at a time.
3. Move `fast` two nodes at a time.
4. If a cycle exists, `fast` will eventually meet `slow`.
5. If `fast` or `fast.next` becomes `null`, there is no cycle.
6. Return `true` when both pointers meet; otherwise return `false`.

## Complexity Analysis

Let `n` be the number of nodes.

- **Time Complexity:** `O(n)`
- **Space Complexity:** `O(1)`

## Key Concepts

- Linked Lists
- Floyd's Cycle Detection
- Slow and Fast Pointers
- Cycle Detection
- Two Pointer Technique
- Constant Space
- Problem Solving

## LeetCode

**Problem:** 141. Linked List Cycle

**Difficulty:** Easy

**Language:** Java

**Topics:** Linked List, Two Pointers
