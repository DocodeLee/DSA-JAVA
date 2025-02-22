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

## How to remove a given value from singly linked list in java
1. set current as pointer on the head  :: ListNode current = head;
2. set temp as null pointer :: ListNode temp = null;
3. move current until null and it is not match with value :: while(current != null && current.data != value)
4. each step move temp to current, current moves to next :: temp = current; current = current.next;
5. if in array there were no same value return;
6. if found temp.next = current.next; (temp is currently on the previous of current Node)
<img width="843" alt="image" src="https://github.com/user-attachments/assets/22668d5f-8fd3-4643-b8ae-c33882299e30" />

## How to dectec a loop in a sinlgly linked list

### In this problem we need to use two pointer which has different speed;

1. ListNode fast = head;
2. ListNode slow = head;
3. move fast until fast will be null :: while( fast != null && fast.next !=null)
fast = fast.next.next; // move two steps

slow = slow.next;
4. if(fast == slow){ return true}
5. or false;;

## How to find a start of loop in singly linked list
### This is to find a start point of the loop

first part is same 

set fast and slow > move fast and step with different speed > if (fast == slow) part appears

return getStartingNode(slow);

### Make a method 
private ListNode getStartingNode(ListNode slow)

set the temp node on head > move temp and slow until temp meet slow > if meet return temp

<img width="883" alt="image" src="https://github.com/user-attachments/assets/57b2dcb8-6816-4880-a11f-810c845b1d23" />
<img width="1036" alt="image" src="https://github.com/user-attachments/assets/fb8b6bb4-e6e4-48e7-a69f-4c7180fc500f" />
<img width="475" alt="image" src="https://github.com/user-attachments/assets/cf0178f7-4b90-4ebb-ae8f-de0b957a3196" />

Regardless of length of array, the slow pointer will meet fast in the kth node of loop and r will be left

and this r is the always same with m length. so if temp starts from the head to node slow will move few rotations + r distance

## How to remove loop
Same unitl detecting loop.

if detect find the head of loop and finally set slow.next =null;

## Merge two sorted signly linked list
1. declare dummyNode with random value > dummy.next will be the head
2. set the tail on the dummyNode
3. compare a.data and b.data if a is smaller > connect tail to a , if b is smaller, connect tail to be
4. move each part to next
5. tail = tail.next << update tail to the last Node
6. if one list over jsut move tail to another one
7. return dummy.next becasue dummy is not the member of linkedList

## Add two singly linked list 9:22
