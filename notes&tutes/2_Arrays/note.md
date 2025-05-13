# 📚 Arrays — Complete Notes for AI & Programming

---

## 📌 What is an Array?

An **array** is a **data structure** that stores a collection of elements (values or variables) of the **same data type** in a **contiguous memory location**.

In simple terms:
- It’s like a list of items you can access by index.
- Arrays can be **one-dimensional (1D)**, **two-dimensional (2D)**, or **multi-dimensional**.

---

## 📌 Why are Arrays Important in AI & Data Science?

- **Efficient storage** of large numerical datasets.
- **Faster access** to elements via index positions.
- **Optimised for mathematical operations** (like matrix multiplication, vector addition, etc.)
- Used heavily in **image processing, machine learning models, and neural networks**.
- Libraries like **NumPy, TensorFlow, and PyTorch** rely on arrays (or multi-dimensional arrays called tensors).

---

## 📌 Array Types

| Type                    | Description                                      | Example                                       |
|:------------------------|:------------------------------------------------|:----------------------------------------------|
| **1D Array**             | A simple list of elements                        | `[1, 2, 3, 4]`                                |
| **2D Array**             | A table or matrix (array of arrays)              | `[[1, 2], [3, 4]]`                           |
| **Multi-dimensional Array** | More than 2 dimensions (3D, 4D, etc.)          | `[[[1,2], [3,4]], [[5,6], [7,8]]]`           |

---

## 📌 Arrays in Python  

### 📎 Using Python’s Native `list` as an Array

```python
my_list = [10, 20, 30, 40]
print(my_list[2])  # Output: 30
```
### 📎 Using the `array` Module

```python
import array as arr

numbers = arr.array('i', [1, 2, 3, 4])
print(numbers[1])  # Output: 2
```
### 📎 Using NumPy Arrays (Preferred in AI)

```python
import numpy as np

my_array = np.array([1, 2, 3, 4])
print(my_array[0])  # Output: 1
```
✅ Supports multi-dimensional arrays (2D, 3D, etc.)
✅ Allows vectorised operations (faster computations)

## 📌 Common Array Operations (NumPy)

| Operation             | Syntax Example               |
|:---------------------|:----------------------------|
| **Create 1D array**    | `np.array([1, 2, 3])`        |
| **Create 2D array**    | `np.array([[1, 2], [3, 4]])` |
| **Access element**     | `arr[0][1]`                  |
| **Array shape**        | `arr.shape`                  |
| **Array size**         | `arr.size`                   |
| **Reshape array**      | `arr.reshape(3, 2)`          |
| **Array addition**     | `arr1 + arr2`                |
| **Matrix multiplication** | `np.dot(arr1, arr2)`     |

---

## 📌 Advantages of Arrays

✅ Fast element access via index  
✅ Easy to traverse and modify  
✅ Memory-efficient (fixed type, contiguous memory in NumPy)  
✅ Supports vectorised operations (especially in AI)  
✅ Ideal for storing large, structured, numerical data  

---

## 📌 Disadvantages of Arrays

❌ Fixed size in traditional languages (C, Java)  
❌ All elements must be of the same type (in libraries like NumPy)  
❌ Insertion/deletion at arbitrary positions can be inefficient (shifting elements)  

---

## 📌 Use Cases in AI

- Storing dataset features and labels  
- Images as 2D or 3D arrays (RGB images)  
- Model weights in deep learning  
- Batch processing of data  
- Performing matrix operations for neural networks  

---

## 📌 Key Takeaways

✅ Arrays are structured, indexed collections of elements of the same type  
✅ Essential in AI and Data Science for efficient numerical operations  
✅ Python’s **NumPy** is the go-to library for arrays  
✅ Arrays can be **1D, 2D (matrices), or multi-dimensional (tensors)**
