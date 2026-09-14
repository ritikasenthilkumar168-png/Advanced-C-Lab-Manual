## EXP NO 26: C PROGRAM TO DISPLAY STACK ELEMENTS USING LINKED LIST.
# Aim:
To write a C program to display stack elements using linked list.

# Algorithm:
Define a structure Node with two members: data to store the integer value and next to point to the next node in the linked list.
Declare a global variable head representing the starting node of the linked list.
Define a function display to print the elements of the linked list.
Declare a pointer p and initialize it with the head of the linked list.
Use a while loop to traverse the linked list:
Print the data of the current node.
Move to the next node using the next pointer.
# Program:
```
struct Node   
{  
int data;  
struct Node *next;  
}*head;  
void display()  
{  
    struct Node *current=head;
    while(current!=NULL)
    {
        printf("%d\n",current->data);
        current=current->next;
    }
}
```
# Output:
<img width="445" height="587" alt="WhatsApp Image 2026-09-14 at 5 59 41 PM" src="https://github.com/user-attachments/assets/ecc8cd19-82fa-41f0-ada5-bdd3568f4e09" />

# Result:
Thus, the program to display stack elements using linked list is verified successfully.

## EXP.NO 27: C PROGRAM TO POP AN ELEMENT FROM THE GIVEN STACK USING LINKED LIST.
# Aim:
To write a C program to pop an element from the given stack using liked list.

# Algorithm:
Check for Empty Stack
If head is equal to NULL, Print "Stack is empty."
Else Proceed to the next step.
Set head to point to the next node in the stack.
# Program:
```
struct Node   
{  
int data;  
struct Node *next;  
}*head;  
void pop()  
{ 
    if(head!=0)
    {
        head=head->next;
    }
    else
    {
        printf("stack is empty");
    }
}
```
# Output:
<img width="975" height="662" alt="WhatsApp Image 2026-09-14 at 5 59 49 PM" src="https://github.com/user-attachments/assets/1c9f7b34-e8ac-4485-9cb6-da8c569099e8" />

# Result:
Thus, the program to pop an element from the given stack using liked list is verified successfully.

# EXP NO:28 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING LINKED LIST.
# Aim:
To write a C program to display queue elements using linked list.

# Algorithm:
Check if Queue is Empty
Display Queue Elements
Print the data of the current node pointed to by front
Update front to point to the next node.
End the display function.
# Program:
```
struct Node
{
   float data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void display()
{
    if(front==NULL)
    {
        printf("queue is empty\n");
    }
    else
    {
        struct Node *ptr;
        ptr=front;
        printf("queue elements:\n");
        while(ptr!=0)
        {
            printf("%.2f\n",ptr->data);
            ptr=ptr->next;
        }
    }
}
```
# Output:
<img width="711" height="646" alt="WhatsApp Image 2026-09-14 at 5 59 58 PM" src="https://github.com/user-attachments/assets/25816c7c-0d30-4bc0-b42b-b7e80b9bddd6" />

# Result:
Thus, the program to display queue elements using linked list is verified successfully.

# EXP NO:29 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING LINKED LIST
# Aim:
To write a C program to insert elements in queue using linked list

# Algorithm:
Allocate Memory for New Node
Set Data and Next Pointer
Check if Queue is Empty
Set both front and rear to point to the new node p.
Set the next pointer of the current rear to point to the new node p.
End of Enqueue Operation
# Program:
```
struct Node
{
   char data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void enqueue(float data)
{
    struct Node *ptr=(struct Node*)malloc(sizeof(struct Node));
    ptr->data=data;
    ptr->next=NULL;
    if(front==NULL)
    {
        front=rear=ptr;
    }
    else
    {
        rear->next=ptr;
        rear=ptr;
    }
}
```
# Output:
<img width="680" height="645" alt="WhatsApp Image 2026-09-14 at 6 00 11 PM" src="https://github.com/user-attachments/assets/f7df6e35-bba3-42c0-9b03-237407bb48a7" />

# Result:
Thus, the program to insert elements in queue using linked list is verified successfully.

## EXP NO:30 C FUNCTION TO FIND THE PEEK OF QUEUE USING LINKED LIST.
# Aim:
The aim of this function is to retrieve the "peek" (the front element) of a queue implemented using a linked list

# Algorithm:
Check if the queue is empty: o If the queue is empty (i.e., the front pointer is NULL), return an error or a message indicating that the queue is empty.
Access the front element: o If the queue is not empty, return the data stored in the front node of the linked list (i.e., the element at the head of the queue).
# Program:
```
struct Node
{
   char data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void peek()
{
    printf("%c",front->data);
}
```
# Output:
<img width="476" height="672" alt="WhatsApp Image 2026-09-14 at 6 00 20 PM" src="https://github.com/user-attachments/assets/d8f8cfdb-bd42-463e-b9f0-6b8b752d4496" />

# Result:
Thus, the program to retrieve the "peek" (the front element) of a queue implemented using a linked list is verified successfully.
