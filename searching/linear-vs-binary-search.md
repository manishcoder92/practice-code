# 🧠 Linear Search vs Binary Search

## 📌 What

Both are searching algorithms used to find an element in a list.

---

## 🔍 Linear Search

### ✔️ How it works

* Check each element one by one
* Stop when element is found

### 💻 Code

```python
arr = [5, 3, 7, 1, 9]
target = 7

for num in arr:
    if num == target:
        print("Found")
```

### ⏱ Complexity

* Time: O(n)

---

## ⚡ Binary Search

### ✔️ How it works

* Works on sorted arrays
* Divide the array into halves
* Check middle element

### 💻 Code

```python
arr = [1, 2, 3, 4, 5, 6, 7]
target = 4

low, high = 0, len(arr) - 1

while low <= high:
    mid = (low + high) // 2

    if arr[mid] == target:
        print("Found")
        break
    elif arr[mid] < target:
        low = mid + 1
    else:
        high = mid - 1
```

### ⏱ Complexity

* Time: O(log n)

---

## ⚖️ Key Differences

| Feature         | Linear Search | Binary Search |
| --------------- | ------------- | ------------- |
| Requirement     | No sorting    | Sorted array  |
| Time Complexity | O(n)          | O(log n)      |
| Speed           | Slow          | Fast          |

---

## 🎯 Conclusion

* Use Linear Search for small or unsorted data
* Use Binary Search for large sorted data
