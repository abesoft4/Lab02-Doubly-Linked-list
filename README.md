# Lab02-Doubly-Linked-List

---

## Instructions

In this exercise, you will implement a doubly linked list in C and practice various operations, such as insertion, deletion, searching, and traversal. Use the given data values in each exercise to guide your work, and ensure your program handles pointer management properly for both the `next` and `prev` pointers.

---

## Exercises

### 1) Exercise 1 – Defining the Doubly Linked List Node
- Define a structure called `Node` with the following fields:
  - `data` (an integer to store the node’s data).
  - `next` (a pointer to the next `Node` in the list).
  - `prev` (a pointer to the previous `Node` in the list).
- In the `main` function, create a pointer to the head of the list and initialize it to `NULL`.

---

### 2) Exercise 2 – Insertion Operations

**(a) Insertion at the Beginning**  
Write a function, `insertAtBeginning`, that:
- Takes a pointer to the head of the list and an integer value as input.
- Creates a new node, sets its `data` field, and links it at the beginning of the list.
- Updates the `prev` pointer of the original head node (if it exists) and assigns the new node as the head.  
In `main`, insert the values **15** and **10** at the beginning of the list and print the list after each insertion.

**(b) Insertion at the End**  
Write a function, `insertAtEnd`, that:
- Takes a pointer to the head of the list and an integer value as input.
- Creates a new node, sets its `data` field, and links it at the end of the list.
- Ensures the `prev` pointer of the new node is set correctly, and updates the `next` pointer of the last node.  
In `main`, insert the values **20**, **25**, and **30** at the end of the list and print the list after each insertion.

**(c) Insertion in Between Nodes**  
Write a function, `insertAfter`, that:
- Takes a pointer to the head of the list, an integer value for the new node, and a target value.
- Locates the first node containing the target value, then inserts the new node directly after it.
- Adjusts the `next` and `prev` pointers of neighboring nodes accordingly.  
In `main`, use `insertAfter` to insert the value **17** after the node containing **15**, and then print the list.

---

### 3) Exercise 3 – Deletion Operations

**(a) Deletion at the Beginning**  
Write a function, `deleteAtBeginning`, that:
- Takes a pointer to the head of the list.
- Removes the head node, updates the head pointer, and frees the memory of the deleted node.
- Ensures the `prev` pointer of the new head node is set to `NULL`.  
In `main`, call `deleteAtBeginning` to remove the first node and print the list.

**(b) Deletion at the End**  
Write a function, `deleteAtEnd`, that:
- Takes a pointer to the head of the list.
- Traverses to the last node, removes it, updates the `next` pointer of the second-last node, and frees the memory of the deleted node.  
In `main`, call `deleteAtEnd` to remove the last node and print the list.

**(c) Deletion in Between Nodes**  
Write a function, `deleteNode`, that:
- Takes a pointer to the head of the list and a target value.
- Locates the first node containing the target value, removes it, and updates the `next` and `prev` pointers of neighboring nodes.
- Frees the memory of the deleted node.  
In `main`, call `deleteNode` to remove the node with the value **20** and print the updated list.

---

### 4) Exercise 4 – Searching in a Doubly Linked List
Write a function, `searchNode`, that:
- Takes a pointer to the head of the list and a target value.
- Traverses the list to find the first occurrence of the target value.
- If the value is found, returns a pointer to the node; otherwise, returns `NULL`.  
In `main`, call the `searchNode` function to search for the values **25** and **17** and print an appropriate message if each value is found or not.

---

### 5) Exercise 5 – Traversal of a Doubly Linked List

**(a) Forward Traversal**  
Write a function, `traverseForward`, that:
- Takes a pointer to the head of the list.
- Traverses the list from the head to the last node, printing the data value of each node.  
In `main`, test `traverseForward` on your list and verify the printed sequence of values.

**(b) Backward Traversal**  
Write a function, `traverseBackward`, that:
- Takes a pointer to the last node in the list (find the last node by traversing from the head if necessary).
- Traverses the list from the last node to the head, printing the data value of each node.  
In `main`, test `traverseBackward` on your list and verify the printed sequence of values.

