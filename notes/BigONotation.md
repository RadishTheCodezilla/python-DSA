# 📚 Big O Notation — Notes for AI Engineers

---

## 📌 What is Big O Notation?

**Big O Notation** describes the **time complexity** and **space complexity** of an algorithm as a function of the input size, denoted as `n`.  
It gives an upper bound on the growth rate of an algorithm, helping us understand how it performs as the input grows large.

---

## 📌 Why is Big O Important in AI & Data Science?

- **Data volumes** are massive in AI; algorithms need to scale well.
- **Optimising model training time** (e.g. feature selection, sorting, or searching in datasets)
- **Resource efficiency** in production AI systems (memory and computation cost)
- **Choosing between different algorithms** for tasks like matrix multiplication, nearest neighbour searches, or clustering.

---

## 📊 Common Big O Time Complexities (with Examples)

| Big O       | Name               | Example Use Case in AI                     |
|:------------|:-------------------|:-------------------------------------------|
| `O(1)`     | Constant Time        | Accessing an element in a list by index    |
| `O(log n)` | Logarithmic Time     | Binary search in a sorted dataset          |
| `O(n)`     | Linear Time          | Traversing a dataset to compute mean       |
| `O(n log n)` | Linearithmic Time  | Efficient sorting (e.g. Merge Sort)        |
| `O(n²)`    | Quadratic Time       | Comparing every pair (e.g. distance matrix)|
| `O(2ⁿ)`    | Exponential Time     | Recursive combinatorial problems          |
| `O(n!)`    | Factorial Time       | Solving Travelling Salesman Problem        |

---

## 📌 Space Complexity

Same concept as time complexity, but focuses on how much **additional memory** an algorithm uses relative to input size `n`.

**Example:**
- Storing an extra array of size `n` → `O(n)`
- Using a few variables → `O(1)`

---

## 📌 How to Analyse Time Complexity

1. **Identify the operations that repeat based on input size.**
2. **Count the most dominant operations as `n` grows.**
3. **Ignore lower-order terms and constants.**

**Example:**
```python
for i in range(n):         # O(n)
    for j in range(n):     # O(n)
        print(i, j)        # O(1)

Total: O(n²)
        
