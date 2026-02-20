Queue Implementation Using Linked List in C (Peek Operation)

This project demonstrates how to implement a Queue using a Singly Linked List in C programming language and how to display the front element (Peek operation).

📌 Description

In this program:

A queue is implemented using a linked list.

Elements are inserted using the enqueue() function.

The front element is displayed using the peek() function.

The queue follows FIFO (First In, First Out) principle.

🧠 What is a Queue?

A Queue is a linear data structure that follows:

FIFO – First In, First Out

Basic operations of queue:

Enqueue → Insert element at rear

Dequeue → Remove element from front

Peek (Front) → Display front element

IsEmpty → Check if queue is empty

📂 Data Structure Used
struct Node {
    int data;
    struct Node *next;
};

Each node contains:

data → Value stored in queue

next → Pointer to next node

Two pointers are maintained:

front → Points to first element

rear → Points to last element

🔹 Functions
enqueue(int value)

Allocates memory for a new node.

Inserts node at the end (rear).

Updates front and rear pointers accordingly.

peek()

Displays the front element of the queue.

Prints message if queue is empty.

▶️ Operations Performed in main()
enqueue(10);
enqueue(20);
enqueue(30);
peek();
Queue Representation:
Front → 10 → 20 → 30 → NULL
                     ↑
                    Rear
▶️ Sample Output
Front element = 10
⚙️ How to Compile and Run
1️⃣ Compile
gcc queue_linkedlist.c -o queue_linkedlist
2️⃣ Run
./queue_linkedlist
⏱️ Time & Space Complexity

Enqueue: O(1)

Peek: O(1)

Space Complexity: O(n)

Where:

n = Number of elements in queue

📚 Concepts Covered

Queue Data Structure

Linked List

Dynamic Memory Allocation

FIFO Principle

Front and Rear Pointer Handling

⚠️ Limitations

No dequeue() function included (can be added).

Memory is not freed using free().

👨‍💻 Author

Ritik Chauhan

If you want, I can also provide:

Full queue implementation (Enqueue, Dequeue, Peek, Display)

Menu-driven queue program

Comparison README (Queue using Array vs Linked List)
