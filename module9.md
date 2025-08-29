EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:
#include <stdio.h>
#define MAX 100

int stack[MAX];
int top = -1;

// Function to push element into stack
void push(int x) {
    if (top == MAX - 1) {
        printf("Stack Overflow\n");
    } else {
        stack[++top] = x;
        printf("%d pushed to stack\n", x);
    }
}

// Function to pop element from stack
void pop() {
    if (top == -1) {
        printf("Stack Underflow\n");
    } else {
        printf("%d popped from stack\n", stack[top--]);
    }
}

// Function to display stack elements
void display() {
    if (top == -1) {
        printf("Stack is empty\n");
    } else {
        printf("Stack elements: ");
        for (int i = 0; i <= top; i++) {
            printf("%d ", stack[i]);
        }
        printf("\n");
    }
}

int main() {
    int choice, value;

    while (1) {
        printf("\n--- Stack Menu ---\n");
        printf("1. Push\n2. Pop\n3. Display\n4. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);

        switch (choice) {
            case 1:
                printf("Enter value to push: ");
                scanf("%d", &value);
                push(value);
                break;
            case 2:
                pop();
                break;
            case 3:
                display();
                break;
            case 4:
                return 0;
            default:
                printf("Invalid choice!\n");
        }
    }
}


Output:

<img width="1918" height="896" alt="image" src="https://github.com/user-attachments/assets/8034de5b-de5f-4192-8f19-fcda17880876" />




Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:
#include <stdio.h>
#define MAX 100

int stack[MAX];
int top = -1;

// Function to push element into stack
void push(int x) {
    if (top == MAX - 1) {
        printf("Stack Overflow\n");
    } else {
        stack[++top] = x;
        printf("%d pushed into stack\n", x);
    }
}

// Function to display stack elements
void display() {
    if (top == -1) {
        printf("Stack is empty\n");
    } else {
        printf("Stack elements: ");
        for (int i = 0; i <= top; i++) {
            printf("%d ", stack[i]);
        }
        printf("\n");
    }
}

int main() {
    int n, value;

    printf("Enter number of elements to push: ");
    scanf("%d", &n);

    for (int i = 0; i < n; i++) {
        printf("Enter value to push: ");
        scanf("%d", &value);
        push(value);
    }

    display();

    return 0;
}

Output:
<img width="1863" height="907" alt="image" src="https://github.com/user-attachments/assets/ff1863e1-2f1a-4995-b3df-c8878cc82c7c" />




Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:
#include <stdio.h>
#define MAX 100

int queue[MAX];
int front = -1, rear = -1;

// Function to insert element into queue
void enqueue(int x) {
    if (rear == MAX - 1) {
        printf("Queue Overflow\n");
    } else {
        if (front == -1) front = 0; // first element
        queue[++rear] = x;
        printf("%d enqueued into queue\n", x);
    }
}

// Function to display queue elements
void display() {
    if (front == -1 || front > rear) {
        printf("Queue is empty\n");
    } else {
        printf("Queue elements: ");
        for (int i = front; i <= rear; i++) {
            printf("%d ", queue[i]);
        }
        printf("\n");
    }
}

int main() {
    int n, value;

    printf("Enter number of elements to enqueue: ");
    scanf("%d", &n);

    for (int i = 0; i < n; i++) {
        printf("Enter value to enqueue: ");
        scanf("%d", &value);
        enqueue(value);
    }

    display();

    return 0;
}


Output:
<img width="1908" height="886" alt="image" src="https://github.com/user-attachments/assets/0deb03db-1038-4b77-a145-73d7f25b879c" />


Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:
#include <stdio.h>
#define MAX 100

int queue[MAX];
int front = -1, rear = -1;

// Function to insert element into queue
void enqueue(int x) {
    if (rear == MAX - 1) {
        printf("Queue Overflow\n");
    } else {
        if (front == -1) front = 0;  // first element
        queue[++rear] = x;
        printf("%d inserted into queue\n", x);
    }
}

// Function to display queue
void display() {
    if (front == -1 || front > rear) {
        printf("Queue is empty\n");
    } else {
        printf("Queue elements: ");
        for (int i = front; i <= rear; i++) {
            printf("%d ", queue[i]);
        }
        printf("\n");
    }
}

int main() {
    int n, value;

    printf("Enter number of elements to insert: ");
    scanf("%d", &n);

    for (int i = 0; i < n; i++) {
        printf("Enter value to insert: ");
        scanf("%d", &value);
        enqueue(value);
    }

    display();

    return 0;
}


Output:

<img width="1911" height="896" alt="image" src="https://github.com/user-attachments/assets/6096369c-9c0b-4e6d-a1f4-e257beb6cbc9" />

Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:
#include <stdio.h>
#define MAX 100

int queue[MAX];
int front = -1, rear = -1;

// Function to insert (enqueue) element
void enqueue(int x) {
    if (rear == MAX - 1) {
        printf("Queue Overflow\n");
    } else {
        if (front == -1) front = 0;  // first insertion
        queue[++rear] = x;
        printf("%d inserted into queue\n", x);
    }
}

// Function to delete (dequeue) element
void dequeue() {
    if (front == -1 || front > rear) {
        printf("Queue Underflow (empty queue)\n");
    } else {
        printf("%d deleted from queue\n", queue[front]);
        front++;
    }
}

// Function to display queue
void display() {
    if (front == -1 || front > rear) {
        printf("Queue is empty\n");
    } else {
        printf("Queue elements: ");
        for (int i = front; i <= rear; i++) {
            printf("%d ", queue[i]);
        }
        printf("\n");
    }
}

int main() {
    enqueue(10);
    enqueue(20);
    enqueue(30);
    display();

    dequeue();
    display();

    dequeue();
    display();

    return 0;
}


Output:
<img width="1893" height="883" alt="image" src="https://github.com/user-attachments/assets/2afe0057-5012-4eda-928f-27db3cd22d27" />


Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
