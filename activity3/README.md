# Activities

## Task 1:

- Refer to the following link. Discuss how Stacks based on linked lists works:
  https://www.cs.usfca.edu/~galles/visualization/StackLL.html

  Ans: 
    - In a linked list-based implementation of a stack, each element of the stack is represented as a node in a linked list. The top of the stack is represented by the head of the linked list.
    - The Push operation adds an element to the top of the stack. And the Pop operation removes the element at the top of the stack and returns it, In a linked list-based implementation, the head node is removed from the linked list and its data is returned. 
    - The Peek operation returns the element at the top of the stack without removing it. In a linked list-based implementation, the data of the head node is returned.

## Task 2:

The following snippet is from `./src/stack.cpp` lines 25-31.

```cpp
void push(StackNode **root, int new_data)
{
    StackNode *stackNode = newNode(new_data);
    stackNode->next = *root;
    *root = stackNode;
    cout << new_data << endl;
}
```

- Discuss in groups how the code works?

Ans:
  - The 'StackNode' class represents a node in the linked list, with 'data' representing the value of the node and 'next' pointing to the next node in the list.

The 'newNode' function creates a new node with the given data and returns a pointer to it.

The 'isEmpty' function checks if the given root node pointer is NULL, indicating an empty stack.

- Why do we need to use double pointers?

Ans:
  - Because we need to update the value of the 'root' pointer that points to the top of the stack after each push or pop operation.

## Task 3: Individual (At home)

Practice: Asymptotic Analysis and Upper Bounds. Refer to the following link:
https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/AlgAnal/UpperBoundsSumm.html
