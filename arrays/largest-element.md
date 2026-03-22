# 🧠 Largest Element in Array

## 📌 What

Find the largest element in a given array.

## ❓ Why

* It is a fundamental concept in data structures.
* Frequently asked in coding interviews.

## ⚙️ How

* Traverse through the array.
* Keep track of the maximum element found so far.

## 💻 Code

```python
arr = [3, 7, 2, 9, 5]

max_val = arr[0]

for num in arr:
    if num > max_val:
        max_val = num

print(max_val)  '''

## ⏱ Complexity

* Time Complexity: O(n)
* Space Complexity: O(1)
