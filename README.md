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
| 24 | [Finding Minimum and Maximum in a Single Scan?](#finding-minimum-and-maximum-in-a-single-scan) |
| 25  | [Find Array Elements that are Neither Minimum nor Maximum?](#find-array-elements-that-are-neither-minimum-nor-maximum) |
| 26  | [Find 2nd Maximum or Minimum Element?](#find-2nd-maximum-or-minimum-element) |
| 27  | [Find Elements in Range (0-100) with Frequency > 50](#find-elements-in-range-0-100-with-frequency--50) |


---

### [Strings](#strings)

| No. | Questions |
| --- | ----------------------------------------------------------------- |
| 1   | [What is character set?](#character-set) |
| 2   | [What is the ASCII of strings?](#ascii) |
| 3   | [What is string?](#strings) |
| 4   | [Difference b/w character set and strings?](#difference-between-character-set-and-strings) |
| 5   | [How to find Length of string?](#how-to-find-length-of-string) |
| 6   | [How to change case of strings?](#how-to-change-case-of-strings) |
| 7   | [How to count words, vowels and consonants in a string?] (#how-to-count-words-vowels-and-consonants-in-a-string) |
| 8   | [How to validate a string?](#how-to-validate-a-string) |
| 9   | [How to reverse a string?](#how-to-reverse-a-string) |
| 10  | [How to compare strings and check palindrome?](#how-to-compare-strings-and-check-palindrome) |
| 11  | [How to find duplicates in strings?](#how-to-find-duplicates-in-strings) |
| 12  | [How to apply bitwise operations?](#how-to-apply-bitwise-operations) |
| 13  | [How to check if strings are anagram?](#how-to-check-if-strings-are-anagram) |
| 14  | [How to find permutation of strings?](#how-to-find-permutation-of-strings) |

### [Recursion](#recursion)


## Introduction to DSA

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

## Array Representations

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

## Array as ADT (Abstract Data Type)

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

### How to Get, Set, Find Min - Max?

#### 1. Get(index)
Retrieves the element at the specified index.

```cpp
int get(int index) {
    if (index >= 0 && index < 10) // Assuming array size is 10
        return arr[index];
    else
        return -1; // Error value for invalid index
}
```

#### 2. Set(index, value)
Modifies the element at the specified index.

```cpp
void set(int index, int value) {
    if (index >= 0 && index < 10) // Assuming array size is 10
        arr[index] = value;
}
```

#### 3. Min()
Finds the minimum value in the array.

**Time Complexity:** `O(n)`

```cpp
int getMin(){
    int min;
    for(int i = 0; i < 9; i++)
        if(arr[i] > arr[i + 1])
            min = arr[i];
    return min;
}
```

#### 4. Max()
Finds the maximum value in the array.

**Time Complexity:** `O(n)`

```cpp
int getMax(){
    int max = arr[0];
    for(int i = 1; i < 9; i++)
        if(arr[i] > max)
            max = arr[i];
    return max;
}
```

#### 5. Sum() + Average()
Calculates the sum and average of array elements.

**Time Complexity:** `O(n)`

```cpp
// Iterative
int getAverage(){
    int sum = 0;
    for(int i = 0; i < 10; i++)
        sum += arr[i];
    return (sum / 10);
}
```
```cpp
// Recursive
int getAverage(int arr[], int num){
    if(num < 0){
        return 0;
    } else {
        return getAverage(arr, num - 1) + arr[num];
    }
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to Reverse and Shift an Array?

There are two common methods to reverse an array:

#### 1️. Auxiliary Array Method
- Create a temporary array.
- Copy elements in reverse order.
- Copy back to the original array.
- **Time Complexity:** `O(2n)`

```cpp
class Arr {
  public:
    int arr1[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

    void reverse() {
        int arr2[10];

        for(int i = 9, j = 0; i >= 0; i--, j++)
            arr2[j] = arr1[i];

        for(int i = 0; i < 10; i++)
            arr1[i] = arr2[i];

        for(int i = 0; i < 10; i++)
            cout << arr1[i] << " ";
    }
};

int main() {
    Arr arr;
    arr.reverse();
}
```

#### 2. In-Place Swap Method
Swap elements from the start and end of the array.

- **Time Complexity:** `O(n)`

```cpp
#include <iostream>
using namespace std;

class Arr {
  public:
    int arr1[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

    void reverse() {
        for(int i = 0, j = 9; i < j; i++, j--) {
            int temp = arr1[j];
            arr1[j] = arr1[i];
            arr1[i] = temp;
        }

        for(int i = 0; i < 10; i++)
            cout << arr1[i] << " ";
    }
};

int main() {
    Arr arr;
    arr.reverse();
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Left Shift / Rotation?

Move elements one position **left**.

- The **first element** moves to the **last position**.
- Used in **image sliders** and **circular queues**.

- **Time Complexity:** `O(n)`

```cpp
#include <iostream>
using namespace std;

class Arr {
  public:
    int A[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

    void rotate() {
        int temp = A[0];
        for (int i = 0; i < 9; i++) {
            A[i] = A[i + 1];
        }
        A[9] = temp;

        for (int i = 0; i < 10; i++)
            cout << A[i] << " ";
    }
};

int main() {
    Arr A;
    A.rotate();
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Right Shift / Rotation?

Move elements one position **right**.

- The **last element** moves to the **first position**.

- **Time Complexity:** `O(n)`

```cpp
#include <iostream>
using namespace std;

class Arr {
  public:
    int A[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

    void rotate() {
        int temp = A[9];
        for (int i = 9; i > 0; i--) {
            A[i] = A[i - 1];
        }
        A[0] = temp;

        for (int i = 0; i < 10; i++)
            cout << A[i] << " ";
    }
};

int main() {
    Arr A;
    A.rotate();
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Insert into Sorted Array?

This function inserts a given value into a **sorted array** while maintaining its sorted order.

- **Time Complexity:** `O(n)`

```cpp
void insertIntoSorted(int value) {
    int i = length - 1;

    while (i >= 0 && A[i] > value) {
        A[i + 1] = A[i];
        i--;
    }

    A[i + 1] = value;
    length++;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Check if an Array is Sorted?

This function checks whether a given array is sorted in **ascending order**.

- **Time Complexity:** `O(n)`

```cpp
bool isSorted() {
    for (int i = 0; i < 9; i++) {
        if (A[i] > A[i + 1]) {
            return false;
        }
    }
    return true;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Arranging Negative Numbers on Left Side?

This function rearranges the array so that all **negative numbers** are placed on the **left side**, while the **non-negative numbers** remain on the right.

- **Time Complexity:** `O(n)`

```cpp
void adjust() {
    int i = 0, j = 9;
    while (i < j) {
        while (A[i] < 0) { i++; }
        while (A[j] >= 0) { j--; }
        if (i < j) {
            int temp = A[i];
            A[i] = A[j];
            A[j] = temp;
        }
    }
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Merge Arrays?

#### Merging Two Sorted Arrays
- Combines two **sorted arrays** into one sorted array.
- Uses a **two-pointer technique** to efficiently merge the arrays.

- **Time Complexity:** `O(n + m)`, where `n` and `m` are the lengths of the arrays.

```cpp
#include <iostream>
using namespace std;

class Array {
public:
    int A[5] = {1, 4, 7, 9, 10};
    int B[5] = {2, 3, 5, 6, 8};
    int C[10]; // Merged array
    int length = 10;

    void merge() {
        int i = 0, j = 0, k = 0;

        while (i < 5 && j < 5) {
            if (A[i] <= B[j]) {
                C[k++] = A[i++];
            } else {
                C[k++] = B[j++];
            }
        }

        while (i < 5) {
            C[k++] = A[i++];
        }

        while (j < 5) {
            C[k++] = B[j++];
        }
    }

    void print() {
        for (int i = 0; i < length; i++)
            cout << C[i] << " ";
        cout << endl;
    }
};

int main() {
    Array arr;
    arr.merge();
    arr.print();
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Set Operations (Union, Intersection, Difference)?

#### 1. Union of Two Arrays

##### Unsorted Arrays

- Copy all elements of the first array (A) into the result array (C).
- Iterate through the second array (B).
- If an element from B is not already present in C, add it.

- **Time Complexity:** O(m * n) (for checking duplicates)

```cpp
#include<iostream>
using namespace std;

class Array{
    public:
      int A[5] = {2, 4, 1, 5, 10};
      int B[5] = {3, 4, 1, 2, 9};
      int C[10];
      int length = 0;

      void UNION() {
          for(int i = 0; i < 5; i++)
              C[length++] = A[i];
          for(int i = 0; i < 5; i++){
              bool found = false;
              for(int j = 0; j < length; j++){
                  if(B[i] == C[j]){
                      found = true;
                      break;
                  }
              }
              if(!found)
                  C[length++] = B[i];
          }
      }

      void print(){
          for(int i = 0; i < length; i++)
              cout << C[i] << " ";
      }
};

int main()
{
    Array A;
    A.UNION();
    A.print();
}
```

##### Sorted Arrays

- Use two pointers i and j to traverse both arrays.
- Compare elements and add the smaller one to C.
- If they are equal, add one and move both pointers forward.
- Add remaining elements of either array.

- **Time Complexity:** O(m + n) (since both arrays are traversed once)

```cpp
#include<iostream>
using namespace std;
class Array{
  public:
    int A[5] = {1, 4, 7, 8, 10};
    int B[5] = {2, 4, 5, 7, 8};
    int C[10];
    int k = 0;

      void UNION() {
         int i = 0, j = 0;

         while(i < 5 && j < 5){
             if(A[i] < B[j]){
                 C[k++] = A[i++];
             }else if(A[i] > B[j]){
                 C[k++] = B[j++];
             }else{
                 C[k++] = A[i];
                 i++; j++;
             }
         }

         while(i < 5)
             C[k++] = A[i++];
         while(j < 5)
             C[k++] = B[j++];
      }

      void print(){
          for(int i = 0; i < k; i++)
              cout << C[i] << " ";
      }
};

int main()
{
    Array A;
    A.UNION();
    A.print();
}
```

#### 2. Intersection of Two Arrays

##### Unsorted Arrays

- Iterate through A and B, checking for common elements.
- Store them in C if found.

- **Time Complexity:** O(m * n) (brute force comparison)

```cpp
void INTERSECTION(){
    for(int i = 0; i < 5; i++){
        for(int j = 0; j < 5; j++){
            if(A[i] == B[j]){
                C[k++] = A[i];
            }
        }
    }
}
```

##### Sorted Arrays

- Use two pointers i and j.
- If A[i] == B[j], store in C.
- Otherwise, increment the smaller pointer.

- **Time Complexity:** O(m + n)

```cpp
void INTERSECTION(){
    int i = 0, j = 0;
    while(i < 5 && j < 5){
        if(A[i] < B[j]){
            i++;
        }else if(A[i] > B[j]){
            j++;
        }else{
            C[k++] = A[i++];
            j++;
        }
    }
}
```

#### 3. Difference of Two Arrays

##### Unsorted Arrays

- Iterate through A, checking if each element exists in B.
- If not, add to C.

**Time Complexity:** O(m * n) (brute force search)

```cpp
void DIFFERENCE(){
    for(int i = 0; i < 5; i++){
        bool isFound = false;
        for(int j = 0; j < 5; j++){
            if(A[i] == B[j]){
                isFound = true;
                break;
            }
        }
        if(!isFound){
            C[k++] = A[i];
        }
    }
}
```

##### Sorted Arrays

- Use two pointers i and j.
- If A[i] is smaller, add it to C.
- If equal, skip both.
- Append remaining elements of A.

- **Time Complexity:** O(m + n)

```cpp
void DIFFERENCE(){
    int i = 0, j = 0;

    while(i < 5 && j < 5){
        if(A[i] < B[j]){
            C[k++] = A[i++];
        }else if(A[i] > B[j]){
            j++;
        }else{
            i++;
            j++;
        }
    }

    while(i < 5)
        C[k++] = A[i++];
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Find Missing Element (Single Missing, Multiple Missing)?

#### 1. Single Missing Element from Natural Numbers (Sorted Array)

- **From 1 to n (First n Natural Numbers):**

```cpp
void Array::missingElement(){
    int sum = 10 * (10 + 1) / 2;
    int s;
    for(int i = 0; i < 10; i++)
        s += A[i];

    cout << "Missing element is: " << (sum - s);
};
```

- **From k to n:**

```cpp
void Array::missingElement(){
    int diff = A[0] - 0;

    for(int i = 0; i < 10; i++){
        if(A[i] - i != diff){
            cout << "Missing element is: " << (diff + i) << endl;
            break;
        }
    }
};
// Add index + difference
```

#### 2. Multiple Missing Elements from Unsorted Array

- This procedure uses a hash table / bit set, which operates in constant time.
- When searching for missing elements, a hash table is a preferred choice if feasible.
- When using this technique, the required space should be equal to the maximum value of the array. If space is constrained, this approach may not be suitable.

```cpp
void Array::missingElements(){
    int B[14]; // Maximum element of array
    for(int i = 0; i < 14; i++)
        B[A[i]] = 1;
    for(int i = 0; i < 14; i++)
        if(B[i] == 0)
           cout << "Missing element: " << i << endl;
}
```


**[⬆ Back to Top](#table-of-contents)**

---

### Find Duplicate Elements?

#### 1. Finding Duplicates in a Sorted Array
- If an element appears **more than once**, it should be printed **only once**.

```cpp
void duplicateElements(){
    int lastDuplicate = 0;
    for(int i = 0; i < 10 - 1; i++){
        if(A[i] == A[i + 1] && lastDuplicate != A[i]){
            cout << "Duplicate element: " << A[i] << endl;
            lastDuplicate = A[i];
        }
    }
}
```

#### 2. Counting Duplicates in a Sorted Array
- Counts how many times each element appears in a sorted array.

```cpp
void countDuplicates(){
    for(int i = 0; i < 10 - 1; i++){
        if(A[i] == A[i + 1]){
            int j = i + 1;
            while(A[j] == A[i]) j++;
            cout << A[i] << " appears " << j - i << " times." << endl;
            i = j - 1;
        }
    }
}
```

#### 3. Counting Duplicates Using a Hash Table (Sorted Array)

```cpp
void countDuplicates(){
    for(int i = 0; i < 10 - 1; i++){
        if(A[i] == A[i + 1]){
            int j = i + 1;
            while(A[j] == A[i]) j++;
            cout << A[i] << " " << j - i << endl;
            i = j - 1;
        }
    }
}
```

#### 4. Finding Duplicates in an Unsorted Array
- Uses brute force method, setting duplicate values to -1.

```cpp
void findDuplicateUnsort(){
    for(int i = 0; i < 10 - 1; i++){
        int count = 1;
        if(A[i] != -1){
            for(int j = i + 1; j < 10; j++){
                if(A[i] == A[j]){
                    count++;
                    A[j] = -1;
                }
            }
            if(count > 1){
                cout << "Duplicate element " << A[i] << " appears " << count << " times." << endl;
            }
        }
    }
}
```

#### 5. Finding Duplicates Using a Hash Table (Unsorted Array)

```cpp
void findDuplicateUnsort(){
    int B[10] = {0};
    for(int i = 0; i < 10; i++)
        B[A[i]]++;
    for(int i = 0; i < 10; i++)
        if(B[i] > 1)
            cout << "Duplicate element " << i << " appears " << B[i] << " times." << endl;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Finding a Pair with Sum K?

#### 1. Finding a Pair of Elements with Sum K (Sorted Array)
This approach uses the **two-pointer technique** to find a pair whose sum equals `k`.
- If the sum is equal to `k`, the pair is printed.
- If the sum is less than `k`, increment `i` (move right).
- If the sum is greater than `k`, decrement `j` (move left).

- **Time Complexity:** `O(n)`

```cpp
void Array::findPair(int k){
    int i = 0, j = 10 - 1;
    while (i < j) {
        if(A[i] + A[j] == k){
            cout << "Pair found: " << A[i] << " and " << A[j] << endl;
            i++; j--;
        } else if(A[i] + A[j] < k){
            i++;
        } else {
            j--;
        }
    }
}
```

#### 2. Finding a Pair of Elements with Sum K (Unsorted Array)
This approach **checks all possible pairs** in a nested loop to find the sum `k`.
- It iterates through the array, comparing each element with every other element.
- If a pair with sum `k` is found, it is printed.

- **Time Complexity:** `O(n²)`

```cpp
void Array::findPair(int k){
    for(int i = 0; i < 10 - 1; i++){
        for(int j = i + 1; j < 10; j++){
            if(A[i] + A[j] == k){
                cout << "Pair found: " << A[i] << " and " << A[j] << endl;
            }
        }
    }
}
```

#### 3. Finding a Pair of Elements with Sum K (Using Hash Table)
This approach **uses an auxiliary array (hash table)** to store values and find the sum efficiently.

#### How It Works:
- It iterates through the array, checking if `k - A[i]` exists in the hash table.
- If found, it prints the pair.
- Otherwise, it marks `A[i]` as visited in the hash table.

- **Time Complexity:** `O(n)`

```cpp
void Array::findPair(int k){
    int B[10] = {0};

    for(int i = 0; i < 10; i++){
        if(B[k - A[i]] != 0)
            cout << "Pair found: " << A[i] << " and " << k - A[i] << endl;
        B[A[i]]++;
    }
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Reverse an Array?

Reversing an array can be done in different segments:

#### 1. Reverse `[1, k]`
This function reverses the elements from index `1` to `k` (0-based indexing).

```cpp
void reverseOneToK(int k){
    for(int i = 0, j = k - 1; i < k / 2; i++, j--){
        int c = A[i];
        A[i] = A[j];
        A[j] = c;
    }
}
```

#### 2. Reverse `[k + 1, n]`
This function reverses elements from index `k + 1` to `n`, which means reversing the latter part of the array.

```cpp
void reverseFromKPlusOne(int k) {
  for (int i = k + 1, j = size - 1; i < j; i++, j--) {
      int temp = A[i];
      A[i] = A[j];
      A[j] = temp;
  }
}
```

#### 3. Reverse `[1, n]`
This function reverses the entire array.

```cpp
void reverseOneToN(){
    for(int i = 0, j = 10 - 1; i < j; i++, j--){
        int c = A[i];
        A[i] = A[j];
        A[j] = c;
    }
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Find Two Elements with Difference Equal to S in a Sorted Array?

```Array in increasing order, we want to find two elements having difference equal to (s)```

- Works for sorted arrays.
- Uses two pointers (`i` and `j`).
- If difference equals `s`, prints the pair.
- If difference is less than `s`, moves `j` forward.
- If difference is greater than `s`, moves `i` forward.

#### Time Complexity: `O(n)`

```cpp
void findDifference(int s) {
    int i = 0, j = 1;
    while (j < 10) {
        if ((A[j] - A[i]) == s) {
            cout << "Difference found with: " << A[j] << " - " << A[i] << endl;
            i++;
            j++;
        } else if ((A[j] - A[i]) < s) {
            j++;
        } else {
            i++;
        }
    }
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Finding Minimum and Maximum in a Single Scan?

```cpp
void minAndMax(){
    int min = A[0], max = A[0];

    for(int i = 1; i < 10; i++){
        if(A[i] < min)
            min = A[i];
        else if(A[i] > max)
            max = A[i];
    }

    cout << "Minimum: " << min << ", Maximum: " << max << endl;
}
```

- **Best Case:** When array is in descending order (1 comparison per iteration).
- **Worst Case:** When min and max are at opposite ends.

**[⬆ Back to Top](#table-of-contents)**

---

### Find Array Elements that are Neither Minimum nor Maximum?

#### 1. Simple Conditional Check
```cpp
void findNum() {
   if(A[0] > A[1] && A[0] < A[2])
       cout << "Number: " << A[0];
   else if(A[1] > A[0] && A[1] < A[2])
       cout << "Number: " << A[1];
   else
       cout << "Number: " << A[2];
}
```

#### 2. Generalized Approach for Larger Arrays

```cpp
void findMiddleElements(int A[], int n) {
    int minVal = INT_MAX, maxVal = INT_MIN;

    // Finding minimum and maximum values
    for(int i = 0; i < n; i++) {
        if(A[i] < minVal) minVal = A[i];
        if(A[i] > maxVal) maxVal = A[i];
    }

    cout << "Elements neither minimum nor maximum: ";
    for(int i = 0; i < n; i++) {
        if(A[i] != minVal && A[i] != maxVal)
            cout << A[i] << " ";
    }
    cout << endl;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Find 2nd Maximum or Minimum Element?

```cpp
// Maximum
void secondMaximum(){
    int first = INT_MIN, second = INT_MIN;
    for(int i = 0; i < 10; i++){
        if(A[i] > first){
            second = first;
            first = A[i];
        } else if(A[i] > second && A[i] != first){
            second = A[i];
        }
    }
    cout << "Second maximum value: " << second << endl;
}```

```cpp
// Minimum
void secondMinimum(){
    int first = INT_MAX, second = INT_MAX;
    for(int i = 0; i < 10; i++){
        if(A[i] < first){
            second = first;
            first = A[i];
        } else if(A[i] < second && A[i] != first){
            second = A[i];
        }
    }
    cout << "Second minimum value: " << second << endl;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Find Elements in Range (0-100) with Frequency > 50

- Given an array of elements within the range **0 to 100**, find the **frequency of elements greater than 50** and display the count of each occurrence.

#### Approach
- We initialize an array `temp[50]` to store the frequency of numbers **greater than 50** (i.e., numbers between **51 to 100**).
- We read `n` elements from user input.
- If the number is **greater than 50**, we increment its respective index in `temp[]`.
- Finally, we display the numbers and their corresponding frequency.

```cpp
#include <iostream>
using namespace std;

class Array {
public:
    int temp[50] = {0}; // Frequency array for numbers 51-100

    void elementsCounting() {
        for (int i = 0; i < 10; i++) { // Modify 10 based on input size
            int element;
            cin >> element;

            if (element > 50 && element <= 100)
                temp[element - 51]++; // Map 51-100 to 0-49 index
        }
    }

    void display() {
        for (int i = 0; i < 50; i++) {
            if (temp[i] != 0)
                cout << (i + 51) << " appears " << temp[i] << " times" << endl;
        }
    }
};

int main() {
    Array A;
    A.elementsCounting();
    A.display();
}
```

**[⬆ Back to Top](#table-of-contents)**

---
---
---

## Strings

### Character Set

- A character set is the set of characters that are supported by a programming language.
- Computers do not directly understand characters, so numeric codes are assigned to characters.
- These numeric codes are standardized globally, known as ASCII and Unicode.
- Standardized by `American National Standards Institute (ANSI)` and `ISO`.

**[⬆ Back to Top](#table-of-contents)**

---

### ASCII

- Total ASCII codes: `128` (0-127)
- `A-Z` ASCII codes: `65-90`
- `a-z` ASCII codes: `97-122`
- `0-9` ASCII codes: `48-57`
- Special characters: `Enter = 10`, `Space = 13`, `Esc = 27`
- Each symbol/character takes `7 bits` or `1 byte`

**[⬆ Back to Top](#table-of-contents)**

---

### Unicode

- Supports all languages worldwide.
- Uses `16 bits` or `2 bytes`.
- Represented in hexadecimal format.

### Character array
- `char A[5];`
- `char A[5] = {65, 66, 67, 68, 69};`
- `char A[5] = {'A', 'B', 'C', 'D', 'E'}`

**[⬆ Back to Top](#table-of-contents)**

---

### Difference Between Character Set and Strings
- A **character set** is a collection of characters assigned with unique numeric codes.
- A **string** is a sequence of characters that ends with a null character (`\0`).

```cpp
#include <iostream>
using namespace std;

int main() {
    char charSet[] = {65, 66, 67, 68, 69}; // Character Set (ASCII values for A-E)
    char str[] = "ABCDE"; // String with \0 at the end

    cout << "Character Set: ";
    for (char c : charSet) {
        cout << c << " ";
    }
    cout << "\nString: " << str << endl;
    return 0;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### Strings
- A string is a sequence of characters terminated by a special character `\0` (null character).
- The `\0` character acts as a string delimiter.

  ```cpp
  char A[6] = "Hello"; // Automatically adds '\0' at the end
  ```
- Without `\0`, a character array remains just an array of characters, not a string.

**[⬆ Back to Top](#table-of-contents)**

---

### How to find Length of string?

- We cannot calculate the size of a string using `array - 1` because the string may have fewer elements than the total allocated size.
- In C and C++, when you initialize a character array with a string literal like "ABDUL AHAD", the compiler automatically appends a null terminator ('\0') at the end of the string.
  - So, when you declare `char A[] = "ABDUL AHAD";`, the memory layout looks like this:
    - | 'A' | 'B' | 'D' | 'U' | 'L' | 'A' | ' ' | 'H' | 'A' | 'D' | '\0' |

```cpp
char A[] = "ABDUL AHAD";
cout << A << endl;
char B[5] = {'A', 'B', 'C', 'D', '\0'};
cout << B << endl;
char C[] = {'A', 'B', 'C', 'D', '\0'};
cout << C << endl;
int length = 0;
for(int i = 0; A[i] != '\0'; i++)
    length++;
cout << "Length of A: " << length;
```

#### Another approach using a function:

```cpp
int length(char str[]) {
    int i = 0;
    while (str[i] != '\0') {
        i++;
    }
    return i;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to change case of strings?

Changing the case of a string means converting **uppercase letters to lowercase** and **lowercase letters to uppercase**.
- In **ASCII**, uppercase letters ('A' to 'Z') range from **65 to 90**.
- Lowercase letters ('a' to 'z') range from **97 to 122**.
- The difference between uppercase and lowercase letters is **32** (`'A' + 32 = 'a'` and `'a' - 32 = 'A'`).

#### Convert Uppercase to Lowercase

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "ABDUL AHAD";

    // Convert to lowercase
    for (int i = 0; A[i] != '\0'; i++) {
        A[i] = char(A[i] + 32);
    }

    cout << A << endl; // Output: abdul ahad

    // Convert the first letter back to uppercase
    A[0] = char(A[0] - 32);

    cout << A; // Output: Abdul ahad
}
```

#### Convert Lowercase to Uppercase and Vice Versa

- This program swaps the case of each character.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "ABDUL AHAD";

    // Toggle case (uppercase → lowercase, lowercase → uppercase)
    for (int i = 0; A[i] != '\0'; i++) {
        if (A[i] >= 97 && A[i] <= 122) // If lowercase
            A[i] -= 32;
        else if (A[i] >= 65 && A[i] <= 90) // If uppercase
            A[i] += 32;
    }

    char B[] = "cHiLli";

    for (int i = 0; B[i] != '\0'; i++) {
        if (B[i] >= 'a' && B[i] <= 'z') // If lowercase
            B[i] -= 32;
        else if (B[i] >= 'A' && B[i] <= 'Z') // If uppercase
            B[i] += 32;
    }

    cout << A << " " << B;
    // Output: abdul ahad ChIlLI
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to count words, vowels and consonants in a string?

This program calculates:
1. **Word Count**: A word is identified when a space is followed by a non-space character.
2. **Vowel Count**: Characters `a, e, i, o, u` (both uppercase and lowercase).
3. **Consonant Count**: Any letter that is not a vowel.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "We are all Palestinian";
    int wordCount = 0, vowelCount = 0, consonantCount = 0;

    for (int i = 0; A[i] != '\0'; i++) {
        // Counting words (checking spaces between words)
        if (A[i] == ' ' && A[i - 1] != ' ')
            wordCount++;

        // Counting vowels
        if (A[i] == 'a' || A[i] == 'e' || A[i] == 'i' || A[i] == 'o' || A[i] == 'u' ||
            A[i] == 'A' || A[i] == 'E' || A[i] == 'I' || A[i] == 'O' || A[i] == 'U') {
            vowelCount++;
        }
        // Counting consonants (any alphabet that is not a vowel)
        else if ((A[i] >= 65 && A[i] <= 90) || (A[i] >= 97 && A[i] <= 122)) {
            consonantCount++;
        }
    }

    cout << "Total words: " << wordCount + 1 << " ,Vowels: " << vowelCount << " ,Consonants: " << consonantCount;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to validate a string?

This program checks whether a given string is **valid** by ensuring it contains only:
1. **Digits (0-9)**
2. **Uppercase letters (A-Z)**
3. **Lowercase letters (a-z)**

- If the string contains any special characters (e.g., `@, *, #, !`), it is considered **invalid**.

```cpp
#include <iostream>
using namespace std;

int validate(char A[]) {
    for (int i = 0; A[i] != '\0'; i++) {
        // Checking if the character is NOT a digit, uppercase letter, or lowercase letter
        if (!(A[i] >= 48 && A[i] <= 57) && !(A[i] >= 65 && A[i] <= 90) && !(A[i] >= 97 && A[i] <= 122))
            return 0; // Invalid string
    }
    return 1; // Valid string
}

int main() {
    char A[] = "ABDULAHAD786*ali";  // String to validate
    if (validate(A))
        cout << "Valid string!";
    else
        cout << "Not a valid string!";
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to Reverse a String?

Reversing a string means rearranging its characters in the opposite order. We can achieve this using:
1. **Extra Array Method**: Storing the reversed string in a separate array.
2. **Swapping Method**: Swapping characters in the same array.

#### **Method 1: Using an Extra Array**
- First, find the **length** of the string.
- Then, store characters in reverse order in a new array.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "CHILLI";
    int i;

    // Finding string length
    for(i = 0; A[i] != '\0'; i++) {};

    char B[i];  // Creating new array to store reversed string
    i = i - 1;  // Adjusting index to last character

    // Storing characters in reverse order
    for(int j = 0; i >= 0; i--, j++)
        B[j] = A[i];

    cout << "Reversed string: " << B;
}
```

#### **Method 2: Swapping in the Same Array**
- Using two pointers: One at the start, another at the end.
- Swap characters until pointers meet in the middle.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "CHILLI";
    int i, j;

    // Finding string length
    for(j = 0; A[j] != '\0'; j++) {};
    j--;  // Move to last character

    // Swapping characters
    for(i = 0; i < j; i++, j--) {
        char c = A[i];
        A[i] = A[j];
        A[j] = c;
    }

    cout << "Reversed string: " << A;
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to compare strings and check palindrome?

#### **1. Comparing Strings**
String comparison determines which string is lexicographically larger, smaller, or equal.

- Iterate through both strings **character by character**.
- Stop at the first mismatched character.
- Compare their ASCII values:
  - If `A[i] > B[j]`, `A` is larger.
  - If `A[i] < B[j]`, `A` is smaller.
  - If all characters match, the strings are equal.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "APPLE";
    char B[] = "BANANA";
    int i, j;

    // Compare characters one by one
    for(i = 0, j = 0; A[i] != '\0' && B[j] != '\0'; i++, j++)
        if(A[i] != B[j])
            break;

    if(A[i] > B[j])
        cout << "A is larger";
    else if(A[i] < B[j])
        cout << "A is smaller";
    else
        cout << "Both strings are equal!";
}
```

#### **Checking if a String is a Palindrome**

A **palindrome** is a string that reads the same **forward and backward**.
For example:
- **"MADAM"**, **"RACECAR"** are palindromes.
- **"HELLO"**, **"WORLD"** are not palindromes.

1. **Reverse** the string and store it in another array.
2. **Compare** the original and reversed strings **character by character**.
3. If all characters match, **it's a palindrome**.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "MADAM";
    int i;

    // Step 1: Find string length
    for(i = 0; A[i] != '\0'; i++) {}

    char B[i + 1];  // Extra space for null terminator
    B[i] = '\0';  // End reversed string with null character

    // Step 2: Store reversed string
    for(int j = 0; i > 0; i--, j++) {
        B[j] = A[i - 1];
    }

    // Step 3: Compare original and reversed strings
    for(i = 0; A[i] != '\0'; i++) {
        if(A[i] != B[i]) {
            cout << "Not a palindrome\n";
            return 0;
        }
    }

    cout << "Palindrome\n";
}
```

#### **3. Alternative: Two-Pointer Palindrome Check**

- A more efficient approach is to use two pointers, one at the start and one at the end, and compare characters.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "MADAM";
    int i, j;

    // Find string length
    for(j = 0; A[j] != '\0'; j++) {};
    j--;  // Adjust for index

    // Compare first and last characters
    for(i = 0; i < j; i++, j--) {
        if(A[i] != A[j]) {
            cout << "Not a palindrome\n";
            return 0;
        }
    }

    cout << "Palindrome\n";
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to find duplicates in strings?

  Finding duplicate characters in a string helps in **text processing, compression, and data validation**.

#### **Methods to Find Duplicates**
1. **Using Nested Loops** (Brute Force) → **O(n²) Time Complexity**
2. **Using Hash Tables** (Efficient for lowercase letters) → **O(n) Time Complexity**


#### **1. Brute Force Approach (Nested Loops)**

- Compare each character with all previous characters.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "Finding";

    for(int i = 0; A[i] != '\0'; i++) {
        for(int j = 0; j < i; j++) {
            if(A[i] == A[j]) {
                cout << "Duplicate element: " << A[i] << endl;
                break; // Stop checking once a duplicate is found
            }
        }
    }
}
```

#### **2. Efficient Approach Using Hash Tables**

1. Create an **array of size 26** (for lowercase letters).
2. Traverse the string and count occurrences of each character.
3. Print characters that appear **more than once**.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "finding"; // Lowercase string
    int B[26] = {0};  // Hash table initialized with 0

    // Count character occurrences
    for(int i = 0; A[i] != '\0'; i++) {
        B[A[i] - 'a']++;
    }

    // Display duplicates
    for(int i = 0; i < 26; i++) {
        if(B[i] > 1) {
            cout << char(i + 'a') << " appears " << B[i] << " times." << endl;
        }
    }
}
```

#### **3. Optimized Approach: Using Bit Manipulation**

- **Faster** than other methods.
- **Lower memory usage** (only a single integer).
- Works **only for lowercase letters (a-z)**.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "finding";
    int checker = 0, x = 0;

    for(int i = 0; A[i] != '\0'; i++) {
        x = 1 << (A[i] - 'a');  // Create a bitmask

        if((checker & x) > 0) // Check if character already exists
            cout << "Duplicate element: " << A[i] << endl;
        else
            checker = checker | x;  // Mark character as seen
    }
}
```


**[⬆ Back to Top](#table-of-contents)**

---

### How to apply bitwise operations?

#### **Why Use Bitwise Operations?**

Bitwise operations allow efficient manipulation of binary data. They are widely used in:
- **Strings:** Checking for duplicate characters, toggling cases, etc.
- **Integers:** Performing arithmetic and logical operations efficiently.


#### **Types of Bitwise Operations**
##### **1️. Left Shift (`<<`)**
- Shifts bits **to the left** by a specified number of positions.
- Fills the empty right positions with `0`s.
- Effectively **multiplies** the number by `2^n`.

```cpp
int x = 5;      // 0000 0101
int y = x << 1; // 0000 1010  (5 * 2 = 10)
```

##### **2. Bitwise AND (`&`) - Masking**
- Used to check whether a specific bit is set (ON) or not.
- If a bit is `1` in both operands, the result is `1`; otherwise, `0`.

```cpp
int x = 5;      // 0000 0101
int y = 1;      // 0000 0001
int result = x & y; // 0000 0001 (1)
```

- **Use Case:** Checking if a character has already appeared in a string.

##### **3️. Bitwise OR (`|`) - Merging**
- Used to set (turn ON) a bit at a specific position.
- If a bit is `1` in either operand, the result is `1`.

```cpp
int x = 5;      // 0000 0101
int y = 2;      // 0000 0010
int result = x | y; // 0000 0111 (7)
```

- **Use Case:** Marking a character as "seen" in a string.

##### **4. Finding Duplicate Characters in a String**
This method uses bitwise operations to detect duplicate characters efficiently.

- Use a long integer (`H`) as a bit container.
- Left shift (`<<`) to mark characters as seen.
- Use AND (`&`) to check if a character was already marked.
- Use OR (`|`) to mark new characters as seen.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "Finding";
    long int H = 0, x = 0;

    for(int i = 0; A[i] != '\0'; i++) {
        x = 1;
        x = x << (A[i] - 'a');  // Left shift based on character position

        if((x & H) > 0)  // Check if character is already seen
            cout << A[i] << " is a duplicate element!" << endl;
        else
            H = x | H;  // Mark character as seen
    }
}
```

**[⬆ Back to Top](#table-of-contents)**

---

### How to check if strings are anagram?

An anagram is a word or phrase formed by rearranging the letters of a different word or phrase. In this approach, we check whether all the elements from string 1 are present in string 2.

- First, check if the sizes of both strings are equal. If not, they are not anagrams.
- Use an array of size 26 (for lowercase letters) to count occurrences of each character in the first string.
- Traverse the second string and decrement the character count in the array.
- If any value in the array becomes negative, the strings are not anagrams.
- If all values are zero at the end, the strings are anagrams.

```cpp
#include <iostream>
using namespace std;

int main() {
    char A[] = "finding";
    char B[] = "dingfin";

    int i, C[26] = {0};
    bool isAnagram = true;

    // Count character occurrences in A
    for(i = 0; A[i] != '\0'; i++)
        C[A[i] - 'a'] += 1;

    // Compare with B
    for(i = 0; B[i] != '\0'; i++) {
        C[B[i] - 'a'] -= 1;
        if(C[B[i] - 'a'] < 0) {
            isAnagram = false;
            cout << "Not Anagram" << endl;
            break;
        }
    }

    if(isAnagram && B[i] == '\0')
        cout << "Anagram" << endl;
}
```

#### Complexity Analysis
| Method | Time Complexity | Space Complexity |
|--------|----------------|------------------|
| Nested Loops | O(n²) | O(1) |
| Hash Table | O(n) | O(1) |

**Recommended Approach:** Using hash tables provides better performance compared to the nested loop method.

**[⬆ Back to Top](#table-of-contents)**

---

### How to Find Permutation of Strings?

- **Arrangement of a string.**

- For `ABC`:
  - Possible permutations: `ABC, ACB, BAC, BCA, CAB, CBA`
  - Since there are `3` characters, the number of arrangements is `3!`.
  - For `n` characters, the arrangement is `n!`.
- **State Space Tree**: Imagine a tree where each branch represents a possible state of a problem, and the leaves show the results.
- **Backtracking**: Going back and trying another path in the tree to explore different possibilities.


- **Brute Force**: Trying every possible combination to find a solution.
- **Recursion**: Using a procedure within itself to explore different paths, often used for backtracking.
- **Dynamic Programming**: It's like a smarter brute force. It also tries different combinations but aims to find the best solution efficiently.

- Use recursion to achieve backtracking.
- With backtracking, we perform brute force.
- Traverse in each call and pick characters that are not yet selected.
- At the leaf node, prepare a string and display it.

#### Method 1: Using Recursion with a Helper Array
```cpp
#include <iostream>
using namespace std;

void perm(char s[], int k){
    static char res[10];
    static int A[10] = {0};
    if(s[k] == '\0'){
        res[k] = '\0';
        cout << res << " ";
    }else{
        for(int i = 0; s[i] != '\0'; i++){
            if(A[i] == 0){
                res[i] = s[k];
                A[i] = 1;
                perm(s, k + 1);
                A[i] = 0;
            }
        }
    }
}

int main()
{
   char p[] = "ABC";
   perm(p, 0);
}
```

#### Method 2: Using Swapping
```cpp
#include <iostream>
using namespace std;

void swap(char &x, char &y){
    char z = x;
    x = y;
    y = z;
}

void perm(char p[], int l, int h){
    if(l == h){
        cout << p << " ";
    }else{
        for(int i = l; i <= h; i++) {
            swap(p[l], p[i]);
            perm(p, l + 1, h);
            swap(p[l], p[i]);
        }
    }
}

int main()
{
   char p[] = "ABC";
   perm(p, 0, 2);
}
```

**[⬆ Back to Top](#table-of-contents)**

---
---
---

## Recursion
