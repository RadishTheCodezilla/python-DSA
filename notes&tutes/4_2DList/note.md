# 📚 2D Lists in Python — Complete Guide

---

## 📌 What is a 2D List?

A **2D list** in Python is essentially a **list of lists**.  
Think of it as a **table or grid** with **rows and columns** — where each element of the outer list is itself a list.

✅ Similar to a **matrix** in mathematics.

---

## 📌 How to Create a 2D List

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
```
This creates a 3x3 grid (3 rows and 3 columns).
---

## 📌 Accessing Elements in a 2D List
```python
print(matrix[0][1])  # Output: 2
```
matrix[0] → first row [1, 2, 3]

matrix[0][1] → second element of the first row: 2
---

## 📌 Traversing a 2D List
Using nested loops:
```python
for row in matrix:
    for item in row:
        print(item, end=" ")
    print()
```

## 📌 Modifying a 2D List
Change a value:
```python
matrix[1][2] = 10
```

Add a new row:
```python
matrix.append([10, 11, 12])
```
---

## 📌 Why Use 2D Lists in AI?

✅ To represent **matrices** in mathematical operations  
✅ For storing **image data** (each pixel’s RGB values as a grid)  
✅ To manage **game grids, pathfinding maps, or simulations**  
✅ For **adjacency matrices** in graph algorithms  
✅ Before **NumPy arrays**, 2D lists served as basic multi-dimensional data containers  

---

## 📌 Limitations of 2D Lists (and When to Prefer NumPy)

❌ Slower for large data operations  
❌ No built-in vectorised operations  
❌ Memory-inefficient for AI use cases  

✅ **NumPy arrays** are preferred for heavy numerical or AI tasks since they’re faster, memory-efficient, and support powerful operations like matrix multiplication, reshaping, and slicing.

---

## 📌 Key Takeaways

✅ A 2D list is a list of lists — like a table or matrix  
✅ Useful for storing and manipulating structured data  
✅ Can be traversed with nested loops  
✅ **NumPy arrays** are a better alternative for large, high-performance AI applications  
