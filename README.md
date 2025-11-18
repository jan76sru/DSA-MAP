# 🧠 DSA MAP — Reference Guide

A quick guide to common **Data Structures**, their **operations**, **time complexities**, and **use-cases**.

---

## 📘 1. Basic Data Types

| Type | Description | Example | Use Case |
|------|--------------|----------|-----------|
| `int` | Integer number | `5, -10, 42` | Counting, indexing |
| `float / double` | Decimal number | `3.14, -2.7` | Precision math, geometry |
| `char` | Single character | `'a', 'Z'` | Strings, alphabets |
| `string` | Sequence of chars | `"hello"` | Text data |
| `bool` | True / False | `true, false` | Conditions, logic |

---

## 🧩 2. Arrays / Lists

| Operation | Time Complexity | Description |
|------------|----------------|--------------|
| Access by index | <span style="color:limegreen;">O(1)</span> | Direct access |
| Insert at end | <span style="color:limegreen;">O(1)</span> (amortized) | Push back |
| Insert/delete at middle | <span style="color:orange;">O(n)</span> | Shift elements |
| Search (unsorted) | <span style="color:orange;">O(n)</span> | Linear search |
| Search (sorted + binary) | <span style="color:deepskyblue;">O(log n)</span> | Binary search |

**Use Cases:**  
- Static or predictable-size collections  
- Problems with **index-based access**, e.g. *Two Sum, Max Subarray, Sliding Window*  

---

## 🪣 3. Linked List

| Operation | Time Complexity | Description |
|------------|----------------|--------------|
| Access by index | <span style="color:orange;">O(n)</span> | Sequential traversal |
| Insert/Delete at head | <span style="color:limegreen;">O(1)</span> | Constant time |
| Insert/Delete in middle | <span style="color:orange;">O(n)</span> | Traverse first |
| Search | <span style="color:orange;">O(n)</span> | Sequential search |

**Use Cases:**  
- Dynamic memory usage  
- Implementing **Stacks, Queues, Hash Chaining**  
- Problems involving **pointers / nodes**

---

## 🧱 4. Stack

| Operation | Time Complexity | Description |
|------------|----------------|--------------|
| Push | <span style="color:limegreen;">O(1)</span> | Add top |
| Pop | <span style="color:limegreen;">O(1)</span> | Remove top |
| Peek | <span style="color:limegreen;">O(1)</span> | Read top |
| Search | <span style="color:orange;">O(n)</span> | Sequential search |

**Use Cases:**  
- **LIFO** (Last In, First Out)  
- **Expression Evaluation**, **Backtracking**, **DFS traversal**, **Undo/Redo**  

---

## 🧭 5. Queue / Deque

| Operation | Time Complexity | Description |
|------------|----------------|--------------|
| Enqueue | <span style="color:limegreen;">O(1)</span> | Add to rear |
| Dequeue | <span style="color:limegreen;">O(1)</span> | Remove from front |
| Peek | <span style="color:limegreen;">O(1)</span> | Read front |
| Search | <span style="color:orange;">O(n)</span> | Sequential search |

**Use Cases:**  
- **FIFO** (First In, First Out)  
- **BFS**, **Scheduling**, **Sliding Window Maximum**, **Producer-Consumer**  

---

## 🌳 6. Tree

| Operation | Time Complexity | Description |
|------------|----------------|--------------|
| Search | <span style="color:deepskyblue;">O(log n)</span> (balanced), <span style="color:orange;">O(n)</span> (unbalanced) | Find node |
| Insert | <span style="color:deepskyblue;">O(log n)</span> | Add node |
| Delete | <span style="color:deepskyblue;">O(log n)</span> | Remove node |
| Traversal | <span style="color:orange;">O(n)</span> | DFS / BFS traversal |

**Use Cases:**  
- **Hierarchical data**, **sorting**, **prefix-based searching**  
- Problems: *BST operations, Lowest Common Ancestor (LCA), Binary Tree Traversals*  

---

## 🕸️ 7. Graph

| Operation | Time Complexity | Description |
|------------|----------------|--------------|
| Add Vertex/Edge | <span style="color:limegreen;">O(1)</span> / <span style="color:limegreen;">O(1)</span> | Basic structure |
| DFS / BFS | <span style="color:orange;">O(V + E)</span> | Traversal |
| Shortest Path (Dijkstra) | <span style="color:deepskyblue;">O(E log V)</span> | Priority queue |
| Topological Sort | <span style="color:orange;">O(V + E)</span> | DAG traversal |

**Use Cases:**  
- **Network / relationship problems**, **shortest paths**, **cycle detection**  

---

## 🪙 8. Hash Table / Map / Dictionary

| Operation | Average | Worst Case |
|------------|----------|-------------|
| Insert | <span style="color:limegreen;">O(1)</span> | <span style="color:orange;">O(n)</span> |
| Delete | <span style="color:limegreen;">O(1)</span> | <span style="color:orange;">O(n)</span> |
| Search | <span style="color:limegreen;">O(1)</span> | <span style="color:orange;">O(n)</span> |

