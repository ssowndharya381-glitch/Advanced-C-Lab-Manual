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
```
#include <stdio.h>

int main()
{
    int stack[100], top = -1;
    int n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    {
        scanf("%d", &stack[++top]);
    }

    printf("Stack elements are:\n");

    for(i = top; i >= 0; i--)
    {
        printf("%d\n", stack[i]);
    }

    return 0;
}
```
Output:

<img width="770" height="280" alt="Screenshot 2026-09-02 213435" src="https://github.com/user-attachments/assets/1ac4cb69-2c7e-454a-9a60-d10e0365e6b0" />



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

```
#include <stdio.h>

int main()
{
    int stack[100], top = -1;
    int n, i, element;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    {
        printf("Enter element: ");
        scanf("%d", &stack[++top]);
    }

    printf("Enter element to push: ");
    scanf("%d", &element);

    top++;
    stack[top] = element;

    printf("Stack after PUSH:\n");

    for(i = top; i >= 0; i--)
    {
        printf("%d\n", stack[i]);
    }

    return 0;
}
```
Output:

<img width="793" height="273" alt="Screenshot 2026-09-02 213522" src="https://github.com/user-attachments/assets/11011ce7-8b11-442a-86a5-347e9279ca16" />



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

```
#include <stdio.h>

int main()
{
    int queue[100], front = 0, rear = -1;
    int n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    {
        scanf("%d", &queue[++rear]);
    }

    printf("Queue elements are:\n");

    for(i = front; i <= rear; i++)
    {
        printf("%d ", queue[i]);
    }

    return 0;
}
```

Output:

<img width="703" height="203" alt="Screenshot 2026-09-02 213644" src="https://github.com/user-attachments/assets/c5291a86-6b15-433d-b413-86db37299316" />



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

```
#include <stdio.h>

int main()
{
    int queue[100], front = 0, rear = -1;
    int n, i, element;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    {
        printf("Enter element: ");
        scanf("%d", &queue[++rear]);
    }

    printf("Enter element to insert: ");
    scanf("%d", &element);

    rear++;
    queue[rear] = element;

    printf("Queue after insertion:\n");

    for(i = front; i <= rear; i++)
    {
        printf("%d ", queue[i]);
    }

    return 0;
}
```

Output:


<img width="687" height="198" alt="Screenshot 2026-09-02 213742" src="https://github.com/user-attachments/assets/e4f3eeb1-4fc5-4fd8-b7c1-2042a93afdcf" />


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

```
void deleteElement(int queue[], int *front, int *rear)
{
    if(*front > *rear)
    {
        printf("Queue is empty");
    }
    else
    {
        printf("Deleted element = %d\n", queue[*front]);
        (*front)++;
    }
}
```
Output:

<img width="681" height="97" alt="Screenshot 2026-09-02 213858" src="https://github.com/user-attachments/assets/7a22709d-edd6-47fe-9a08-08df6b3f81aa" />



Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
