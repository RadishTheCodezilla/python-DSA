# 📚 Linked Lists in Python — Complete Note

---

## 📌 What is a Linked List?

A **Linked List** is a **linear data structure** where elements (called **nodes**) are stored in **non-contiguous memory locations**. Each node contains:

- **Data (value)**
- A **reference (or pointer) to the next node** in the sequence.

Unlike arrays, linked lists don’t require a fixed size and allow **efficient insertion and deletion** of elements.

---

## 📌 Why Use Linked Lists?

- **Dynamic size** — grows and shrinks as needed.
- **Efficient insertions/deletions** at arbitrary positions without shifting elements.
- Useful when the **number of elements is unknown in advance**.
- Helpful in implementing other data structures like **stacks, queues, and graphs**.

---

## 📌 Types of Linked Lists

| Type                  | Description                                  |
|:----------------------|:---------------------------------------------|
| **Singly Linked List**  | Each node points to the next node             |
| **Doubly Linked List**  | Each node points to both next and previous nodes |
| **Circular Linked List**| The last node points back to the first node   |

---

## 📌 Common Linked List Operations

| Operation  | Description                                        |
|:------------|:---------------------------------------------------|
| **Insertion** | Add a new node at the beginning, middle, or end    |
| **Deletion**  | Remove a node from a specific position             |
| **Traversal** | Visit each node to perform an action (like printing)|
| **Search**    | Find if a value exists in the list                 |

---

## 📌 Advantages of Linked Lists

✅ Dynamic size — no need to define initial size  
✅ Easy insertion and deletion without shifting elements  
✅ Efficient memory usage for large, unpredictable data sets  

---

## 📌 Disadvantages of Linked Lists

❌ Extra memory for storing pointers  
❌ No random access — elements accessed sequentially  
❌ Slower search than arrays (linear time O(n))  

---

## 📌 Use Cases in AI / Programming

- Memory-efficient storage for variable-sized data  
- Implementing **queues, stacks, hash tables, adjacency lists**  
- Handling **large dynamic datasets** in algorithms  
- Managing sequences in **game AI, simulations, and agent-based models**  

---

## 📌 Key Takeaways

✅ Linked Lists store elements in nodes connected by pointers  
✅ They are dynamic, flexible, and efficient for insertions/deletions  
✅ Python supports linked lists via custom classes  
✅ Important in AI when managing complex data structures or graphs  
