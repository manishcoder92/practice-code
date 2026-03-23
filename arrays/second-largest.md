# 🧠 Second Largest Element in Array

## 📌 What

Find the second largest element in a given array.

## ❓ Why

* Helps build strong comparison logic
* Frequently asked in coding interviews

## ⚙️ How

* Initialize two variables: first and second
* Traverse the array
* Update values accordingly

## 💻 Code

```python
arr = [3, 7, 2, 9, 5]

first = second = float('-inf')

for num in arr:
    if num > first:
        second = first
        first = num
    elif num > second and num != first:
        second = num

print(second)
```

## ⏱ Complexity

* Time Complexity: O(n)
* Space Complexity: O(1)
