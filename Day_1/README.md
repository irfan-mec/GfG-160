# Second Largest Element in an Array

Given an array of positive integers arr[] of size n, the task is to find second largest distinct element in the array.

Note: If the second largest element does not exist, return -1.

---


## Examples:

**Input**: arr[] = [12, 35, 1, 10, 34, 1]
**Output**: 34
Explanation: The largest element of the array is 35 and the second largest element is 34.
---
**Input**: arr[] = [10, 5, 10]
**Output**: 5
Explanation: The largest element of the array is 10 and the second largest element is 5.
---
**Input**: arr[] = [10, 10, 10]
**Output**: -1
Explanation: The largest element of the array is 10 there is no second largest element.

---

**One Pass Search - O(n) Time and O(1) Space**
The idea is to keep track of the largest and second largest element while traversing the array. Initialize largest and second largest with -1. Now, for any index i,

If arr[i] > largest, update second largest with largest and largest with arr[i].
Else If arr[i] < largest and arr[i] > second largest, update second largest with arr[i].