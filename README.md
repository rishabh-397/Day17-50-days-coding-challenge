# Day17-50-days-coding-challenge
## 🔹 Problem 1: Design a Min Stack

### Problem Statement:
Design a stack that supports:
- `push(int val)`
- `pop()`
- `top()`
- `getMin()` – returns the **minimum element** in the stack  
**All in constant time – O(1)**.

### ✅ Example:
```plaintext
Input: ["MinStack","push","push","push","getMin","pop","top","getMin"]
       [[],[-2],[0],[-3],[],[],[],[]]
Output: [null,null,null,null,-3,null,0,-2]
💡 Approach:
Maintain two stacks:

Main stack for values

Min stack to track the current minimum

Each time you push(), compare with current min and push onto minStack accordingly.

🔹 Problem 2: Two Sum
Problem Statement:
Given nums[] and a target, return the indices of two numbers that add up to the target.
Each input has exactly one solution.

✅ Example:
Input: nums = [2,7,11,15], target = 9 → Output: [0, 1]

Input: nums = [3,2,4], target = 6 → Output: [1, 2]

Input: nums = [3,3], target = 6 → Output: [0, 1]

💡 Approach:
Use a hashmap to store value -> index.

For each number, check if target - num is already in the map.

