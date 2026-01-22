* Bubble Sort in C

* Overview
This program sorts an array of 9 integers using the bubble sort algorithm.
It uses pointers, pass-by-reference, arrays, and functions.
The array is printed before sorting, after each swap, and after sorting.

* Functions

* printValues(int* array)
Input: Pointer to integer array  
Output: Prints array  
Return: None  

Steps:
1. Print '['
2. Loop through array
3. Print each value
4. Print ']'

* swap(int* a, int* b)
Input: Pointers to two integers  
Output: Values swapped in memory  
Return: None  

Steps:
1. Create temp variable
2. temp = *a
3. *a = *b
4. *b = temp

* sort(int* array)
Input: Pointer to integer array  
Output: Sorted array  
Return: None  

Steps:
1. Loop i from 0 to MAX-1
2. Loop j from 0 to MAX-2-i
3. Compare array[j] and array[j+1]
4. Swap if needed
5. Print array after swap