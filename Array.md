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
 declare min int ::: int min = array[0];

 iterate array

 update if you find smaller value ::: if( min > array[i]) {min = array[i];}

 return the updated min ::: return min;

## Find second maximum value in Array
 declare two int value 1.maximum 2. secondMaximu

 Iterate the number

 if number is bigger than maximum > update it with bigger and bigger becomes second

 YOU NEED TO CONSIDER IF THE VALUE IS BETWEEN MAX AND SECOND, ::: else if (arr[i] > secMax && arr[i] < Max)

 after it finish

 return secondMax

## Move all zeros to the end of Array
We will get int Array and wants to send 0 to end of array

>>I thought we need sort() and need to use temp as main but it wasn't

First declare pointer 1 > this is the setted until the condition changed

iterate the array

exchange if pointer1 is 0 and array value is not 0 (when change, use int temp)

and in other condition : increase pointer 1 when it is not 0

There is no statement for sortion so just finish the code in here

## How to Resize Array
make new array with new size ::: int[] temp = new int[length];

>iterate 0 to temp.length

change temp to input ::: inputArray = temp;

## Find the Missing Number in Array
// maybe brutally wee can find missing number but it is not good for solving problem

// mathmetical approach : add from 0 to n = n(n+1)/2

int n = array.length + 1;

int sum = n * (n +1) /2

for(int num : nums) {sum = sum - num}

return sum;

## How to Check String is Palindrome
> We are going to get String and return type is Boolean

char[] charArray = inputString.toCharArray();

int start = 0;

int end = string.length - 1;

while(start < end)

if( charArray[start] != charArray[end]) return false;

or start ++ ; end ++;

return true;

