# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np

rows = int(input())
cols = int(input())

print("Enter the elements of the 2D array row-wise:")
arr = []
for _ in range(rows):
    row = list(map(int, input().split()))
    arr.append(row)
arr = np.array(arr)

print("Enter the new column elements:")
new_col = list(map(int, input().split()))
new_col = np.array(new_col).reshape(rows, 1)

arr = np.delete(arr, 1, axis=1)
updated_arr = np.insert(arr, 1, new_col, axis=1)

print("Updated array:")
print(updated_arr)
```

## Output
![image](https://github.com/user-attachments/assets/b69e4d74-1e5f-440f-ae8e-88c818898a2a)


## Result
The Python program using NumPy to delete and replace a column in a 2D array has been executed successfully, and the output has been verified.
