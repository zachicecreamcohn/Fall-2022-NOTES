# M0: Pre Lecture

## 1.1 Data Structures

- <u>Data Structure</u>
  - A way of organizing, storing, and performing operations on data


### Common Data Structures
| Data Structure | Description                                                                                                                                                                                                          |
|----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Record         | Stores subitems, often called fields, with a name associated with each subitem                                                                                                                                       |
| Array          | Stores an ordered list of items, where each item is directly accessible by a positional index                                                                                                                        |
| Linked List    | Stores an ordered list of items in nodes, where each node stores data and has a pointer to the next node                                                                                                             |
| Binary Tree    | Each node stores data and has up to two children, known as a "left child" and a "right child"                                                                                                                        |
| Hash Table     | Stores unordered items by mapping (or hashing) each item to a location in an array                                                                                                                                   |
| Max-heap       | A tree where a node's key is >= the node's childrens' keys                                                                                                                                                           | 
| Min-heap       | A tree where a node's key is <= the node's childrens' keys                                                                                                                                                           | 
| Graph          | A data structure for representing connections among items. Consists of vertices connected by edges. <br/> <br/> A **vertex** represents an item in a graph. An **edge** represents a connection between two vertices | 


- To insert an item into a linked list, a node is created for new item, and pointers are changed to include the new node. 
  - No shifting required.

## 1.2 Introduction to algorithms

- <u>Algorithm</u>
  - A squence of steps to solve a computational problem or perform a calculation.
- <u>Computational Problem</u>
  - Specifies an input, a question about input that can be answered using a computer, and the desired output.

### Common Algorithms
| Common Algorithm                 | Description                                                                                                         |
|----------------------------------|---------------------------------------------------------------------------------------------------------------------|
| Longest common substring problem | Determines the longest common substring that exists in two input strings                                            |
| Binary Search                    | Efficient algorithm for searching a list. List's elements must be sorted and directly accessible (like in an array) |
| Dijkstra's shortest path         | Determines the shortest path from a start vertex to each vertex in a graph.                                         |

- <u>NP-Complete</u> problems
  - A set of problems for which no known efficient algorithm exists.
  - Have the following characteristics
    1. No efficient algorithm has been found to solve NP-complete problem
    2. No one has proven that an efficient algorithm to solve an NP-complete problem is impossible
    3. If an efficient algorithm exists for one NP-complete problem, then _all_ NP-complete problems can be solved efficiently


- An <u>efficient algorithm</u> is one whose runtime increases no more than polynomially with respect to input size. 
- An <u>inefficient algorithm</u> is one whose runtime increases exponentially with respect to input size.


## 1.3 Relation between data structures and algorithms
- Return first item
  - Linked list : `list->head`
  - Array : `array[0]`

## 1.4 Abstract data types
- <u>Abstract data type (ADT)<u>
  - data type described by predefined user operations without indicating how each operation is implemented.
  - A programmer does not need to know the underlying implementation of the list ADT in order to use a list.

### Common ADTs
| Abstract Data Type (ADT) | Description                                                                                                                                | Common underlying data structure |
|--------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|
| List                     | ADT for holding ordered data                                                                                                               | Array, linked list               |
| Dynamic Array            | ADT for holding ordered data _and allowing indexed access_                                                                                 | Array                            |
| Stack                    | ADT in which items are only inserted or removed from the top of a stack                                                                    | Linked list                      |
| Queue                    | ADT in which items are inserted at the end of the queue and removed from the front of the queue                                            | Linked list                      |
| Deque                    | (doubled ended queue), ADT in which items can be inserted nad removed from both the front and back                                         | Linked list                      | 
| Bag                      | ADT for storing items in which the order does not matter and duplicate items are allowed                                                   | Array, linked list               |
| Set                      | ADT for a collection of distinct items                                                                                                     | Binary search tree, hash table   |
| Priority queue           | A queue where each item has a priority, and items with higher priority are closer to the front of the queue than items with lower priority | Heap                             |
| Dictionary (map)         | ADT that associates (or maps) keys with values                                                                                             | Hash table, binary search tree   | 



## 1.5 Applications of ADTs

### Standard Libraries in various programming languages
| Programming Language | Library                         | Common supported ADTs                       |
|----------------------|---------------------------------|---------------------------------------------|
| Python               | Python standard library         | list, set dict, deque                       |
| C++                  | Standard template library (STL) | vector, list, deque, queue, stack, set, map |
| Java                 | Java collections framework (JSF) | Collection, Set, List, Map, Queue, Deque    |


## 1.6 Sorting: Introduction
- <u>Sorting</u>
  - The process of converting a list of elements into ascending (or descending) order
  - Because the program can't "see" the entire list, it needs to move in simpler steps, typically observing or swapping just two elements at a time.

## 1.7 Selection sort
- <u>Selection Sort</u>
  - A sorting algorithm that treats the input as two parts, a sorted part and an unsorted part, and repeatedly selects the proper next valye to move from the unsorted part to the end of the sorted part.
  - O(N^2)
- 