# 🧠 Binary Search

## 📌 What

Binary Search is an efficient algorithm used to find an element in a sorted array.

## ❓ Why

* Much faster than linear search
* Important for large datasets
* Frequently asked in interviews

## ⚙️ How

* Find the middle element
* Compare it with the target
* If equal → found
* If smaller → search right half
* If larger → search left half

## 💻 Code

```python
arr = [1, 2, 3, 4, 5, 6, 7]
target = 4

low, high = 0, len(arr) - 1

while low <= high:
    mid = (low + high) // 2

    if arr[mid] == target:
        print("Element found")
        break
    elif arr[mid] < target:
        low = mid + 1
    else:
        high = mid - 1
```

## ⏱ Complexity

* Time Complexity: O(log n)
* Space Complexity: O(1)

## ⚠️ Note

Binary search works only on sorted arrays.
