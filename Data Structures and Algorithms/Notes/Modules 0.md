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
