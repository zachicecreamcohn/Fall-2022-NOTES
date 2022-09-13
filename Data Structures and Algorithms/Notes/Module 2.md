## 3.7 Doubly-linked lists
- <u>doubly-linked list</u>
  - a data structure for implementing a list ADT
  - each node has data, a pointer to the next node, pointer to the previous node
  - Just like a singly-linked list, but it has pointers going to the next **and previous** nodes

## 3.10 Linked list traversal
- <u>list traversal</u>
  - visits all nodes in the list once and performs an operation on each node
  - Supports both singly linked and doubly linked lists
  - Starts at the head
- <u>Reverse Transversal
  - starts at the tail
  - Supports only doubly-linked list
- <u>Insertion sort for doubly-linked lists</u>
  - only works for doubly-linked lists because backward transversal only works on doubly-linked lists
  - O(N^2)