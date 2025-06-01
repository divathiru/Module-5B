# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np

rows = int(input())
cols = int(input())

print("Enter the elements row-wise:")
arr = []
for _ in range(rows):
    row = list(map(int, input().split()))
    arr.append(row)

arr = np.array(arr)
sorted_arr = np.sort(arr, axis=0)

print("Original array:")
print(arr)

print("Column-wise sorted array:")
print(sorted_arr)
```
## Output
![image](https://github.com/user-attachments/assets/565be803-97ff-4e0f-b354-3a813c75b915)

## Result
The Python program using NumPy to sort a 2D array column-wise has been executed successfully, and the output has been verified.
