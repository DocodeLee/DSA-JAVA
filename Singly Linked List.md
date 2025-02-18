# Singly Linked List
starts from head move to next node

head = new ListNode(value);

head.next = nextNode;

## How to print elements ins singly Linked List

Use while loop of for loop and ::: current.data >> will return value


## How to find length of Singly Linked List
declare int value for count

<img width="427" alt="image" src="https://github.com/user-attachments/assets/9e278a0f-1eb9-4b33-b66a-d4ec254a9266" />

return count;

## How to insert node at the beggining of a Singly Linked List
> Set newNode and connect first and move the head lastly

## How to insert node at the end of Singly Linked List
In this case we need to handle edge case

> ListNode newNode = new ListNode(value);  :: declare newNode

when head is null > newNode will be head

when list is not null > set current on heada;

move current until current.next != null > current = current.next;

when current.next becomes null > current.next = newNode

## Insert Node in a Singly Linked List at a given position

Case 1 : if position is 1 > it means head

ListNode newNode = new ListNode(value); 

newNode.next = head; & head = newNode;


Case 2 : else cases

call the previous Node on head and declare count value to check

if previous moves to the ( posiiton -1 ) set current on previous.next

newNode.next = current; && previous.next = newNode; 

## Delete head Node in Singly Linked List

if head is null return null

declare temp Node on temp

move head to next and set temp.next = null

then return temp

## Delete last Node in Singly Linked List

if( head == null || head.next == null) > return head;

set Current on the head and make pointer Previous

ListNode current = head;

ListNode previous = null;

while(current.next != null)

previous = current; >> by this previous is always on the previous node

current = current.next 

when loop ends > previous.next = null; ->> return current;

## Delete a node in given Position

if position is less than 0 or bigger than length return null;

if position is 1 > return head

if posiiton is k :

declare current on head and previous as null (pointer)

declare count as 1 and count++ moving current to current.next previous on current

move until k and just connect previous.next = current.next

then current.next = null and return current;

> You don't need to move two pointer from the first we know current will be next of previous so just declare aafter movement

## How to search an element in linked List
set Pointer on the head

while current is not null

if current.data is same with target return true

or just move current to next node

if nothing found return false;

## How to find nth node from the end of Linked list in java

> we need to use two pointers

1. declare first pointer
2. declare second pointer
3. declare int for counting number
4. while count < n , pointer1 = pointer1.next,  (using counter++)
5. while (pointer1 != null) , pointer1 = pointer1.next & pointer2 = pointer2.next
6. return pointer2

> Moving pointer 1 until null is the point

## How to remove duplicates from sorted Linked List in Java

### key is the sorted list java

> if next node is same with current skip the next node

1. set current Node on Head
2. while current is not null and current.next is not null // current & current.next is set to compare
3. if(current.data == current.next.data) > current.next = current.next.next;
4. else current = current.next;

We need to use else for edge case because we are using while loop so it still goes if we don't set else statement

## How to insert node in a sorted linked list in java
### key si the sorted list java

1. declare Node current on head
2. delcare temp Node as null ::: we need to use this because we need to connect new node to list
3. while current is not null and smaller than targetValue
4. temp = current (this make temp and current has 1 index different) & current = current.next; 
5. if loop is end newNode.next = current
6. temp.next = new Node;
7. return head ::: return the List

## How to remove a given key from singly linked list in java
