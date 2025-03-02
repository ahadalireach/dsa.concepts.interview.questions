# Data Structures and Algorithms (DSA) - Concepts & Interview Questions

## <a id="table-of-contents"></a>Table of Contents

### [Introduction to DSA](#introduction-to-dsa)

| No. | Questions |
| --- | ----------------------------------------------------------------- |
| 1   | [What is Data Structure?](#what-is-data-structure) |
| 2   | [How is Data Organized in Memory?](#how-is-data-organized-in-memory) |
| 3   | [Stack vs Heap Memory](#stack-vs-heap-memory) |
| 4   | [Types of Data Structures](#types-of-data-structures) |
| 5   | [Time and Space Complexity](#time-and-space-complexity) |

---

## <a id="introduction-to-dsa"></a>Introduction to DSA

### What is Data Structure? 📂

- A **Data Structure** is a way of organizing and storing data in memory during program execution.
- It allows **efficient storage, retrieval, and manipulation** of data.
- Data structures use **algorithms** to structure data efficiently in memory.

**[⬆ Back to Top](#table-of-contents)**

---

### How is Data Organized in Memory?

The way data is stored in main memory for efficient access is called a **Data Structure**.
Memory is divided into three main sections:

1. **Code Section** 🖥️
   - Contains the program's executable instructions.
   - Execution starts from this section.

2. **Stack Section** 📌
   - Stores function calls and local variables.
   - Uses **Last In, First Out (LIFO)** order.
   - Memory is **statically allocated** and automatically managed.

3. **Heap Section** 📂
   - Stores dynamically allocated memory (e.g., `malloc()` in C or `new` in C++/Java).
   - Accessed via **pointers**.
   - Memory needs to be **manually managed** (deallocation required).

**[⬆ Back to Top](#table-of-contents)**

---

### Stack vs Heap Memory

| Feature   🔥 | Stack Memory 📌 | Heap Memory 📂 |
|-------------|---------------|---------------|
| Allocation  | Static        | Dynamic       |
| Access Speed | Faster        | Slower       |
| Size        | Limited       | Large        |
| Lifetime    | Auto-managed  | Manually managed (deallocation required) |
| Usage      | Function calls, local variables | Dynamic objects, large data structures |

- The **stack** is efficient but limited in size.
- The **heap** is flexible but requires proper memory management.

**[⬆ Back to Top](#table-of-contents)**

---

### <a id="types-of-data-structures"></a>🤷‍♂️ Types of Data Structures

#### **Physical Data Structures**
- Define how data is stored in memory.
  - **Array**: Fixed size, used when the max size is known.
  - **Linked List**: Dynamic, stored in heap, suitable when size is unknown.

#### **Logical Data Structures**
- Define data operations like searching & sorting.
  - **Stack**: Last In, First Out (LIFO)
  - **Queue**: First In, First Out (FIFO)
  - **Tree & Graph**: Non-linear structures
  - **Hash Table**: Key-value pairs for quick lookup

**[⬆ Back to Top](#table-of-contents)**

---

### <a id="time-and-space-complexity"></a>Time and Space Complexity

#### **⏳ Time Complexity**

- Measures algorithm efficiency as input size increases.
- Ignoring constants: `O(n + 1) → O(n)`.
- Common complexities:
  - `O(1)`: Constant time (random access in an array).
  - `O(log n)`: Logarithmic time (Binary Search).
  - `O(n)`: Linear time (Loop through an array).
  - `O(n log n)`: Quasi-linear (Merge Sort, Quick Sort).
  - `O(n²)`: Quadratic time (Bubble Sort, Insertion Sort).

#### **🗄️ Space Complexity**

- Determines memory usage based on input size.
- Includes auxiliary space (extra space required apart from input data).

**[⬆ Back to Top](#table-of-contents)**

---

## ⏱️ Quick Guide to Measuring Time Complexity

### 1. Loop-Based Patterns

| Pattern | Code Example | Time Complexity |
|---------|-------------|----------------|
| Single Loop | `for (int i = 0; i < n; i++)` | O(n) |
| Nested Loops | `for (int i = 0; i < n; i++)` `for (int j = 0; j < n; j++)` | O(n²) |
| Triple Nested Loops | `for (int i = 0; i < n; i++)` `for (int j = 0; j < n; j++)` `for (int k = 0; k < n; k++)` | O(n³) |
| Loop with Increment (`i *= 2`) | `for (int i = 1; i < n; i *= 2)` | O(log n) |
| Loop with Decrement (`i /= 2`) | `for (int i = n; i > 0; i /= 2)` | O(log n) |

### 2. Recursive Patterns

| Pattern | Recurrence Relation | Time Complexity |
|---------|---------------------|----------------|
| Linear Recursion | `T(n) = T(n-1) + O(1)` | O(n) |
| Binary Recursion | `T(n) = 2T(n/2) + O(1)` | O(n) |
| Divide & Conquer (Merge Sort, Quick Sort Worst Case) | `T(n) = 2T(n/2) + O(n)` | O(n log n) |
| Exponential Recursion (Fibonacci, Brute Force DFS) | `T(n) = T(n-1) + T(n-2)` | O(2ⁿ) |

### 3. Divide and Conquer Patterns

| Algorithm | Recurrence | Complexity |
|-----------|------------|------------|
| Binary Search | `T(n) = T(n/2) + O(1)` | O(log n) |
| Merge Sort | `T(n) = 2T(n/2) + O(n)` | O(n log n) |
| Quick Sort (Best & Avg) | `T(n) = T(n/2) + O(n)` | O(n log n) |
| Quick Sort (Worst Case - sorted array) | `T(n) = T(n-1) + O(n)` | O(n²) |

### 4. Dynamic Programming Patterns

| Pattern | Example | Time Complexity |
|---------|---------|----------------|
| Memoization (Top-Down Recursion with Cache) | Fibonacci DP | O(n) |
| Bottom-Up Iterative DP | Knapsack, LIS | O(n²) or O(n³) |
| Matrix Chain Multiplication | `T(n) = O(n³)` | O(n³) |

### 5. Graph Algorithms

| Algorithm | Complexity |
|-----------|------------|
| BFS / DFS (Adjacency List) | O(V + E) |
| Dijkstra (Min Heap) | O((V + E) log V) |
| Bellman-Ford | O(VE) |
| Floyd Warshall (All-Pairs Shortest Path) | O(V³) |
| Prim’s / Kruskal’s MST | O(E log V) |

### 6. Sorting Algorithms

| Algorithm | Best Case | Worst Case |
|-----------|------------|------------|
| Bubble Sort / Insertion Sort | O(n) | O(n²) |
| Merge Sort | O(n log n) | O(n log n) |
| Quick Sort | O(n log n) | O(n²) |
| Heap Sort | O(n log n) | O(n log n) |

### 7. Logarithmic and Amortized Complexities

| Pattern | Example | Complexity |
|---------|---------|------------|
| Binary Search | Search in sorted array | O(log n) |
| Heap Operations (Insert/Delete) | Priority Queue, Dijkstra | O(log n) |
| Balanced BST (Insertion, Deletion, Search) | AVL, Red-Black Tree | O(log n) |
| Union-Find (Path Compression & Rank) | DSU operations | O(α(n)) (inverse Ackermann) |

### 8. Special Cases

| Case | Example |
|------|---------|
| Iterating All Subsets | O(2ⁿ) |
| Iterating All Permutations | O(n!) |
| Brute Force Checking All Pairs | O(n²) |

---

## 💾 Quick Guide to Calculating Space Complexity

### 1. What is Space Complexity?
Space Complexity is the total memory required by a program to execute. It includes:
1. Fixed Part – Independent of input size (e.g., code, static/global variables, constants).
2. Variable Part – Depends on input size (e.g., dynamic memory allocation, function call stack, recursion depth).

### 2. Components of Space Complexity
#### a) Fixed Memory (O(1))
- Code Space: Memory occupied by compiled instructions.
- Constant Space: Fixed-size variables, constants.
- Global & Static Variables: Memory allocated at program startup, remains till termination.

#### b) Variable Memory (Depends on Input)
- Stack Space: Used for function calls (parameters, return addresses, local variables).
- Heap Space: Memory dynamically allocated using `new` in Java/C++, `malloc()` in C.
- Data Structures: Arrays, lists, trees, hash tables, etc.

### 3. Steps to Calculate Space Complexity
#### Step 1: Analyze Fixed Space
```cpp
int a = 10, b = 20; // Fixed space O(1)
```
#### Step 2: Analyze Variable Space
```cpp
int[] arr = new int[n]; // Takes O(n) space
```
#### Step 3: Analyze Function Calls & Stack Usage
```cpp
void recursive(int n) {
    if (n == 0) return;
    recursive(n - 1);
} // O(n) stack space
```
#### Step 4: Consider Auxiliary Space
```cpp
int[] newArray = new int[n]; // O(n) auxiliary space
```

### 4. Space Complexity Analysis for Common Data Structures

| Data Structure | Space Complexity |
|---------------|-----------------|
| Array (1D) | O(n) |
| 2D Array | O(n²) |
| Linked List | O(n) |
| HashMap | O(n) |
| Tree (Balanced) | O(n) |
| Graph (Adjacency List) | O(V + E) |
| Stack (n elements) | O(n) |
| Queue (n elements) | O(n) |

### 5. Space Complexity of Common Algorithms

#### Iterative Algorithm (O(1))
```cpp
void printArray(int arr[], int n) {
    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";
    }
} // O(1) space
```

#### Recursive Algorithm (O(n))
```cpp
int factorial(int n) {
    if (n == 0) return 1;
    return n * factorial(n - 1);
} // O(n) stack space
```

#### Sorting Algorithms

| Algorithm | Auxiliary Space |
|-----------|----------------|
| Bubble Sort | O(1) |
| Merge Sort | O(n) |
| Quick Sort (in-place) | O(log n) |
| Heap Sort | O(1) |

### 6. Best Practices for Optimizing Space Complexity
- Use In-Place Algorithms
- Use Iteration Instead of Recursion
- Choose Space-Efficient Data Structures
- Free Memory When Not Needed

**[⬆ Back to Top](#table-of-contents)**

---
---
---
