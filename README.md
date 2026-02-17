# Stack Space & Time Complexity

This repository contains a C++ implementation of the **Stack** data structure along with explanations and analysis of **space and time complexity** for its operations.

---

## 📌 Overview

A **Stack** is a linear data structure that follows the **LIFO (Last In, First Out)** principle. Elements are added and removed from one end only — the top.

This project includes:
- A dynamic stack implementation using arrays
- Handling of overflow and underflow
- Time complexity analysis for key operations
- Space complexity analysis
- Example usage

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `main.cpp` | Implementation of stack functions and demonstration |
| `README.md` | This documentation file |
| `ComplexityAnalysis.pdf` *(optional)* | Notes on time and space complexity |

---

## 🧠 Stack Operations Covered

The following operations are implemented and analyzed in this project:

| Operation | Description |
|-----------|-------------|
| `create()` | Initialize a stack |
| `push()` | Add an element to the stack |
| `pop()` | Remove the top element |
| `peek()` | Get element at a specific position |
| `isEmpty()` | Check if stack has no elements |
| `isFull()` | Check if stack has reached capacity |
| `traverse()` | Print all elements |

---

## 📊 Time Complexity Summary

| Operation | Time Complexity |
|-----------|----------------|
| `push()` | O(1) *(amortized)* |
| `pop()` | O(1) |
| `peek()` | O(1) |
| `isEmpty()` | O(1) |
| `isFull()` | O(1) |
| `traverse()` | O(n) |

> **Note:**  
> - `push()` has amortized O(1) time if implemented with dynamic resizing (doubling).
> - If resizing happens during push, that particular push may take O(n) time, but averaged over many operations it remains O(1).

---

## 📏 Space Complexity

| Resource | Space Complexity |
|----------|------------------|
| Stack storage | O(n) |

Where `n` is the number of elements stored in the stack.

---


## 🛠 How to Build and Run

**Compile:**
```bash
g++ -o stack main.cpp

Run:

./stack

```


## 💡 Example

```cpp

Stack st;
st.size = 5;
create(&st);

push(&st, 10);
push(&st, 20);
push(&st, 30);

cout << "Popped element: " << pop(&st) << endl;

```


## ⚠ Notes

- Overflow is handled by checking before pushing.

- Underflow is handled by checking before popping.

- This implementation uses dynamic memory allocation, so free() or equivalent must be used to release memory.

## 📌 About the Author

* This repository is maintained by Avinandan Bose, focusing on clear and practical implementations of data structures and algorithm analysis.

## 📜 License

This project is released under the MIT License.

