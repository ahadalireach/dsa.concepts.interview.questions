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

### [Array Representations](#array-representations)

| No. | Questions |
| --- | ----------------------------------------------------------------- |
| 1   | [What is an Array?](#what-is-an-array) |
| 2   | [What are Dynamic Arrays?](#what-are-dynamic-arrays) |
| 3   | [What are Static Arrays?](#what-are-static-arrays) |
| 4   | [What is a 2D Array?](#what-is-a-2d-array) |
| 5   | [What defines the Dimensionality of an array?](#what-defines-the-dimensionality-of-an-array) |
| 6   | [Advantages and Disadvantages of Arrays](#advantages-and-disadvantages-of-arrays) |


### [Array as ADT (Abstract Data Type)](#array-as-adt-abstract-data-type)

| No. | Questions |
| --- | ----------------------------------------------------------------- |
| 1   | [What does it mean by Array ADT?](#what-does-it-mean-by-array-adt) |
| 2   | [How to Add / Append?](#how-to-add-append) |
| 3   | [How to Insert?](#how-to-insert) |
| 4   | [How to Delete?](#how-to-delete) |
| 5   | [How to Search?](#how-to-search) |
| 6   | [What is Linear Search?](#what-is-linear-search) |
| 7   | [How to improve Linear Search (Move to Head / Move to Front)?](#how-to-improve-linear-search-move-to-head-move-to-front) |
| 8  | [What is Binary Search?](#what-is-binary-search) |
| 9  | [Difference between Linear and Binary Search?](#difference-between-linear-and-binary-search) |
| 10  | [How to Get, Set, Find Min - Max?](#how-to-get-set-find-min-max) |
| 11  | [How to Reverse and Shift an Array?](#how-to-reverse-and-shift-an-array) |
| 12  | [Left Shift / Rotation?](#left-shift-rotation) |
| 13  | [Right Shift / Rotation?](#right-shift-rotation) |
| 14  | [Insert into Sorted Array?](#insert-into-sorted-array) |
| 15  | [Check if an Array is Sorted?](#check-if-an-array-is-sorted) |
| 16  | [Arranging Negative Numbers on Left Side?](#arranging-negative-numbers-on-left-side) |
| 17  | [Merge Arrays?](#merge-arrays) |
| 18  | [Set Operations (Union, Intersection, Difference)?](#set-operations-union-intersection-difference) |
| 19  | [Find Missing Element (Single Missing, Multiple Missing)?](#find-missing-element-single-missing-multiple-missing) |
| 20  | [Find Duplicate Elements?](#find-duplicate-elements) |
| 21  | [Finding a Pair with Sum K?](#finding-a-pair-with-sum-k) |
| 22  | [Reverse an Array?](#reverse-an-array) |
| 23  | [Find Two Elements with Difference Equal to S in a Sorted Array?](#find-two-elements-with-difference-equal-to-s-in-a-sorted-array) |
| 24  | [Find Array Elements that are Neither Minimum nor Maximum?](#find-array-elements-that-are-neither-minimum-nor-maximum) |
| 25  | [Find 2nd Maximum or Minimum Element?](#find-2nd-maximum-or-minimum-element) |


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

#### <a id="types-of-data-structures"></a>🤷‍♂️ Types of Data Structures

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

#### ⏱️ Quick Guide to Measuring Time Complexity

#### 1. Loop-Based Patterns

| Pattern | Code Example | Time Complexity |
|---------|-------------|----------------|
| Single Loop | `for (int i = 0; i < n; i++)` | O(n) |
| Nested Loops | `for (int i = 0; i < n; i++)` `for (int j = 0; j < n; j++)` | O(n²) |
| Triple Nested Loops | `for (int i = 0; i < n; i++)` `for (int j = 0; j < n; j++)` `for (int k = 0; k < n; k++)` | O(n³) |
| Loop with Increment (`i *= 2`) | `for (int i = 1; i < n; i *= 2)` | O(log n) |
| Loop with Decrement (`i /= 2`) | `for (int i = n; i > 0; i /= 2)` | O(log n) |

#### 2. Recursive Patterns

| Pattern | Recurrence Relation | Time Complexity |
|---------|---------------------|----------------|
| Linear Recursion | `T(n) = T(n-1) + O(1)` | O(n) |
| Binary Recursion | `T(n) = 2T(n/2) + O(1)` | O(n) |
| Divide & Conquer (Merge Sort, Quick Sort Worst Case) | `T(n) = 2T(n/2) + O(n)` | O(n log n) |
| Exponential Recursion (Fibonacci, Brute Force DFS) | `T(n) = T(n-1) + T(n-2)` | O(2ⁿ) |

#### 3. Divide and Conquer Patterns

| Algorithm | Recurrence | Complexity |
|-----------|------------|------------|
| Binary Search | `T(n) = T(n/2) + O(1)` | O(log n) |
| Merge Sort | `T(n) = 2T(n/2) + O(n)` | O(n log n) |
| Quick Sort (Best & Avg) | `T(n) = T(n/2) + O(n)` | O(n log n) |
| Quick Sort (Worst Case - sorted array) | `T(n) = T(n-1) + O(n)` | O(n²) |

#### 4. Dynamic Programming Patterns

| Pattern | Example | Time Complexity |
|---------|---------|----------------|
| Memoization (Top-Down Recursion with Cache) | Fibonacci DP | O(n) |
| Bottom-Up Iterative DP | Knapsack, LIS | O(n²) or O(n³) |
| Matrix Chain Multiplication | `T(n) = O(n³)` | O(n³) |

#### 5. Graph Algorithms

| Algorithm | Complexity |
|-----------|------------|
| BFS / DFS (Adjacency List) | O(V + E) |
| Dijkstra (Min Heap) | O((V + E) log V) |
| Bellman-Ford | O(VE) |
| Floyd Warshall (All-Pairs Shortest Path) | O(V³) |
| Prim’s / Kruskal’s MST | O(E log V) |

#### 6. Sorting Algorithms

| Algorithm | Best Case | Worst Case |
|-----------|------------|------------|
| Bubble Sort / Insertion Sort | O(n) | O(n²) |
| Merge Sort | O(n log n) | O(n log n) |
| Quick Sort | O(n log n) | O(n²) |
| Heap Sort | O(n log n) | O(n log n) |

#### 7. Logarithmic and Amortized Complexities

| Pattern | Example | Complexity |
|---------|---------|------------|
| Binary Search | Search in sorted array | O(log n) |
| Heap Operations (Insert/Delete) | Priority Queue, Dijkstra | O(log n) |
| Balanced BST (Insertion, Deletion, Search) | AVL, Red-Black Tree | O(log n) |
| Union-Find (Path Compression & Rank) | DSU operations | O(α(n)) (inverse Ackermann) |

#### 8. Special Cases

| Case | Example |
|------|---------|
| Iterating All Subsets | O(2ⁿ) |
| Iterating All Permutations | O(n!) |
| Brute Force Checking All Pairs | O(n²) |

---

### 💾 Quick Guide to Calculating Space Complexity

#### 1. What is Space Complexity?
Space Complexity is the total memory required by a program to execute. It includes:
1. Fixed Part – Independent of input size (e.g., code, static/global variables, constants).
2. Variable Part – Depends on input size (e.g., dynamic memory allocation, function call stack, recursion depth).

#### 2. Components of Space Complexity
##### a) Fixed Memory (O(1))
- Code Space: Memory occupied by compiled instructions.
- Constant Space: Fixed-size variables, constants.
- Global & Static Variables: Memory allocated at program startup, remains till termination.

##### b) Variable Memory (Depends on Input)
- Stack Space: Used for function calls (parameters, return addresses, local variables).
- Heap Space: Memory dynamically allocated using `new` in Java/C++, `malloc()` in C.
- Data Structures: Arrays, lists, trees, hash tables, etc.

#### 3. Steps to Calculate Space Complexity
##### Step 1: Analyze Fixed Space
```cpp
int a = 10, b = 20; // Fixed space O(1)
```
##### Step 2: Analyze Variable Space
```cpp
int[] arr = new int[n]; // Takes O(n) space
```
##### Step 3: Analyze Function Calls & Stack Usage
```cpp
void recursive(int n) {
    if (n == 0) return;
    recursive(n - 1);
} // O(n) stack space
```
##### Step 4: Consider Auxiliary Space
```cpp
int[] newArray = new int[n]; // O(n) auxiliary space
```

#### 4. Space Complexity Analysis for Common Data Structures

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

#### 5. Space Complexity of Common Algorithms

##### Iterative Algorithm (O(1))
```cpp
void printArray(int arr[], int n) {
    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";
    }
} // O(1) space
```

##### Recursive Algorithm (O(n))
```cpp
int factorial(int n) {
    if (n == 0) return 1;
    return n * factorial(n - 1);
} // O(n) stack space
```

##### Sorting Algorithms

| Algorithm | Auxiliary Space |
|-----------|----------------|
| Bubble Sort | O(1) |
| Merge Sort | O(n) |
| Quick Sort (in-place) | O(log n) |
| Heap Sort | O(1) |

#### 6. Best Practices for Optimizing Space Complexity
- Use In-Place Algorithms
- Use Iteration Instead of Recursion
- Choose Space-Efficient Data Structures
- Free Memory When Not Needed

**[⬆ Back to Top](#table-of-contents)**

---
---
---

## <a id="array-representations"></a>Array Representations

### What is an Array?
- Array is like a container that is use to store some kind of data or collection of elements.
- It is a linear data structure. And have contiguous memory locations.
- It allows easy access to elements using an index.
- Example:
  ```cpp
  int arr[5] = {1, 2, 3, 4, 5};
  ```

**[⬆ Back to Top](#table-of-contents)**

---

### What are Dynamic Arrays?
- A **dynamic array** can change its size during runtime.
- It is implemented using pointers and memory allocation functions like `new` in C++.
- Can grow or shrink during runtime using `new` and `delete`.
- ```cpp
  int *arr = new int[10];
  ```
- ```cpp
  #include<iostream>
  using namespace std;

  int main(){
      int *arr = new int[5];
      for(int i = 0; i < 5; i++){
          cout << "Enter " << i + 1 << " element: ";
          cin >> arr[i];
      }
      delete[] arr;
  }
  ```

**[⬆ Back to Top](#table-of-contents)**

---

### What are Static Arrays?
- A **static array** has a fixed size determined at compile time.
- Fixed-size memory allocation.
- Cannot grow or shrink dynamically.
-
  ```cpp
  int arr[10];
  ```

**[⬆ Back to Top](#table-of-contents)**

---

```cpp
#include<iostream>
using namespace std;

int main(){
    int *a = new int[5];

    for(int i = 0; i < 5; i++){
        cout << "Enter " << i + 1 << " element: ";
        cin >> a[i];
    }

    char i;
    cout << "Do you want to increase the size of array? (Y/N): ";
    cin >> i;

    if(i == 'Y'){
        int num;
        cout << "\nEnter number of elements you want to add: ";
        cin >> num;

        int *b = new int[5 + num];

        for(int i = 0; i < 5; i++){
            b[i] = a[i];
        }

        for(int i = 5; i < 5 + num; i++){
            cout << "Enter " << i + 1 << " element: ";
            cin >> b[i];
        }

        delete[] a;
        a = b;
        b = nullptr;

        for(int i = 0; i < 5 + num; i++){
            cout << a[i] << " ";
        }
    }else{
        for(int i = 0; i < 5; i++){
            cout << a[i] << " ";
        }
    }

    delete[] a;
}
```

---

### Advantages and Disadvantages of Arrays

| **Advantages**                                     | **Disadvantages**                                      |
|--------------------------------------------------|------------------------------------------------------|
| Fast access to elements using an index.         | Fixed size (static arrays) cannot be resized.       |
| Efficient memory usage for storing similar data. | Insertion and deletion are costly due to shifting.  |
| Easier to traverse using loops.                  | - |

**[⬆ Back to Top](#table-of-contents)**

---

### What is a 2D Array?

- A **2D array** represents data in a tabular format with rows and columns.
- Commonly used to implement matrices.
- Accessed using two indices (one for row and one for column).
```cpp
int matrix[3][3] = {
      {1, 2, 3},
      {4, 5, 6},
      {7, 8, 9}
  };
  ```

**[⬆ Back to Top](#table-of-contents)**

---

### What defines the Dimensionality of an Array?
- The number of indices needed to access an element defines the **dimensionality** of an array.
- Example:
  - **1D Array:** `arr[5]`
  - **2D Array:** `arr[3][3]`
  - **3D Array:** `arr[3][3][3]`

**[⬆ Back to Top](#table-of-contents)**


---

### Methods/Ways of Declaring 2D Arrays

#### 1. Normal Declaration

- Memory will be created like a single dimension array , but compiler will allow us to access that array as a 2D arrays with rows and columns.
```cpp
int A[3][4] = {
    {1,2,3,4},
    {2,4,6,8},
    {3,5,7,9}
};
```

#### 2. Array of Pointers

- The pointer will be created inside heap memory and through that we can access , initialise and declare all the elements inside the array. This is array of arrays.
```cpp
int *A[3];
A[0] = new int[4];
A[1] = new int[4];
A[2] = new int[4];
```
```cpp
int row, col;
cout << "Number of rows, col: ";
cin >> row >> col;
int *A[row];
for(int i = 0; i < row; i++){
    A[i] = new int[col];
}

for(int i = 0; i < row; i++){
    for(int j = 0; j < col; j++){
        cout << "Enter A[" << i << "][" << j << "] element: ";
        cin >> A[i][j];
    }
}

for(int i = 0; i < row; i++){
    for(int j = 0; j < col; j++){
        cout << A[i][j] << " ";
    }
    cout << endl;
}

for(int i = 0; i < row; i++){
    delete[] A[i];
}

delete[] A;
```

#### 3. Double Pointer Method

- Almost everything is inside the heap pointer.
- The pointer acts like a variable; there is no `new` operator for it, so it is created inside the stack.

```cpp
int **A;
A = new int*[3];
for(int i = 0; i < 3; i++){
    A[i] = new int[4];
}
```
```cpp
int **A;
    A = new int*[3]; // Allocating memory for 3 rows
    for(int i = 0; i < 3; i++){
        A[i] = new int[4]; // Allocating memory for 4 columns in each row
    }

    // Example usage: Assigning values
    for(int i = 0; i < 3; i++){
        for(int j = 0; j < 4; j++){
            A[i][j] = (i + 1) * (j + 1); // Sample values
        }
    }

    // Displaying the 2D array
    cout << "2D Array Elements:\n";
    for(int i = 0; i < 3; i++){
        for(int j = 0; j < 4; j++){
            cout << A[i][j] << " ";
        }
        cout << endl;
    }

    // Freeing allocated memory
    for(int i = 0; i < 3; i++){
        delete[] A[i]; // Deleting columns
    }
    delete[] A; // Deleting row pointers
```

**[⬆ Back to Top](#table-of-contents)**

---
---
---

## <a id="array-as-adt-abstract-data-type"></a>Array as ADT (Abstract Data Type)

### What is Array ADT?

An **Array ADT (Abstract Data Type)** consists of:
1. **Data Representation** (handled by the compiler)
2. **Operations on Data** (defined by the program)

#### **Key Components of Array ADT:**
- **Data:**
  - **Array space** → Memory allocated for the array.
  - **Size** → Total allocated memory.
  - **Length** → Number of elements currently stored.

- **Operations:**
  - `Display()` → Show all elements.
  - `Add(x)` / `Append(x)` → Add an element at the end.
  - `Insert(index, x)` → Insert an element at a specific position.
  - `Delete(index)` → Remove an element.
  - `Search(x)` → Find an element.
  - `Get(index)` → Retrieve an element at a specific position.
  - `Set(index, x)` → Update an element.
  - `Max / Min` → Find the maximum or minimum element.
  - `Reverse` → Reverse the array.
  - `Shift / Rotate` → Move elements left or right.

- `size = 10`, but only `length = 5` elements are used in an array.
- This means 5 slots are empty but allocated in memory.

**[⬆ Back to Top](#table-of-contents)**

---

### How to Add / Append?

Adding or **appending** means inserting an element at the **end** of an array.

- The new element is stored at the next available index.
- The **time complexity** is **O(1)** (constant time) since we are adding at the end.

```cpp
arr[length] = x;  // Insert element at the next index
length++;         // Increase the length of the array
```

**[⬆ Back to Top](#table-of-contents)**

---


---

### How to Insert?

Insertion means adding an element at a **specific index** in the array.

#### Time Complexity:
- **Best case (O(1))** → When inserting at the **end**.
- **Worst case (O(n))** → When inserting at the **beginning** (as elements need to be shifted).

```cpp
#include <iostream>
using namespace std;

class Arr {
    private:
        int *A;
        int length;
        int size;

    public:
        Arr(int size) {
            this->size = size;
            A = new int[size];
            length = 0;
        }

        void insert(int num) {
            if (length < size) {
                A[length] = num;
                length++;
            } else {
                cout << "Array is full!" << endl;
            }
        }

        void add(int index, int num) {
            if (index < 0 || index > length) {
                cout << "Invalid index!" << endl;
                return;
            }
            if (length == size) {
                cout << "Array is full!" << endl;
                return;
            }
            for (int i = length; i > index; i--) {
                A[i] = A[i - 1];
            }
            A[index] = num;
            length++;
        }

        void display() {
            for (int i = 0; i < length; i++) {
                cout << A[i] << " ";
            }
            cout << endl;
        }

        ~Arr() {
            delete[] A;
            cout << "Array destroyed" << endl;
        }
};

int main() {
    Arr ar(5);
    ar.insert(1);
    ar.insert(2);
    ar.insert(3);
    ar.insert(5);
    ar.add(3, 4);
    ar.display();
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to Delete?

**Deletion** means removing an element from a **specific index** in the array.

#### Time Complexity:
- **O(n)** → Because elements must be shifted after deletion.

```cpp
void del(int index) {
    if (index >= 0 && index < length) {
        for (int i = index; i < length - 1; i++) {
            A[i] = A[i + 1];
        }
        length--;
    }
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to Search?

Searching involves finding an element in an array. The two main searching techniques are:
1. **Linear Search** → Works on both sorted and unsorted arrays.
2. **Binary Search** → Works only on sorted arrays for faster searching.

**[⬆ Back to Top](#table-of-contents)**


---

### What is Linear Search?
- Linear search is a simple searching algorithm where we traverse the array element by element until we find the key.
- If we find the element in the array, we return its index; otherwise, we return `-1` to indicate it is not present.
- The value we are searching for is called the **key**.

#### Time Complexity
- **Best case time complexity:** `O(1)` (when the key is found at the first position).
- **Worst case time complexity:** `O(n)` (when the key is at the last position or not present at all).

```cpp
#include <iostream>
using namespace std;

int search(int arr[], int size, int key) {
    for(int i = 0; i < size; i++) {
        if(arr[i] == key) {
            return i; // Return index if found
        }
    }
    return -1; // Return -1 if not found
}

int main() {
    int arr[] = {10, 20, 30, 40, 50};
    int size = sizeof(arr) / sizeof(arr[0]);
    int key = 30;

    int result = search(arr, size, key);
    if (result != -1)
        cout << "Element found at index: " << result << endl;
    else
        cout << "Element not found" << endl;

    return 0;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to Improve Linear Search (Move to Head / Move to Front)?

#### Optimization Techniques:
##### 1. **Transposition:**
Move the recently searched element one step forward for faster future access.
#### 2. **Move to Front (Move to Head):**
Move the frequently searched element to the beginning of the array.


##### **1. Transposition:**
In this technique, when we find the element, we swap it with the previous element. This ensures that frequently accessed elements move closer to the start over time.

```cpp
#include <iostream>
using namespace std;

class Arr {
    public:
        int arr[10] = {1, 3, 5, 7, 9, 10, 8, 6, 4, 2};

        int search(int key) {
            for (int i = 0; i < 10; i++) {
                if (arr[i] == key) {
                    if (i != 0) {
                        swap(&arr[i], &arr[i - 1]);
                        return i - 1;
                    }
                    return i;
                }
            }
            return -1;
        }

        void swap(int *arr1, int *arr2) {
            int temp = *arr2;
            *arr2 = *arr1;
            *arr1 = temp;
        }
};

int main() {
    Arr arr1;
    cout << "Element found at index: " << arr1.search(4) << endl;
}
```

##### **2. Move to Front (Move to Head)**

In this method, whenever an element is found, we swap it with the first element.
This ensures that the most frequently searched elements stay at the beginning.

```cpp
#include <iostream>
using namespace std;

class Arr {
    public:
        int arr[10] = {1, 3, 5, 7, 9, 10, 8, 6, 4, 2};

        int search(int key) {
            for (int i = 0; i < 10; i++) {
                if (arr[i] == key) {
                    if (i != 0) {
                        swap(&arr[i], &arr[0]);
                        return 0;
                    }
                    return i;
                }
            }
            return -1;
        }

        void swap(int *arr1, int *arr2) {
            int temp = *arr2;
            *arr2 = *arr1;
            *arr1 = temp;
        }
};

int main() {
    Arr arr1;
    cout << "Element found at index: " << arr1.search(2) << endl;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### What is Binary Search?

- Works only on **sorted** arrays.
- Always searches for the **middle element** and splits the array into two halves.
- **Time Complexity:** `O(log n)`

#### **Process:**
1. If `key == middle element` → ✅ **Found**.
2. If `key < middle element` → 🔍 Search in **left half**.
3. If `key > middle element` → 🔍 Search in **right half**.


```cpp
// Iterative
#include <iostream>
using namespace std;

class Arr {
    public:
        int arr[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

        int search(int key) {
            int l = 0, h = 9;
            int mid;
            while (l <= h) {
                mid = (l + h) / 2;
                if (key == arr[mid])
                    return mid;
                else if (key < arr[mid])
                    h = mid - 1;
                else
                    l = mid + 1;
            }
            return -1;
        }
};

int main() {
    Arr arr1;
    cout << "Element found at index: " << arr1.search(11) << endl;
}
```

```cpp
// Recursive
#include <iostream>
using namespace std;

class Arr {
    public:
        int arr[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

        int search(int key, int l, int h) {
            if (l <= h) {
                int mid = (l + h) / 2;
                if (key == arr[mid])
                    return mid;
                else if (key < arr[mid])
                    return search(key, l, mid - 1);
                else
                    return search(key, mid + 1, h);
            }
            return -1;
        }
};

int main() {
    Arr arr1;
    cout << "Element found at index: " << arr1.search(10, 0, 9) << endl;
}
```

#### **Analysis of Binary Search**

##### Time Complexity: `O(log n)`

- The complexity is determined by the number of comparisons from tracing the **binary tree**.


##### For Successful Search:
- **Best case:** `O(1)`
- **Worst case:** `O(log n)`

##### For Unsuccessful Search:
- Always `O(log n)`, whether using **recursion** or **iteration**.

---

### Difference Between Linear and Binary Search:

| **Search Type**     | **Best Case** | **Worst Case** | **Works on Sorted Array?** |
|---------------------|--------------|---------------|--------------------------|
| **Linear Search**   | `O(1)`       | `O(n)`        | Yes (But Complexity is High)                     |
| **Binary Search**   | `O(1)`       | `O(log n)`    | Yes                    |


**[⬆ Back to Top](#table-of-contents)**

---
