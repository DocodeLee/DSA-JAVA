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
