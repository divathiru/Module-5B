# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd

student_data1 = {
    'name': ['Alice', 'Bob', 'Charlie'],
    'age': [20, 21, 19],
    'grade': ['A', 'B', 'C']
}

student_data2 = {
    'name': ['David', 'Eva', 'Frank'],
    'age': [22, 20, 21],
    'grade': ['B', 'A', 'A']
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

combined_df = pd.concat([df1, df2], axis=0, ignore_index=True)

print(combined_df)
```

## Output
![image](https://github.com/user-attachments/assets/021083c4-40fd-4354-bf66-6cf772abce26)

## Result
The Python program to concatenate two DataFrames row-wise has been executed successfully, and the output has been verified.
