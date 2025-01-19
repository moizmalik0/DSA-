# DSA-Final Assignment
# Node class to create a new node for the linked list
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

# Stack implementation using Linked List
class Stack:
    def __init__(self):
        self.top = None  # Initialize the stack with no elements

    def push(self, data):
        """Add an element to the stack."""
        new_node = Node(data)
        new_node.next = self.top
        self.top = new_node
        print(f"Pushed {data} onto the stack.")

    def pop(self):
        """Remove and return the top element of the stack."""
        if self.is_empty():
            print("Stack is empty. Nothing to pop.")
            return None
        popped_data = self.top.data
        self.top = self.top.next
        print(f"Popped {popped_data} from the stack.")
        return popped_data

    def peek(self):
        """Return the top element without removing it."""
        if self.is_empty():
            print("Stack is empty. Nothing to peek.")
            return None
        return self.top.data

    def is_empty(self):
        """Check if the stack is empty."""
        return self.top is None

# Queue implementation using Linked List
class Queue:
    def __init__(self):
        self.front = None  # Front of the queue
        self.rear = None   # Rear of the queue

    def enqueue(self, data):
        """Add an element to the end of the queue."""
        new_node = Node(data)
        if self.rear is None:  # If the queue is empty
            self.front = self.rear = new_node
        else:
            self.rear.next = new_node
            self.rear = new_node
        print(f"Enqueued {data} into the queue.")

    def dequeue(self):
        """Remove and return the front element of the queue."""
        if self.is_empty():
            print("Queue is empty. Nothing to dequeue.")
            return None
        dequeued_data = self.front.data
        self.front = self.front.next
        if self.front is None:  # If the queue becomes empty
            self.rear = None
        print(f"Dequeued {dequeued_data} from the queue.")
        return dequeued_data

    def peek(self):
        """Return the front element without removing it."""
        if self.is_empty():
            print("Queue is empty. Nothing to peek.")
            return None
        return self.front.data

    def is_empty(self):
        """Check if the queue is empty."""
        return self.front is None

# Driver code to demonstrate functionality
if __name__ == "__main__":
    # Stack demonstration
    print("Stack Operations:")
    stack = Stack()
    stack.push(10)
    stack.push(20)
    stack.push(30)
    print(f"Top element: {stack.peek()}")
    stack.pop()
    print(f"Top element after pop: {stack.peek()}")
    print()

    # Queue demonstration
    print("Queue Operations:")
    queue = Queue()
    queue.enqueue(10)
    queue.enqueue(20)
    queue.enqueue(30)
    print(f"Front element: {queue.peek()}")
    queue.dequeue()
    print(f"Front element after dequeue: {queue.peek()}")

Conclusion: 
Objective: Implementation of Stack and Queue using Linked List
GitHub Submission:
LinkedIn Post:

Implementation of Stack and Queue Using Linked List
GitHub Submission:

Code Implementation:

README Template
Stack and Queue Implementation Using Linked List
Overview
This repository contains implementations of Stack and Queue using Linked List. These implementations demonstrate a foundational understanding of core data structures and how linked lists can be leveraged for dynamic memory management.

Features
Dynamic data management using Linked List.
Efficient implementation of Stack (LIFO) and Queue (FIFO).
How to Run the Program
Clone the Repository:
Stack-queue-implementation  
Example for Python:
python stack_queue.py  
Code Purpose:
Stack: Perform operations like push, pop, and peek using a linked list.
Queue: Implement enqueue, dequeue, and front operations.
Time Complexity
Operation	Stack	Queue
Push	O(1)	N/A
Pop	O(1)	N/A

LinkedIn Post
implemented Stack and Queue using Linked Lists! ... This hands-on task allowed me to dive deeper into fundamental data structures while exploring the dynamic memory allocation capabilities of linked lists.

Key Highlights:
Stack Implementation: Efficiently managed LIFO operations like push, pop, and peek.
This project not only honed my programming skills but also deepened my understanding of modular coding and algorithmic efficiency. Throughout the process, I prioritized clean and well-documented code to make the repository beginner-friendly and reusable.

GitHub Submission
README File
Here’s the structure we can use for your README:

Stack and Queue Using Linked List
This is a simple project where I’ve implemented Stack and Queue using Linked List to understand how these data structures work. It was really interesting to see how linked lists make operations like push and pop efficient.

Run:
Clone the repository: 
If you’re using Python, you can do:
Stack: I implemented the basic operations like push, pop, and peek.
Queue: I did enqueue, dequeue, and a front method.
Complexity
Here’s how efficient the operations are:

Operation	Stack Time Complexity	Queue Time Complexity
Push	O(1)	N/A
Pop	O(1)	N/A
I wanted to practice working with linked lists and understand how they’re used to build basic data structures. This was a good way to reinforce the concepts I learned ..

LinkedIn Post:
(https://www.linkedin.com/posts/moiz-malik-7ba020269_hey-everyone-just-completed-a-project-where-activity-7286711764119920640-Sql9?utm_source=share&utm_medium=member_android)
