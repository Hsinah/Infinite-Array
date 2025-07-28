# Infinite-Array
# 🔍 Infinite Sorted Array Search in Java

This repository provides a Java implementation to find the **position of an element in a sorted array of infinite size**.

📖 Inspired by the article:  
➡️ [GeeksforGeeks – Find Position of Element in Sorted Infinite Array](https://www.geeksforgeeks.org/dsa/find-position-element-sorted-array-infinite-numbers/)

---

## 🧠 Problem Statement

Given an infinite sorted array (i.e., size is unknown), the goal is to find the index of a target element efficiently.

---

## 🚀 Approach

Since the array is infinite (or assumed to be), traditional binary search can’t be applied directly. Here's how this solution works:

1. **Range Expansion**:  
   Start with a small window (`start = 0`, `end = 1`) and double the window size until `arr[end] >= target`.

2. **Binary Search**:  
   Once the range is found, perform a standard binary search between `start` and `end`.
