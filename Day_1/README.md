# Second Largest Element in an Array

This repository contains a solution to the problem of finding the second largest distinct element in an array. The task is to identify the second largest element efficiently using a single pass.

---

## Problem Statement

Given an array of positive integers `arr[]` of size `n`, the goal is to find the second largest distinct element in the array.

### **Note**:  
If the second largest element does not exist, return `-1`.

---

## Examples

### Example 1:
**Input**:  
`arr[] = [12, 35, 1, 10, 34, 1]`  

**Output**:  
`34`  

**Explanation**:  
The largest element is `35` and the second largest is `34`.

---

### Example 2:
**Input**:  
`arr[] = [10, 5, 10]`  

**Output**:  
`5`  

**Explanation**:  
The largest element is `10` and the second largest is `5`.

---

### Example 3:
**Input**:  
`arr[] = [10, 10, 10]`  

**Output**:  
`-1`  

**Explanation**:  
The largest element is `10` but there is no second largest distinct element.

---

## Approach: One Pass Search

### **Time Complexity**: O(n)  
### **Space Complexity**: O(1)  

This solution uses a single traversal of the array to determine the second largest element while maintaining constant space.

### Algorithm:
1. Initialize `largest` and `secondLargest` to `-1`.
2. Traverse the array:
   - If `arr[i] > largest`:
     - Update `secondLargest = largest`
     - Update `largest = arr[i]`
   - Else if `arr[i] < largest` **and** `arr[i] > secondLargest`:
     - Update `secondLargest = arr[i]`
3. After the traversal, `secondLargest` will hold the second largest element.
4. If no second largest distinct element exists, return `-1`.

---
