# Day 3: Reverse an Array

## 🚀 Challenge
Reverse the elements of a given array without using any in-built functions.

### 📂 Problem Statement
Given an array of integers, reverse the array so that the first element becomes the last, the second element becomes the second last, and so on.

---

## 💡 Approaches Explored

### 1️⃣ **Naive Approach**
- **Logic:** Use an additional array to store elements in reverse order.
- **Time Complexity:** O(n)
- **Space Complexity:** O(n)

### 2️⃣ **Optimized In-Place Approach**
- **Logic:** Use two pointers—one starting from the beginning and the other from the end—to swap elements.
- **Time Complexity:** O(n)
- **Space Complexity:** O(1)

---

## ✨ Key Learnings
- Reinforced the importance of understanding in-place algorithms to reduce space complexity.
- Practiced swapping elements using indices effectively.
- Recognized the relevance of reversing arrays in various real-world scenarios like reversing strings, managing datasets, and implementing algorithms.

---

## 🔗 Why This Problem Matters
Reversing an array is a fundamental operation in programming that appears in data manipulation, algorithm design, and real-world applications like processing data structures or creating efficient solutions for recursive problems.

---

## Example

### Input:
`arr = [1, 2, 3, 4, 5]`

### Output:
`[5, 4, 3, 2, 1]`