**Use Cases:**  
- **Fast lookup**, **frequency counting**, **caching**, **memoization**  
- Problems: *Two Sum, Subarray Sum, Duplicate Check*  

---

## ⚖️ 9. Heap / Priority Queue

| Operation | Time Complexity | Description |
|------------|----------------|--------------|
| Insert | <span style="color:deepskyblue;">O(log n)</span> | Heapify up |
| Get Min/Max | <span style="color:limegreen;">O(1)</span> | Root element |
| Delete Min/Max | <span style="color:deepskyblue;">O(log n)</span> | Heapify down |

**Use Cases:**  
- **Top-K**, **Scheduling**, **Median finding**, **Dijkstra’s Algorithm**  

---

## 🔤 10. String Algorithms

| Operation | Time Complexity | Example |
|------------|----------------|----------|
| Length / Access | <span style="color:limegreen;">O(1)</span> | `s[i]` |
| Concatenation | <span style="color:orange;">O(n)</span> | `s1 + s2` |
| Substring Search | <span style="color:tomato;">O(n*m)</span> (naive), <span style="color:deepskyblue;">O(n+m)</span> (KMP) | Pattern search |
| Reverse | <span style="color:orange;">O(n)</span> | `s[::-1]` |

**Use Cases:**  
- Pattern Matching, Palindromes, String Hashing  

---

## 📚 Categories by Problem Type

| Category | Common DS Used | Typical Problems |
|-----------|----------------|------------------|
| Array / String | Array, HashMap | Two Sum, Sliding Window, Prefix Sum |
| Linked Data | LinkedList, Stack | Reverse List, Cycle Detection |
| Tree / Recursion | Tree, Stack | Traversal, Depth, LCA |
| Graph | Graph, Queue, Heap | Shortest Path, Connected Components |
| Dynamic Programming | Array, Map | Subset Sum, LIS, Knapsack |
| Greedy | Heap, Sorting | Activity Selection, Huffman Encoding |

---

## 🧮 Quick Big-O Reference

| Complexity | Example | Meaning |
|-------------|----------|----------|
| <span style="color:limegreen;">O(1)</span> | Hash lookup | Constant time |
| <span style="color:deepskyblue;">O(log n)</span> | Binary search | Logarithmic |
| <span style="color:orange;">O(n)</span> | Linear scan | Grows with input |
| <span style="color:gold;">O(n log n)</span> | Merge sort | Log-linear |
| <span style="color:tomato;">O(n²)</span> | Nested loops | Quadratic |
| <span style="color:red;">O(2ⁿ)</span> | Recursion (subset) | Exponential |

---

> 🧩 **Tip:** Learn operations + time complexity → map to problem type → choose best data structure.


# 🧠 DSA MAP — Reference Guide

A quick guide to common **Data Structures**, their **operations**, **time complexities**, and **use-cases**.

---

## ⚡ Complexity Growth (Visual Overview)

📈 **X-axis:** Input Size (n)  
📉 **Y-axis:** Time Taken

| Growth Curve | Big-O | Description | Example DS / Algorithm |
|---------------|--------|-------------|--------------------------|
| ▓ **Flat line** | <span style="color:limegreen;">O(1)</span> | Constant — doesn’t grow with input | Hash lookup, Stack push/pop |
| ╱ | <span style="color:deepskyblue;">O(log n)</span> | Slow growth | Binary Search, Heap, BST |
| ╱╱ | <span style="color:orange;">O(n)</span> | Linear growth | Array traversal, Queue |
| ╱╱╱ | <span style="color:gold;">O(n log n)</span> | Near-linear | MergeSort, QuickSort (avg) |
| ╱╱╱╱ | <span style="color:tomato;">O(n²)</span> | Quadratic | Bubble Sort, nested loops |
| ╱╱╱╱╱ | <span style="color:red;">O(2ⁿ)</span> | Exponential | Recursion, Subset generation |

---

## 🧩 Comparison Chart — Time Complexity by Data Structure

