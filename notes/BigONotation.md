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
```

## 📌 Rules of Thumb

- **Drop constants and non-dominant terms.**
  - `O(3n + 5)` → `O(n)`
  - `O(n² + n)` → `O(n²)`
- **Nested loops** → multiply their complexities.
- **Consecutive independent operations** → take the highest.

---

## 📌 Big O for Common AI/Data Science Operations

| Operation                          | Big O                          |
|:----------------------------------|:--------------------------------|
| Accessing an array element        | `O(1)`                          |
| Linear search                     | `O(n)`                          |
| Binary search                     | `O(log n)`                      |
| Matrix multiplication             | `O(n³)` (or better with optimised algorithms) |
| Sorting (QuickSort, MergeSort)    | `O(n log n)`                    |
| k-Nearest Neighbours (brute force)| `O(n)` per query                |

---

## 📌 Best, Average, and Worst Case

Some algorithms behave differently depending on the input.

**Example:** QuickSort

- **Best:** `O(n log n)`
- **Average:** `O(n log n)`
- **Worst:** `O(n²)`

---

## 📌 Big O and Neural Networks

- **Training time** often depends on number of layers, neurons per layer, and dataset size.

**Example:**

- **Forward pass:** `O(n)` per neuron  
- **Backpropagation:** similar or higher  
- **Total per epoch:** depends on number of parameters and data points.

**Optimising AI models often involves reducing complexity:**

- Using mini-batches (instead of full-batch)
- Dimensionality reduction (PCA, t-SNE)
- Approximate algorithms

---

## 📌 Visual Intuition

As `n` increases:

- `O(1)` stays flat
- `O(log n)` grows slowly
- `O(n)` grows linearly
- `O(n log n)` steeper than linear
- `O(n²)` grows very fast
- `O(2ⁿ)` and `O(n!)` explode rapidly

---

## 📌 Key Takeaways

✅ Big O helps **compare algorithm performance**  
✅ Focuses on how algorithms **scale with input size**  
✅ Both **time and space complexity** matter in AI applications  
✅ Always aim for **lower complexity algorithms** for large data problems  
✅ Some AI-specific optimisations include **parallelisation, batching, and dimensionality reduction**

---

## 🎯 Pro Tip for AI Aspirants

When working with AI libraries like **TensorFlow**, **PyTorch**, or **scikit-learn** — understanding underlying complexities will help you:

- Choose the right algorithm for your dataset size.
- Predict runtime and memory use.
- Optimise bottlenecks in model training.

