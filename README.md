# Bubble Sort in C

## Overview
This program sorts an array of 9 integers using the bubble sort algorithm.
It uses pointers, pass-by-reference, arrays, and functions.
The array is printed before sorting, after each swap, and after sorting. 

The program prints the array:  
- Before sorting  
- After every swap  
- After sorting  

---

## Functions

### printValues(int* array)
**Input:** Pointer to the array  
**Output:** Prints the array in a single line with brackets  
**Return:** None  

**How it works:**  
1. Print `'['`  
2. Loop through the array from index 0 to MAX-1  
3. Print each number followed by a space  
4. Print `']'` and a newline  

---

### swap(int* a, int* b)
**Input:** Pointers to two integers  
**Output:** Swaps the values in memory  
**Return:** None  

**How it works:**  
1. Create a temporary variable `temp`  
2. Set `temp = *a`  
3. Set `*a = *b`  
4. Set `*b = temp`  

---

### sort(int* array)
**Input:** Pointer to the array  
**Output:** Sorts the array using bubble sort  
**Return:** None  

**How it works:**  
1. Outer loop `i` goes from 0 to MAX-1 (number of passes)  
2. Inner loop `j` goes from 0 to MAX-2-i (comparing each pair)  
3. Compare `array[j]` and `array[j+1]`  
4. If `array[j] > array[j+1]`, call `swap(&array[j], &array[j+1])`  
5. Call `printValues(array)` after each swap so I can see the array changing  

---

### main()
**Input:** None  
**Output:** Runs the program  
**Return:** 0  

**What I did in main:**  
1. Created the array `{7,3,9,4,6,1,2,8,5}`  
2. Printed `"Before:"` and the array  
3. Tested the swap function with `x = 3` and `y = 5`  
4. Called `sort(array)`  
5. Printed `"After:"` and the sorted array  