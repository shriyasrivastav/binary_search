# binary_search
Project File Structure:
Let’s have a look at the steps to build binary search python project:

1. Recursive approach

Function definition
Read inputs, sort and call function
2. Iterative approach

Read inputs and sort
Loop for binary search


1. Recursive approach
I. Function definition
Code Explanation:

def binary_search(start,end,int_list,target): Declare and define the function binary search with parameters: start, end, list of elements and target element
start<=end: This condition is necessary to avoid an out_of_index_error and satisfies the condition when an element is not present in a list.
Test conditions: If the target is the middle element of the list, the position is returned, else it is checked if less than the middle element. Upon satisfying this condition, the function is called with a change in the lower and upper bounds being start and mid-1 respectively. Similarly, for the case of the target element being greater than the middle element, the bounds are updated to mid+1 and end.
Return value: The binary search python function return position, if the element is found and -1 otherwise.
II. Read inputs and call function:
Code Explanation:

Inputs: Read the list length from the user and the elements of the list. Append the elements to the list
sorted(int_list): A prerequisite for binary search is to have a sorted list. Hence using sorted(), we sort the list
Function call: The inputs are passed to the function binary_search. The value returned is printed.


2. Iterative Approach:
Now, let’s discuss python binary search iterative approach:

I. Read inputs and sort the list:
Code explanation:

Inputs: Read the list length from the user and using a for loop, read the elements of the list. Append the elements to the list
sorted(int_list): Sort the list for binary search
II. Loop for binary search
Code Explanation:

Define variables: Define variables start, and end position. Position is set to -1 initially
While loop: The terminating condition for the while loop is ‘start<=end’. Inside the loop, check the target element with the middle element, and update the position variable. If lesser than middle element, update upper bound to middle-1 and in the case of greater than middle element, update start to middle +1.
Position condition: If position remains unchanged at -1, it indicates the element is not present in the list. If it is updated, then the position is printed.
