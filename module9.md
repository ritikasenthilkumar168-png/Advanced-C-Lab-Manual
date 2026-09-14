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
float stack[100];
int size=3,top=-1,i;
void push (float data)
{
    if(top==size-1){
        printf("stack is full\n");
    }
    else{
        top+=1;
        stack[top]=data;
    }
}
void display()
{
     for(i=top;i>=0;i--)
    {
        printf("%.2f ",stack[i]);
    }
    if(top==-1)
    {
        printf("stack is empty\n");
    }
}
void pop ()
{
    if(top==-1)
    {
        printf("stack is empty");
    }
    else
    {
        top=top-1;
    }
}
void peek()
{
       printf("%.2f ",stack[top]);
}
```

Output:
<img width="970" height="811" alt="WhatsApp Image 2026-09-14 at 5 35 44 PM" src="https://github.com/user-attachments/assets/bb2f0a15-c199-4464-bbd3-b22665cb5fa6" />


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
int size=3,top=-1;
float stack[100];
void push (float data)
{
    if(top==size-1)
    {
        printf("stack is full\n");
    }
    else
    {
        top=top+1;
        stack[top]=data;
    }
}
```

Output:
<img width="390" height="520" alt="WhatsApp Image 2026-09-14 at 5 35 57 PM" src="https://github.com/user-attachments/assets/12407454-3994-436b-86c7-59c61e70ce42" />


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
int front,rear;
char queue[100];
void display(){
    if(front==-1||front>rear){
        printf("No elements to display");
    }
    else{
        for(int i=front;i<=rear;i++){
            printf("%c\n",queue[i]);
        }
    }
}
```

Output:
<img width="667" height="517" alt="WhatsApp Image 2026-09-14 at 5 36 13 PM" src="https://github.com/user-attachments/assets/c05bc00d-848a-4fc5-96b5-772fbe0b395a" />


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
int rear,front,size=3;
int queue[50];
void enqueue(int data) 
{
    if (rear<size)
    {
        if(front==-1)
        front++;
        rear++;
        queue[rear]=data;
    }
 
}
```

Output:
<img width="868" height="538" alt="WhatsApp Image 2026-09-14 at 5 36 29 PM" src="https://github.com/user-attachments/assets/5c0e0ddc-3dd0-45f3-a257-bdb62fbbf025" />


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
int front, rear;
void dequeue()
{
    if(front==-1||front>rear){
        printf("No elements to display");
    }
    else{
        front++;
    }
}
```

Output:
<img width="722" height="642" alt="WhatsApp Image 2026-09-14 at 5 36 44 PM" src="https://github.com/user-attachments/assets/e36e2c6c-eabf-40fc-9900-766c4aa57d8a" />

Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
