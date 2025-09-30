

-----

# Data Structures

Data structure is a particular way of storing and organizing data in a computer so that it can be used efficiently. A data structure is a special format for organizing and storing data. General data structure types include arrays, files, linked lists, stacks, queues, trees, graphs and so on.

### **Data Structures** are classified into two types:

1)  **Linear data structures**: Elements are accessed in a sequential order but it is not compulsory to store all elements sequentially. Examples: Linked Lists, Stacks and Queues.
2)  **Non-linear data structures**: Elements of this data structure are stored/accessed in a non-linear order. Examples: Trees and graphs

-----

# Array

An **Array** is a fundamental data structure that stores a collection of items, typically of the same data type, in contiguous memory locations. Think of it as a set of numbered boxes all placed in a line.

### Characteristics
 1) **Homogeneous** → Stores elements of the same type.

 2) **Fixed Size** → Size defined at creation, cannot change.

 3) **Indexed Access** → Elements accessed by index (0-based).

 4) **Static Memory** → Memory allocated at compile-time.

### Example

```c
int arr[4] = {10, 20, 30, 40};
```

### Time Complexity

| Operation | Complexity | Description |
| :---: | :---: | :--- |
| **Access**  | $O(1)$ | Instant, as the address is calculated directly using the index. |
| **Search**  | $O(n)$ | Must check, on average, half the elements. |
| **Insertion/Deletion** | $O(n)$ | Requires shifting potentially all subsequent elements to maintain sequence. |

### Space Complexity
 * O(n) where n is the number of elements.
 * Some overhead for fixed size (may allocate extra unused space).
-----

# Linked Lists

A **linked list** is a data structure used for storing collections of data. A linked list has the following properties:

### Characteristics

  A **linked list** is a data structure used for storing collections of data. A linked list has the following properties:

  1) Successive elements are connected by **pointers**.
  2) The last element points to **NULL**.
  3) Can **grow or shrink in size** during execution of a program.
  4) Can be made just as long as required (until system memory exhausts).
  5) Does not waste memory space (but takes some extra memory for pointers). It allocates memory as list grows.

### Singly Linked List Example
    [Head] -> [4 | next] -> [15 | next] -> [7 | next] -> [40 | NULL]

### Types of Linked List
   1) **Singly Linked List** → Each node contains data + next pointer. Last node points to NULL.
   2) **Doubly Linked List** → Each node contains data + next + previous pointers, allowing two-way traversal.
   3) **Circular Linked List** → Last node points back to the first node. Can be singly or doubly circular.
### Time Complexity

| Operation | Complexity | Description |
| :---: | :---: | :--- |
| **Access**  | $O(n)$ | Requires sequential traversal from the start. |
| **Search** | $O(n)$ | Must traverse the list until the element is found. |
| **Insertion/Deletion** | $O(1)$ | Requires only updating the pointers of the surrounding nodes (assuming the node's location is known). |
### Space Complexity
 * O(n) for n nodes.
 * Extra space overhead per node for storing pointers (e.g., 1 pointer in singly linked, 2 in doubly linked).

-----

# Linked List vs. Array 
|  No.  | Linked List                               | Array                                       |
| :---: | :---------------------------------------- | :------------------------------------------ |
| **1** | Made of **nodes** (data + link).          | Made of **elements** at index.              |
| **2** | Access by **going step by step**.         | Access directly with **index**.             |
| **3** | Can **remove node fully**.                | Delete means **overwrite/shift**.           |
| **4** | **Insert/Delete** is easy (change links). | **Insert/Delete** is slow (shift elements). |
| **5** | Uses **dynamic memory** (no wastage).     | Uses **fixed memory** (wastage possible).   |


-----

# Time & Space Complexity

### Time Complexity Notations


Time complexity tells you **how fast an algorithm runs** as the input size ($n$) grows.

| Notation | Meaning | Scenario |
| :---: | :--- | :--- |
| $\mathbf{\Omega}$ | **Lower bound** (best-case time) | Minimum time required. |
| $\mathbf{\Theta}$ | **Tight bound** (average-case time) | Typical performance time. |
| $\mathbf{O}$ | **Upper bound** (worst-case time) | Maximum time required. |

### Space Complexity

Space complexity tells you **how much memory** an algorithm uses relative to the input size ($n$).

| Structure | Space Usage | Explanation |
| :---: | :--- | :--- |
| **Array** | $O(n)$ | Stores $n$ elements, requiring linear space. |
| **Linked List** | $O(n)$ | Stores $n$ nodes, where each node has data + a pointer. |
| **Example** | $O(1)$ Extra Space | $O(1)$ means the algorithm uses a fixed amount of extra memory (like a few variables), regardless of how large the input ($n$) is. |

***