| Data Structure | Access | Search | Insert | Delete |
|----------------|---------|---------|---------|---------|
| **Array / List** | <span style="color:limegreen;">O(1)</span> | <span style="color:orange;">O(n)</span> | <span style="color:orange;">O(n)</span> | <span style="color:orange;">O(n)</span> |
| **Linked List** | <span style="color:orange;">O(n)</span> | <span style="color:orange;">O(n)</span> | <span style="color:limegreen;">O(1)</span> (head) | <span style="color:limegreen;">O(1)</span> (head) |
| **Stack** | <span style="color:limegreen;">O(1)</span> (top) | <span style="color:orange;">O(n)</span> | <span style="color:limegreen;">O(1)</span> | <span style="color:limegreen;">O(1)</span> |
| **Queue / Deque** | <span style="color:limegreen;">O(1)</span> (front/rear) | <span style="color:orange;">O(n)</span> | <span style="color:limegreen;">O(1)</span> | <span style="color:limegreen;">O(1)</span> |
| **Hash Table / Map** | — | <span style="color:limegreen;">O(1)</span> avg | <span style="color:limegreen;">O(1)</span> avg | <span style="color:limegreen;">O(1)</span> avg |
| **Binary Search Tree (Balanced)** | <span style="color:deepskyblue;">O(log n)</span> | <span style="color:deepskyblue;">O(log n)</span> | <span style="color:deepskyblue;">O(log n)</span> | <span style="color:deepskyblue;">O(log n)</span> |
| **Heap / Priority Queue** | <span style="color:limegreen;">O(1)</span> (min/max) | <span style="color:deepskyblue;">O(log n)</span> | <span style="color:deepskyblue;">O(log n)</span> | <span style="color:deepskyblue;">O(log n)</span> |
| **Graph (Adjacency List)** | — | <span style="color:orange;">O(V+E)</span> | <span style="color:limegreen;">O(1)</span> | <span style="color:limegreen;">O(1)</span> |
| **String** | <span style="color:limegreen;">O(1)</span> (char access) | <span style="color:tomato;">O(n*m)</span> (pattern) | <span style="color:orange;">O(n)</span> | <span style="color:orange;">O(n)</span> |

---

## 🧮 Visual Growth Comparison (ASCII Chart)


---

## 📚 Categories by Problem Type

| Category | Common DS Used | Typical Problems |
|-----------|----------------|------------------|
| Array / String | Array, HashMap | Two Sum, Sliding Window, Prefix Sum |
| Linked Data | LinkedList, Stack | Reverse List, Cycle Detection |
| Tree / Recursion | Tree, Stack | Traversal, Depth, LCA |
| Graph | Graph, Queue, Heap | Shortest Path, Connected Components |
| Dynamic Programming | Array, Map | Subset Sum, LIS, Knapsack |
| Greedy | Heap, Sorting | Activity Selection, Huffman Encoding |

---

## 🧮 Quick Big-O Reference

| Complexity | Example | Meaning |
|-------------|----------|----------|
| <span style="color:limegreen;">O(1)</span> | Hash lookup | Constant time |
| <span style="color:deepskyblue;">O(log n)</span> | Binary search | Logarithmic |
| <span style="color:orange;">O(n)</span> | Linear scan | Grows with input |
| <span style="color:gold;">O(n log n)</span> | Merge sort | Log-linear |
| <span style="color:tomato;">O(n²)</span> | Nested loops | Quadratic |
| <span style="color:red;">O(2ⁿ)</span> | Recursion (subset) | Exponential |

---

> 🧭 **Tip:** The lower and flatter the curve → the faster the algorithm for large inputs.

---


# Java Collections — Two-Column Vertical Layout

## Overview
All major Java Collections grouped cleanly into two vertical columns for quick scanning.

---

## Two-Column Table

| **Category / Types** | **Category / Types** |
|----------------------|-----------------------|
| **Core Interfaces** | **Queue Implementations** |
| • Collection        | • PriorityQueue |
| • List              | • ArrayDeque |
| • Set               | • LinkedList |
| • Queue             | • ConcurrentLinkedQueue |
| • Deque             | • LinkedBlockingQueue |
| • Map               | • ArrayBlockingQueue |
|                     | • PriorityBlockingQueue |
|                     | • DelayQueue |
|                     | • SynchronousQueue |
|                     | • LinkedTransferQueue |
| **List Implementations** | **Deque Implementations** |
| • ArrayList         | • ArrayDeque |
| • LinkedList        | • LinkedList |
| • Vector            | • ConcurrentLinkedDeque |
| • Stack (legacy)    | • LinkedBlockingDeque |
| • CopyOnWriteArrayList | |
| **Set Implementations** | **Specialized Collections** |
| • HashSet           | • BitSet |
| • LinkedHashSet     | • EnumSet |
| • TreeSet           | • EnumMap |
| • EnumSet           | • Properties |
| • CopyOnWriteArraySet | • TreeMap / TreeSet |
| • ConcurrentSkipListSet | • ConcurrentSkipListMap / Set |
| • AbstractSet       | |
| **Map Implementations** | **Legacy (Avoid)** |
| • HashMap           | • Vector |
| • LinkedHashMap     | • Stack |
| • TreeMap           | • Hashtable |
| • Hashtable         | • Dictionary |
| • ConcurrentHashMap | • Properties |
| • WeakHashMap       | |
| • IdentityHashMap   | |
| • EnumMap           | |
| • ConcurrentSkipListMap | |
| • Properties        | |
| **Abstract Base Classes** | |
| • AbstractCollection | |
| • AbstractList       | |
| • AbstractSequentialList | |
| • AbstractSet        | |
| • AbstractQueue      | |
| • AbstractMap        | |

---

If you want, I can produce a **3-column**, **color-coded**, or **cheatsheet-optimized** markdown version.

