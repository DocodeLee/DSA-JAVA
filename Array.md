# Array
adjacent, continuous

size is fixed and cannot modified

<img width="898" alt="image" src="https://github.com/user-attachments/assets/ea9f479e-1ea4-47c0-bd2a-7b9fd826f277" />
+ indexed and can be positioned

+ index starts 0 , lengths starts from 1

## Declaration of Array
int myArray[]; <<< int[] myArray;

## Initialization of Array
gives memory to array elements. initailized like >> arrayName = new dataType[size] ;
## Declaration + Initialization
dataType[] arrayName = new dataType[size];

int[] myArray = new int[5];
int myArray[] = new int[5];
int myArray[] = {1,2,3,4,5};

## Adding and updating Array
when add elements use index.
arrya[index] = value;
## printing out array value
use System.out.println(array[index])
## Remove elements from Array
There is no way to modify the made Array 

>Count Odd element > make a new Array with odd_size > put the only need elements
<img width="300" alt="image" src="https://github.com/user-attachments/assets/7c548aca-ad31-4c1f-99d4-fb4437845afc" />
## How to reverse Array
I thought make a new list and iterate from the last index

but we can just change using temp int

>activate new int value temp > change [start] [end] > change end with temp value > start++, end--
<img width="463" alt="image" src="https://github.com/user-attachments/assets/a4ff0910-8817-49c7-b9f7-eb7bc4ed14b7" />

## Find min value in Array
＞ declare min int ::: int min = array[0];
> iterate array 
> update if you find smaller value ::: if( min > array[i]) {min = array[i];}
> return the updated min ::: return min;
