# ADA_LAB-UE223026-
                                                                              LAB 1
                                                  PRACTICAL 1
Aim: To find time complexity of Selection Sort to represent it through graph.

Description: 
This C++ code measures the average time taken to sort randomly generated arrays using the selection sort algorithm and writes this data to a file named "data.txt". It utilizes functions for file writing, selection sorting, and timing measurements to analyze sorting performance for different array sizes.

Algorithm:
1. Selection Sort
   
•	Start with the first element as the minimum.

•	Compare the minimum element with the next element in the array.

•	If the next element is smaller, update the minimum element.

•	Repeat steps 2 and 3 for all elements in the array.

•	Swap the minimum element with the first unsorted element.

•	Move to the next unsorted element and repeat steps 2-5 until the entire array is sorted.

Time Complexity:
The time complexities of Selection Sort are as follows:
1.	Best-case time complexity: O(n^2)
2.	Worst-case time complexity: O(n^2)
3.	Average-case time complexity: O(n^2)
Here, n represents the number of elements in the array or list being sorted.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/7993df02-033d-423c-b2d6-1786d78b9309)

















                                          PRACTICAL 2
Aim: To find time complexity of Tower of Hanoi and to represent it through graph.

Description: 
This C++ code implements the Tower of Hanoi problem using recursion. It defines a function th() to solve the Tower of Hanoi problem for a given number of disks (n) and outputs the moves to transfer disks from the source peg to the destination peg. The Algo() function measures the average time taken to solve the Tower of Hanoi problem for different numbers of disks (from 1 to 9) and writes this data to a file named "data.txt" in CSV format. The main() function calls Algo() to perform these operations.

Algorithm:
1. Tower of Hanoi
   
a.	Define a function th(n, source, destination, spare) to move n disks from the source peg to the destination peg using the spare peg as an auxiliary.

b.	If n equals 1:

•	Print the move of the disk from the source peg to the destination peg.

c.	Else:

•	Recursively call th(n-1, source, spare, destination) to move n-1 disks from the source peg to the spare peg using the destination peg as an auxiliary.

•	Print the move of the nth disk from the source peg to the destination peg.

•	Recursively call th(n-1, spare, destination, source) to move n-1 disks from the spare peg to the destination peg using the source peg as an auxiliary.

Time Complexity:
The time complexities for the Tower of Hanoi algorithm are typically described in terms of the number of moves required to solve the problem. Here are the complexities:
1.	Best-case time complexity: O(2^n)
2.	Average-case time complexity: O(2^n)
3.	Worst-case time complexity: O(2^n)
In all cases, the number of moves required grows exponentially with the number of disks (n) in the Tower of Hanoi problem.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/cf8ca9ab-3357-4a77-8182-c48640ad6f38)













                                           PRACTICAL 3
Aim: To find time complexity of Horner and to represent it through graph.

Description:
This C++ code implements Horner's method for polynomial evaluation and measures the average time taken to evaluate polynomials of increasing degrees (from 1 to 1000 in steps of 10), storing the results in a file named "data.txt" and displaying them on the console.

Algorithm:
Horner
1.	Define a function Horner(a, n, m, x) to evaluate a polynomial using Horner's method, where a[] is the array of coefficients, n is the current index, m is the highest degree of the polynomial, and x is the value at which to evaluate the polynomial.
2.	If n equals m:
•	Return the coefficient a[m].
3.	Else:
•	Return (a[n] + x * Horner(a,n+1,m,x).

Time Complexity:
For Horner's method of polynomial evaluation:
1.	Best-case time complexity: O(n)
2.	Average-case time complexity: O(n)
3.	Worst-case time complexity: O(n)
 where n is the degree of the polynomial being evaluated.
Graph:
![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/8af056f0-2236-4b1e-9c02-03509f970dd3)
 















                                           PRACTICAL 4
Aim: To find time complexity of Truth Table function generator and to represent it through graph.

Description:
This C++ code generates and prints all possible combinations of "T" and "F" for a given length (up to 10), measuring the average time taken to generate these combinations and storing the results in a file named "data.txt."

Algorithm:
Boolean
1.	Define a function TT(x, k, n) to generate all possible truth table combinations for a Truth Table expression with n variables, where x[] is the array to store the current combination, k is the current index, and n is the total number of variables.
2.	If k equals n+1:
•	Print the current combination stored in the array x[].
3.	Else:
•	Set x[k] to 'T' and recursively call TT(x, k+1, n) to generate combinations with the current variable set to true.
•	Set x[k] to 'F' and recursively call TT(x, k+1, n) to generate combinations with the current variable set to false.

Time Complexity:
The time complexity for generating a truth table (T/F table) depends on the number of variables n in the boolean expression for which the truth table is being generated.
1.	Best-case time complexity: O(2^n)
2.	Average-case time complexity: O(2^n)
3.	Worst-case time complexity: O(2^n)
Here, n represents the number of variables in the boolean expression. The reason for the exponential time complexity is that a truth table for a boolean expression with n variables has 2^n rows, each representing a unique combination of truth values for the variables. Generating all these combinations requires exponential time as the number of variables increases.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/8ffcf147-1a50-4843-abdc-3f3a7b7f458b)














                                           PRACTICAL 5
Aim: To find time complexity of Sum of n numbers and to represent it through graph.

Description:
This C++ code measures the average time taken to compute the sum of elements in an array using recursion, for array sizes ranging from 13,000 to 99,000 in steps of 10,000. It generates random arrays, performs the sum calculation 10 times for each array size, and records the timing data in a file named "data.txt" while displaying the results on the console.

Algorithm:
Sum of n numbers
1.	Define a function sum(a, k) to calculate the sum of elements in an array up to index k, where a[] is the array of integers and k is the index.
2.	If k equals 1:
•	Return the value of the first element a[0].
3.	Else:
•	Return (a[k - 1] + sum(a, k - 1)), which is the sum of the current element a[k - 1] and the sum of elements up to index k - 1.


Time Complexity:
For sum of n numbers:
1.	Best-case time complexity: O(1)
2.	Average-case time complexity: O(n)
3.	Worst-case time complexity: O(n)
These complexities represent the time required to compute the sum of n numbers using recursion under different scenarios.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/6e72d0fb-d8df-41ed-a4f5-6befc3e018d0)

















                                                                              LAB 2
                                           PRACTICAL 1
Aim: To find time complexity of Binary Search and to represent it through graph.

Description:
This C++ code implements binary search on a sorted array of integers, measuring the average time taken to find a specified element in arrays of increasing sizes (from 10 to 990 elements in steps of 100). It generates random arrays, sorts them, performs binary search 10 times for each array size, displays the search results, and records the timing data in a file named "data.txt."

Algorithm:
Binary Search
1.	Define a function binary_search(a, low, high, el) to perform binary search on a sorted array a[] for the element el within the range [low, high].
2.	While low is less than high:
•	Calculate the middle index as mid = (low + high) / 2.
•	If el is less than the middle element a[mid], update high = mid - 1.
•	If el is greater than the middle element a[mid], update low = mid + 1.
•	If el is equal to the middle element a[mid], return mid as the index where el is found.
3.	If the element el is not found within the range [low, high], return an appropriate indication (e.g., -1 or another value that indicates not found).

Time Complexity:
For Binary search time complexities: 
1.	Best-case time complexity: O(1)
2.	Average-case time complexity: O(logn)
3.	Worst-case time complexity: O(logn)
These complexities demonstrate the efficiency of binary search, particularly in sorted lists, where it can quickly find elements with a logarithmic time complexity.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/7a4ba74f-016a-48ea-b352-4edc375e6619)






                                           PRACTICAL 2
Aim: To find time complexity of Power and to represent it through graph.

Description :
This C++ code calculates the power of a number using an optimized approach based on exponentiation by squaring. It measures the average time taken to compute the square of numbers from 1 to 199 in steps of 10, repeating the computation 10 times for each number and recording the timing data in a file named "data.txt" while displaying the results on the console.

Algorithm:
Power
1.	Define a function power(n, x) to calculate x^n, where n is the exponent and x is the base.
2.	Initialize a variable power to 1.
3.	While n is not equal to 0:
•	If n is even (n % 2 == 0):
I.	Update x = x * x (square x).
II.	Update n = n / 2 (divide n by 2).
•	If n is odd: 
I.	Update power = power * x (multiply power by x)
4.	Return the final value of power.

Time Complexity:
For Power function time complexities: 
1.	Best-case time complexity: O(1)
2.	Average-case time complexity: O(log2n)
3.	Worst-case time complexity: O(log2n)
These complexities demonstrate that the exponentiation by squaring algorithm is efficient, especially for large exponents, as it reduces the number of multiplications required compared to a naive approach.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/b5d1041b-257d-47cf-8f94-22764900e9c2)
















                                           PRACTICAL 3
Aim: To find time complexity of combining two sorted sort and to represent it through graph.

Description:
This C++ code implements a function to merge two sorted arrays into a third sorted array. It measures the average time taken to perform this operation for increasing array sizes (from 10,000 to 1,000,000 elements) and records the timing data in a file named "data.txt" while displaying the results on the console.

Algorithm:
Combining two sorted list
1.	Define a function sorted_list(list1, list2, n, m) to merge two sorted lists list1 and list2 of sizes n and m, respectively, into a sorted list list3.
2.	Initialize variables x = 0, y = 0, z = 0.
3.	Create an array list3 of size m + n to store the merged sorted list.
4.	While both x and y are less than their respective list sizes (x < n and y < m):
•	If list1[x] < list2[y]:
I.	Assign list3[z] = list1[x].
II.	Increment x and z by 1.
•	Else:
I.	Assign list3[z] = list2[y].
II.	Increment y and z by 1.
5.	After the above loop, if there are remaining elements in list1, copy them to list3.
6.	After the above loop, if there are remaining elements in list2, copy them to list3.

Time Complexity:
For combining 2 sorted lists:
1.	Best-case time complexity: O(m+n)
2.	Average-case time complexity: O(m+n)
3.	Worst-case time complexity: O(m+n)
This analysis demonstrates that the time complexity for combining two sorted lists using the merge approach is linear in the combined size of the lists (m+n).

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/c37247a0-7b8d-4513-a90e-2a2e625a404e)
















                                           PRACTICAL 4
Aim: To find time complexity of code for finding actual position and to represent it through graph.

Description:
This C++ code implements the partitioning step of the quicksort algorithm to arrange elements such that all elements smaller than a chosen pivot are placed before it, and all greater elements are placed after it. It measures the average time taken to perform this operation for increasing array sizes (from 1,000 to 100,000 elements) with randomly generated elements, recording the timing data in a file named "data.txt" and displaying the results on the console.

Algorithm:
To find actual position of number
1.	Define a function actual_pst(a, n, el) to rearrange the elements in an array a[] such that all elements less than el are before it, and all elements greater than el are after it. The function also returns the index of the first occurrence of el in the original array.
2.	Initialize variables grt = 0, sml = 0, indx_pst, t, fst = 0, last = n - 1, i, and j.
3.	Iterate through the array a[] from index 0 to n - 1:
•	If a[i] is less than el, increment sml.
•	If a[i] is greater than el, increment grt.
•	If a[i] is equal to el, set indx_pst to i.
4.	Swap a[indx_pst] with a[sml].
5.	Initialize fst = 0 and last = n - 1 for the partitioning process.
6.	While fst is less than last:
•	Iterate from fst to sml - 1:
•	Iterate from last to sml:
•	If fst is less than last, swap a[fst] with a[last].
7.	The function does not return any value (void).

Time Complexity:
For finding actual position:
1.	Best-case time complexity: O(nlogn)
2.	Average-case time complexity: O(nlogn)
3.	Worst-case time complexity: O(n^2)
These complexities describe the behavior of the actual_pst function in different scenarios based on the input array's arrangement around the pivot element el.

Graph:
![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/77e2c302-ce0e-49c1-a5d3-a3bd14b95a27)
 










                                                                              LAB 3
                                           PRACTICAL 1
Aim: To find time complexity of Merge Sort and to represent it through graph.	

Description:
This C++ code implements the merge sort algorithm and measures the average time taken to sort randomly generated arrays of increasing sizes (from 1 to 10,000 elements). It records the timing data in two separate files ("data.txt" and "data2.txt") for different scale factors, demonstrating the time complexity of merge sort as (O(nlogn)). Additionally, it includes a function (`complex()`) to calculate and write the time complexity data based on (nlog n) for comparison.

Algorithm:
Merge
1.	Calculate the sizes of the subarrays: n1 = mid - left + 1 and n2 = right - mid.
2.	Create temporary arrays L and R of sizes n1 and n2, respectively.
3.	Copy elements from the original array a[] to L and R.
4.	Merge the elements from L and R back into array a[] in sorted order.
MergeSort
1.	If low is less than high:
•	Calculate mid as (low + high) / 2.
•	Recursively call MergeSort for the left and right halves of the array: MergeSort(a, low, mid) and MergeSort(a, mid + 1, high).
•	Merge the sorted halves using the merge function.
Complex
1.	Calculate t as i * log(i).
2.	Write the pair (i, t) to a file using WriteToFile(i, t) function.

Time Complexity:
For merge sort :
1.	Best-case time complexity: O(nlogn)
2.	Average-case time complexity: O(nlogn)
3.	Worst-case time complexity: O(nlogn)
Merge Sort's consistent time complexity across different scenarios makes it a popular choice for sorting large datasets efficiently.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/c340e61e-2093-40e2-ad34-1ed0c313cc83)





                                           PRACTICAL 2
Aim: To find time complexity of Quick Sort and to represent it through graph.

Description:
This C++ code implements the quicksort algorithm and measures the average time taken to sort randomly generated arrays of increasing sizes (from 1 to 10,000 elements). It records the timing data in "data.txt" and "data2.txt" for different scale factors, showcasing the time complexity of quicksort as (O(n log n)). Additionally, it includes functions (`average()` and `worst()`) to calculate and write the time complexity data based on (n log n) and (n^2), respectively, for comparison.

Algorithm:
Partition
1.	Define a function Partition(a, low, high) to partition the array a[] into two halves around a pivot element.
2.	Initialize variables i = low, j = high, and p = a[low] (pivot).
3.	Use a do-while loop:
•	Increment I until a[i] greater than or equal to p.
•	Decrement j until a[j] is less than or equal to p.
•	If I is less than j, swap a[i] and a[j].
4.	Swap a[low] with a[j] to place the pivot in its correct sorted position.
5.	Return the index j, which represents the partition point.
Quick Sort
1.	Define a function QS(a, low, high) to recursively sort the array a[] using the Quick Sort algorithm.
2.	If low is less than high:
•	Call Partition(a, low, high) to get the partition index j.
•	Recursively call QS for the left subarray: QS(a, low, j - 1).
•	Recursively call QS for the right subarray: QS(a, j + 1, high).
Average
1.	Define a function average() to perform some operation, such as writing data to a file, based on the average-case scenario for Quick Sort.
2.	Iterate from 1 to 10000 in steps of 1000:
•	Calculate t as i * log(i).
•	Write the pair (i, t) to a file using WriteToFile(i, t) function.
Worst Case
1.	Define a function worst() to perform some operation, such as writing data to a file, based on the worst-case scenario for Quick Sort.
2.	Iterate from 1 to 10000 in steps of 1000:
•	Calculate t as (i * i) / 100.
•	Write the pair (i, t) to a file using WriteFile(i, t) function.

Time Complexity:
For quick sort:
1.	Best-case time complexity: O(nlogn)
2.	Average-case time complexity: O(nlogn)
3.	Worst-case time complexity: O(n2). 
Quick Sort is known for its efficiency and is widely used in practice due to its average-case time complexity of O(nlogn).

Graph:
![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/92a28607-5b8e-4eef-8e40-b014870cef37)


 












                                           PRACTICAL 3
Aim: To find time complexity of Maximum and minimum through iteration and merge sort and to compare it through graph.

Description:
This C++ code implements functions to find the maximum and minimum elements in an array using both recursive and iterative approaches. It measures the average time taken to find the maximum and minimum elements for array sizes ranging from 100 to 900 elements, repeating the process 10 times for each array size, and records the timing data in "data.txt" and "data2.txt" for analysis and comparison between the recursive and iterative methods.

Algorithm:
MaxMinIterative
1.	Define a function MaxMinIterative(a, low, high) to find the maximum and minimum elements in an array a[] iteratively.
2.	Initialize two nested loops to iterate through the array:
•	Outer loop from low to high.
•	Inner loop from i+1 to high.
3.	Compare each element a[i] with elements a[j] where j is greater than i.
4.	If a[i] is greater than a[j] , swap them to ensure that a[i] holds the minimum element among the elements from i to high.
5.	After iterating through the array, print the maximum element at index high and the minimum element at index low.
MaxMin
1.	Define a function MaxMin(a, low, high) to find the maximum and minimum elements in an array a[] recursively.
2.	Declare variables max, min, mid, max1, and min1.
3.	Check if low is equal to high, which indicates a single element in the array:
•	If true, set max and min to a[low] since it is both the maximum and minimum element.
4.	Otherwise, calculate the middle index mid as (low + high) / 2.
5.	Recursively call MaxMin for the left half of the array: MaxMin(a,low,mid).
6.	Check if low is equal to high again, now for the right half of the array:
•	If true, set max1 and min1 to a[low] since it is both the maximum and minimum element in this half.
7.	Recursively call MaxMin for the right half of the array: MaxMin(a,mid + 1, high). 
8.	Compare max with max1 and update max if max1 is greater.
9.	Compare min with min1 and update min if min1 is smaller.
10.	Print the maximum and minimum elements after the recursion completes.

Time Complexity:
Max and Min Iterative:
1.	Best-case time complexity: O(n)
2.	Average-case time complexity: O(n)
3.	Worst-case time complexity: O(n)
The iterative approach to find the maximum and minimum elements in an array has a linear time complexity, making it efficient for arrays of any size and arrangement.

Max and Min through Merge sort:
1.	Best-case time complexity: O(nlogn)
2.	Average-case time complexity: O(nlogn)
3.	Worst-case time complexity: O(nlogn)
Merge Sort's time complexity for finding the maximum and minimum elements is efficient across different scenarios, making it a reliable algorithm for sorting and related tasks.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/8b440c44-c63e-4dd9-ac9f-f142767ade78)















                                           PRACTICAL 4
Aim: To find time complexity of Matrix Multiplication through divide and conquer and to represent it through graph.

Description:
This C++ code implements matrix multiplication using the Strassen's algorithm and measures the average time taken for matrix multiplication of randomly generated square matrices of increasing sizes (from 2x2 to 256x256). It records the timing data in "data.txt" for analysis and includes a function (`complexity()`) to calculate and write the time complexity data based on ( n^3 ) for comparison.

Algorithm:
add_matrices Function:
1.	Parameters: Two matrices A and B.
2.	Returns: The sum of matrices A and B.
combine_matrices Function:
1.	Parameters: Four matrices C11, C12, C21, and C22.
2.	Returns: A combined matrix formed by arranging C11, C12, C21, and C22 in a block matrix form.
matrix_multiply Function:
1.	Parameters: Two matrices A and B.
2.	Returns: The product of matrices A and B using Strassen's algorithm.
3.	Steps:
•	If A is a 1x1 matrix, directly compute and return the product.
•	Otherwise, divide matrices A and B into submatrices A11, A12, A21, A22, B11, B12, B21, and B22.
•	Compute seven intermediate matrices P1 to P8 using recursive calls to matrix_multiply for submatrix products.
•	Compute four submatrices C11, C12, C21, and C22 using add_matrices and combine_matrices.
•	Return the combined matrix.
initialize_random_matrix Function:
1.	Parameters: A matrix c and its size.
2.	Action: Initializes the matrix c with random values.
complexity Function:
1.	Action: Calculates and writes to a file the size of matrices (i), which increases exponentially, and their corresponding complexity (n = i^3).


Time Complexity:
For Matrix Multiplication :
1.	Best-case time complexity: O(n^3)
2.	Average-case time complexity: O(n^3)
3.	Worst-case time complexity: O(n^3)
For small matrices, it is a better approach.
Graph:
![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/b9d5a93b-5540-456a-8fee-5001d86010e2)
 


                                           PRACTICAL 5
Aim: To find time complexity of Strassens Multiplication and to represent it through graph.

Description:
This C++ code implements matrix multiplication using the Strassen's algorithm, which is a divide-and-conquer approach to efficiently multiply matrices. It measures the average time taken for matrix multiplication of randomly generated square matrices of increasing sizes (from 2x2 to 256x256) and records the timing data in "data.txt" for analysis. Additionally, it includes a function (`complexity()`) to calculate and write the time complexity data based on ( n^2.81 ) for comparison.

Algorithm:
Divide the Matrices:
1.	Given two matrices A and B, divide them into four equal-size submatrices each:
•	A11, A12, A21, A22 for matrix A.
•	B11, B12, B21, B22 for matrix B.
Compute Intermediate Matrices:
1.  Calculate intermediate matrices X1 to X5 and Y1 to Y5 using additions and subtractions of submatrices as follows:
•	X1 = (A11 + A22)
•	X2 = (A21 + A22)
•	X3 = (A11 + A12)
•	X4 = (A21 - A11)
•	X5 = (A12 - A22)

•	Y1 = (B11 + B22)
•	Y2 = (B12 - B22)
•	Y3 = (B21 - B11)
•	Y4 = (B11 + B12)
•	Y5 = (B21 + B22)
Recursive Multiplications:
1.  Perform seven recursive multiplications (P, Q, R, S, T, U, V) using the intermediate matrices:
•	P = A11 * (B12 - B22)
•	Q = (A11 + A12) * B22
•	R = A11 * (B21 - B11)
•	S = A22 * (B11 + B12)
•	T = (A21 + A22) * B11
•	U = (A12 - A22) * (B21 + B22)
•	V = (A21 - A11) * (B11 + B12)
Compute Result Submatrices:
1.  Compute the result submatrices Z1 to Z4 using additions and subtractions of the recursive multiplications:
•	Z1 = P + S
•	Z2 = Z1 + V
•	Z3 = P + R
•	Z4 = Z3 + U
Combine Result Matrices:
1.  Combine the result submatrices to obtain the final result matrix C:
•	C11 = Z2 – T
•	C12 = R + T
•	C21 = Q + S
•	C22 = Z4 - Q


Time Complexity:
For Strassen Matrix:
1.	Best-case time complexity: O(n^2.81)
2.	Average-case time complexity: O(n^2.81)
3.	Worst-case time complexity: O(n^2.81)
The Strassen algorithm is generally more efficient than the naive approach for large matrices due to its reduced number of scalar multiplications, even though it has a higher exponent in its time complexity. However, for small matrices, the overhead of the Strassen algorithm may not provide a significant advantage over the naive approach.
Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/187d2230-55de-4cb4-ab8e-12e60dc0f7a0)















                                                                              LAB 4
                                           PRACTICAL 1
Aim: To find time complexity of Activity Selector and to represent it through graph.

Description:
This C++ code implements a scheduling algorithm using the Activity Selection (AS) algorithm. It generates random start times, finish times, and profits for activities, sorts them based on start and finish times, and then applies the AS algorithm to select a non-overlapping set of activities that maximize profit. The code measures the average time taken for this process across multiple iterations and records the results in a file.

Algorithm:
Sorting (Start) Function
1.	Define a function Sort_start(int s[],int n) for sorting the start array of every instance.
2.	Initialize array s[] to n size.
3.	Start outer loop from i = 0 to n-1.
•	Start inner loop from j=0 to n-i-1.
•	Compare s[j] with s[j+1].
	If s[j] > s[j+1], swap s[j] and s[j+1].
•	End Inner loop.
End Outer loop.
4.	Output: Sorted array s[] in ascending order.

Sorting (Finish) Functions
1.	Define a function Sort_finish(int f[],int n) for sorting the start array of every instance.
2.	Initialize array f[] to n size.
3.	Start outer loop from i = 0 to n-1.
•	Start inner loop from j=0 to n-i-1.
•	Compare f[j] with f[j+1].
	If f[j] > f[j+1], swap f[j] and f[j+1].
•	End Inner loop.
End Outer loop.
4.	Output: Sorted array f[] in ascending order.

Activity Selector
1.	Define a function AS(int a[], int s[], int f[], int n) for Activity Selector.
2.	Create a new array sol[] of size n to store the selected activities.
3.	Initialize i=0 and j=0.
4.	Set sol[0] = 0.
5.	Start a loop from j=1 to n-1.
•	Set sol[i]=0 (Initialize all other elements of sol[] to 0).
6.	Set sol[i] = a[i].
7.	Start another loop from j=1 to n-1.
•	Check if the start time of activity j (s[j]) is greater than or equal to the finish time of the last selected activity (f[i]).
•	If true, set sol[j] = a[j] (select activity j) and update i=j.
8.	End loops.

Time Complexity:
For activity selector:
1.	Best-case time complexity: O(n)
2.	Average-case time complexity: O(nlogn)
3.	Worst-case time complexity: O(nlogn)
The Activity Selection problem exhibits efficient time complexities, especially in the average and worst cases, due to the effectiveness of the greedy algorithm combined with sorting. However, the best-case time complexity is even better when the activities are already sorted.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/4e37e52e-c0ea-4428-888a-40be91d5a709)


 











                                          PRACTICAL 2
Aim: To find time complexity of Iterative QuickSort and to represent it through graph.

Description:
This C++ code implements an iterative version of the QuickSort algorithm using a stack for partitioning and sorting an array of integers. It generates random integer arrays of increasing sizes, applies QuickSort iteratively for 10 iterations on each array, measures the average time taken, and records the results in a file for analysis.

Algorithm:
Swap 
1.	Define a function Swap(a,b) for Swapping.
2.	Set temp to the value of a.
3.	Set a to the value of b.
4.	Set b to the value of temp.
Partition
1.	Define a function Partition(a, low, high) for partition in Quick Sort.
2.	Set i to low.
3.	Set j to high.
4.	Set p to a[low] (pivot element).
5.	Do the following until I is less than or equal to j:
•	Increment i until a[i] is greater than or equal to p.
•	Decrement j until a[j] is less than or equal to p.
•	If I is less than j, swap a[i] and a[j].
6.	Swap a[low] and a[j] (place pivot in correct position).
7.	Return j.(index of pivot element).
Quick Sort Iterative
1.	Define a function QuickSortIterative(a, low, high) for Iterative Quick Sort.
2.	Create an empty stack.
3.	Push low onto the stack.
4.	Push high onto the stack.
5.	While the stack is not empty, do the following:
•	Pop high from the stack.
•	Pop low from the stack.
•	Call Partition(a, low, high) and store the result in pivotIndex.
•	If pivotIndex – 1 is greater than low, push low and pivotIndex -1 onto the stack.
•	If pivotIndex + 1 is less than high, push pivotIndex + 1and high onto the stack.

Time Complexity:
For Iterative Quicksort:
1.	Best-case time complexity: O(nlogn)
2.	Average-case time complexity: O(nlogn)
3.	Worst-case time complexity: O(n2)
Efficient pivot selection strategies, such as choosing a random pivot or using the "median-of-three" approach, can help mitigate the risk of worst-case behavior and improve the average-case performance of Quick Sort.

Graph:
![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/d2bc19f0-58ec-4dfc-b128-4c03bb12ecdf)
 
                                           PRACTICAL 3
Aim: To find time complexity of KnapSack and to represent it through graph.

Description:
This C++ program implements a knapsack algorithm with three different strategies: sorting by profit, sorting by weight, and sorting by profit-to-weight ratio. It generates random profit and weight values for items, sorts them based on the selected strategy, and calculates the average time taken to solve the knapsack problem for each strategy over multiple iterations. The results are then written to separate files for analysis.

Algorithm:
Sort_profits
1.	Define a function sort_profit(p, w, n) for sorting according to profit in descending order.
2.	Loop i from 0 to n-1
•	Loop j from 0 to n-i-1:
o	If p[j] < p[j+1], do the following:
	Swap p[j] and p[j+1].
	Swap w[j] and w[j+1].
Sort_weight
1.	Define a function sort_weight(p, w, n) for sorting according to weight ascending .
2.	Loop i from 0 to n-1
3.	Loop j from 0 to n-1
o	If w[j] > w[j+1], do the following:
	Swap p[j] and p[j+1].
	Swap w[j] and w[j+1].
Sort_profit_weight
1.	Define a function sort_profit_weight(p, w, n) for sorting according to profit weight ratio in descending .
2.	Loop i from 0 to n-1
•	Loop from 0 to n-i-1
o	Calculate ratio_i = p[i] /w[i] and ratio_j = p[j]/w[j].
o	If ratio_i is greater than ratio_j, do the following:
	Swap p[i] and p[j].
	Swap w[i] and w[j].
Knapsack
1.	Define a function Knapsack(n, max, p, w).
2.	Set max_profit to max.
3.	Create an array Sol of size n and initialize all elements to 0.
4.	Loop i from 0 to n-1
•	Set Sol[i] to 0.
5.	Loop i from 0 to n-1
•	If w[i] is less than max_profit, do the following:
o	Set Sol[i] to 1.
o	Reduce max_profit by w[i].
•	Else, break out of the loop.
6.	If I is less than n, set  Sol[i] to max_profit divided by w[i]. 

Time Complexity:
For Knapsack:
1.	Best-case time complexity: O(1)
2.	Average-case time complexity: O(nW)
3.	Worst-case time complexity: O(nW)
Where n is the number of items and W is the capacity of the knapsack. This time complexity is efficient and practical for moderate-sized instances of the problem, but it can become prohibitive for very large n or W due to the polynomial nature of the complexity.
Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/04c80a22-b8c1-48a4-9366-ffd008312d65)

















                                                                              LAB 5
                                           PRACTICAL 1
Aim: To find time complexity of Shortest Distance (Dijkstra) and to represent it through graph.

Description:
This C++ program implements the Single-Source Shortest Path (SSSP) algorithm using Dijkstra's approach. It generates random cost values for edges in a graph and calculates the shortest paths from a source vertex to all other vertices. The average time taken to perform the SSSP algorithm over multiple iterations for varying graph sizes is computed and written to a file for analysis.

Algorithm:
Shortest Distance (Dijkstra)
1.	Define a function sssp(n, cost, v, dist) for finding the shortest distance from each point.
2.	Loop i from 1 to n
•	Set cost[v,i] to dist[i].
•	Set s[i] to False. (To add the vertex in non visited list).
3.	S[v] = T (To add the vertex in visited list).
4.	Dist [v] = 0
5.	Loop  j from 2 to n-1
•	Choose a vertex u such that s[u] is in non visited list and dist[u] is minimum.
•	Move s[u] in visited list.
•	Loop w from 0 to n
o	If all w are neighbours of u and dist[w] is greater than sum of dist[u] and cost[u][w]
•	Set dist[w] to sum of dist[u] and cost[u][w]
6.	Return dist().

Time Complexity:
For Shortest Distance (Dijkstra):
1.	Best-case time complexity: O(n)
2.	Average-case time complexity: O(n2)
3.	Worst-case time complexity: O(n2)
The time complexity analysis helps understand how the algorithm's performance varies based on the characteristics of the input graph. Efficient implementations of shortest path algorithms often aim to achieve better-than-average-case performance, especially for large or dense graphs.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/0a6ec8b4-85ed-43e8-a86f-62146d7c1419)















                                           PRACTICAL 2
Aim: To find time complexity of Prims Algorithm and to represent it through graph.

Description:
This C++ program implements Prim's algorithm for finding the Minimum Spanning Tree (MST) of a graph. It generates random cost values for edges in the graph, applies Prim's algorithm multiple times to calculate the average time taken for varying graph sizes, and writes the results to a file for analysis.

Algorithm:
Prims
1.	Define a function prims(cost,n,t) for finding the shortest distance from each vertex.
2.	Let (k,l) be the edge with minimum weight.
3.	Set minimum to cost[k,l].
4.	Loop i from 1 to n
•	If cost[i,k] is less than cost[i,l]
o	Set near[i] = k
•	Else 
o	Set near[i] = l
5.	Set near[k] and near[l] to 0.
6.	Loop j from 1 to n-1
•	Loop i from 0 to n
o	If near[i] is not equals to zero and cost[i][near[i]] is less than mincost
	Set u to i
	Set mincost to cost[i][near[i]].
•	Set t[j][0] to 0
•	Set t[j][1] to near[u]
•	Set near[u] to 0
•	Loop k from 0 to n
o	If near[k] is not equals to zero and cost[k][near[k]] is greater than cost[u][k]
	Set near[k] to u.


Time Complexity:
For Prims algorithm:
1.	Best-case time complexity: O(V)
2.	Average-case time complexity: O(ElogV) or O(V2) (depending on implementation and data structures)
3.	Worst-case time complexity: O(V2) or O(ElogV) (depending on implementation and data structures)
Efficient implementations of Prim's algorithm aim to achieve better-than-average-case performance, especially for dense graphs where the worst-case time complexity can be significant. Using appropriate data structures like priority queues can significantly improve the algorithm's performance.

Graph:
![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/0a407432-9804-42c4-a2fc-5b11ff18cee4)

 

  












                                         PRACTICAL 3
Aim: To find time complexity of Kruskal Algorithm and to represent it through graph.

Description:
This C++ program implements Kruskal's algorithm to find the Minimum Spanning Tree (MST) of a graph. It generates random edges with weights, applies Kruskal's algorithm multiple times for different graph sizes, calculates the average time taken, and writes the results to a file for analysis. The program uses a union-find data structure and a min-heap to efficiently process edges and construct the MST.

Algorithm:
Find Function
1.	Define a function find(p,i) for finding next vertex.
2.	Recursively find the parent until reaching a vertex whose parent is itself (indicating the root of the set).
3.	Output: The parent of the set containing vertex i.
Union Function
1.	Define a function unionSets (p,x,y) for union of vertexes.
2.	Find the parents of x and y, and set the parent of one as the other to merge the sets.
Heapify Function
1.	Define a function heapify (edges,i,n) for heapify of heap.
2.	Initialize left as ‘2i + 1’, right as ‘2i + 2’and smallest as ‘i’.
3.	If left is less than n and edges[left] is less than edges[smallest].
•	Set smallest to left.
4.	If right is less than n and edges[right] is less than edges[smallest].
•	Set smallest to right.
5.	If smallest is not equals to i
•	Swap(edges[i], edges[smallest])
•	Heapify(edges,smallest,n)
Build Heap Function
1.	Define a function buildheap(edges, n) for building a heap.
2.	Loop i from n/2 -1 to 0
•	Heapify(edges, i, n)
Kruskal’s Algorithm Function 
1.	Define a function Kruskal(edges, n, numVertices, result) for finding minimum cost.
2.	Build a min-heap using buildHeap.
3.	Loop i from 0 to numVertices 
4.	Initialize edgeCount to 0.
5.	Start While loop till edgeCount is less than numVertices -1 and n is greater than 0
•	Loop i from 0 to 3
o	Set edge[i] to edges[0][i]
o	swap(edges[0], edges[n-1])
•	Swap(edges[0], edges[n-1])
•	Decrement n by 1.
•	Heapify(edges, 0, n)
•	Initialize srcp to find(p,edges[0])
•	Initialize destp to find(p,edges[1])
•	If srcp is not equal to destp
o	Loop i from 0 to 3
	Set result[edgeCount][i] to edge[i].
•	Increment edgeCount by 1
•	unionSets(p,srcp,destp)
 
Time Complexity:
For Kruskals Algoritm:
1.	Best-case time complexity: O(ElogE)
2.	Average-case time complexity: O(ElogE) or O(ElogV) (depending on implementation and data structures)
3.	Worst-case time complexity: O(ElogE) or O(ElogV) (depending on implementation and data structures)
Efficient implementations of Kruskal's algorithm use a sorted edge list or a priority queue to process edges efficiently, leading to better-than-average-case performance in practice. Additionally, using optimized disjoint-set data structures can further improve the algorithm's time complexity.

Graph:
 ![image](https://github.com/Diksha0416/ADA_LAB-UE223026-/assets/134716037/2e469dda-1f60-4d58-be7f-b7c6308dd87d)





             LAB 6
                                           PRACTICAL 1
Aim: To calculate the minimum cost to reach from a source point to the other point in multistage graph. 

Description:
A multistage graph is a directed graph where the nodes are divided into multiple stages, and edges only connect nodes from one stage to the next. It's often used to model problems involving a sequence of decisions or actions, such as production processes or project planning, where each stage represents a distinct phase or step. Algorithms like Dijkstra's or dynamic programming are commonly used to solve optimization problems on multistage graphs.

Algorithm:
1. Stage Function (stage):
•	This function recursively calculates the number of stages in the DAG starting from a given node i. It increments the count parameter for each recursive call until it reaches the last node (n - 1), where it returns the count.

2. Find Function (find_fun):
•	This function is used to find the minimum cost edge from node j to other nodes in the graph. It iterates over the edges starting from j + 1 and calculates the minimum cost using the fcost array.

3. FCost Function (fcost):
•	This function calculates the minimum cost and the path for a given number of stages (k) in the DAG.
•	It initializes arrays d and fcost to store intermediate results.
•	It starts from the second-to-last node (n - 2) and uses the find_fun function to compute the minimum cost for each node.
•	It then constructs the path (p) based on the minimum cost values.

4. Main Function:
•	In the main function, a sample DAG represented by an adjacency matrix (graph) is defined.
•	It calculates the number of stages in the DAG using the stage function and prints it.
•	It then calls the fcost function to find the minimum cost and path for a specified number of stages (k).

Time Complexity:
For the multistage graph algorithm:
1.	Best-case time complexity: O(V + E) + O(V^2) ≈ O(V^2) for sparse graphs.
2.	Average-case time complexity: O(V + E) + O(V^2) ≈ O(V^2) for typical graphs.
3.	Worst-case time complexity: O(V + E) + O(V^2) ≈ O(V^2) for dense graphs.



                                           PRACTICAL 2
Aim: All pair shortest path.

Description:
The All-Pairs Shortest Path (APSP) algorithm calculates the shortest path between all pairs of vertices in a weighted graph. It's commonly solved using algorithms like Floyd-Warshall or Johnson's algorithm. Floyd-Warshall has a time complexity of O(V^3) where V is the number of vertices, making it suitable for dense graphs and small to medium-sized graphs. Johnson's algorithm is more efficient for sparse graphs with a time complexity of O(V^2 log V + VE), where E is the number of edges, but it requires non-negative edge weights.

Algorithm
:
1. Initialization:
•	Initialize an adjacency matrix graph representing the weighted edges between vertices. Use a large value (INF) to represent infinity or absence of an edge.
•	Initialize matrices dist and pred of size VxV to store the shortest distances and predecessor vertices for each pair of vertices.
•	Initialize dist[i][j] with the weight of the edge between vertex i and j, and set pred[i][j] = i if there is an edge, otherwise set pred[i][j] = -1.

2. Floyd-Warshall Algorithm:
•	Iterate through all vertices (k) and for each pair of vertices (i, j):
•	If there exists a shorter path from vertex i to j through vertex k, update dist[i][j] and pred[i][j].
•	Update dist[i][j] to dist[i][k] + dist[k][j] if it's smaller than the current value.
•	Update pred[i][j] to the predecessor vertex on the shortest path.

4. Printing Shortest Paths:
•	After running the algorithm, iterate through all pairs of vertices (i, j) and print the shortest distance from i to j and the corresponding path using the printPath function.

Time Complexity: 
For the All-Pairs Shortest Path (APSP) algorithm using Floyd-Warshall:
1.	Best-case time complexity: O(V^2) (V is the number of vertices) for sparse graphs.
2.	Average-case time complexity: O(V^3) (V is the number of vertices) for typical graphs.
3.	Worst-case time complexity: O(V^3) (V is the number of vertices) for dense graphs.



                                           PRACTICAL 3
Aim: Write a program for assembly line program.

Description:
The assembly line scheduling problem involves optimizing the production process in a manufacturing environment with multiple assembly lines. It typically aims to minimize the total time or cost of production while meeting various constraints such as resource availability, capacity limits, and production sequence requirements. This problem is often solved using dynamic programming or other optimization techniques tailored to specific production line configurations and constraints.

Algorithm:
1.	Initialization:
•	Initialize arrays f1, f2, l1, and l2 to store the earliest possible time to finish on each line and the line used at each stage.
•	Set f1[0] = e1 + a[0][0] and f2[0] = e2 + a[1][0] as the entry times for the first stations on lines 1 and 2, respectively.
2.	Dynamic Programming Loop:
•	Iterate through the remaining stations (j = 1 to n - 1):
•	Calculate f1[j] and l1[j] using the recurrence relation based on the minimum time from the previous station on line 1 or transferring from line 2.
•	Calculate f2[j] and l2[j] similarly for line 2.
•	Choose the minimum time between line 1 and line 2 for each station.
3.	Final Calculation:
•	Compare the finish times at the last station with the exit times (x1, x2) to determine the overall minimum time (fstar) and the line used at the last station (lstar).
4.	Output:
•	Print the minimum time (fstar) as the result.
•	Print the assembly path by tracing back through the lines from the last station using the lstar, l1, and l2 arrays.

Time Complexity: 
The time complexity analysis for the assembly line scheduling algorithm is as follows:
1.	Best-case time complexity: O(n), where n is the number of stations. This is because the algorithm involves a single pass through the stations, performing constant-time operations at each station.
2.	Average-case time complexity: O(n), similar to the best-case scenario, as the algorithm's performance is primarily determined by the number of stations and the constant-time operations within each iteration.
3.	Worst-case time complexity: O(n), which occurs when there are many stations. In this case, the algorithm still performs a single pass through all stations, resulting in a linear time complexity relative to the number of stations.



                                           PRACTICAL 4
Aim: To find the longest common subsequence between two strings using dynamic programming.

Description:
The Longest Common Subsequence (LCS) algorithm using dynamic programming finds the longest subsequence shared between two strings. It creates a matrix to store intermediate results, filling it by comparing characters in the strings. The algorithm then traces back through the matrix to reconstruct the LCS. Its time complexity is O(m*n), where m and n are the lengths of the input strings.

Algorithm:
1.	Initialization:
•	Initialize a 2D array L[m+1][100] to store the lengths of LCSs for substrings of X and Y.
•	Initialize the first row and column of L with zeros, as LCS with an empty string is zero.
2.	Dynamic Programming Loop:
•	Iterate through the substrings of X and Y using nested loops.
•	If the characters at the current positions in X and Y match, increment L[i][j] by 1.
•	Otherwise, set L[i][j] to the maximum of L[i-1][j] and L[i][j-1], as LCS can be formed by skipping characters in either string.
3.	Backtracking for LCS:
•	Using the computed L array, backtrack to reconstruct the LCS by following the arrows (left, up, or diagonal) based on the values in L.
4.	Print LCS with Arrows:
•	Print the LCS along with arrows (<- or ^|) to indicate the direction of backtracking.
5.	Main Function:
•	Initialize strings S1 and S2.
•	Call the lcs function to compute the length of the LCS and print the LCS with arrows.

Time Complexity: 
The time complexity of the Longest Common Subsequence (LCS) algorithm using dynamic programming can be summarized as follows:
1.	Best-case time complexity: O(m * n), where m and n are the lengths of the input strings X and Y, respectively. This occurs when the strings have no common characters, leading to a trivial LCS of length zero.
2.	Average-case time complexity: O(m * n), where m and n are the lengths of the input strings X and Y, respectively. This average complexity is typical for most cases where the strings have varying lengths and share some common characters.
3.	Worst-case time complexity: O(m * n), where m and n are the lengths of the input strings X and Y, respectively. This worst-case scenario occurs when the LCS spans the entire lengths of both strings, resulting in the dynamic programming table being filled completely.



                                                                              LAB 7
                                           PRACTICAL 1
Aim: Knapsack using dynamic programming.

Description:
The Knapsack problem using dynamic programming (DP) optimally selects items to maximize value within a weight limit. It fills a matrix based on item weights and values, computing optimal values for different weight capacities. The algorithm then backtracks to determine which items were selected. Its time complexity is O(n*W), where n is the number of items and W is the knapsack capacity.

Algorithm:

1. Initialization:
•	Create a 2D vector K of size (n+1) * (W+1) to store the maximum values for different weights and items.

2.Dynamic Programming Loop:
•	Iterate through all items and weights using nested loops.
•	If the weight of the current item is less than or equal to the current weight limit, update K[i][w] to the maximum value between adding the current item's value to the maximum value obtained so far with the remaining weight (K[i-1][w - wt[i-1]]) and not adding the current item (K[i-1][w]).
•	If the weight of the current item exceeds the weight limit, set K[i][w] to the value obtained without including the current item (K[i-1][w]).

3. Backtracking for Solution:
•	After filling the K matrix, backtrack to find the selected items that contribute to the maximum value.
•	Start from K[n][W] and move upwards, checking if the value differs from the value in the row above (K[i-1][w]). If it differs, include the item in the solution and move to the previous row and reduced weight (w - wt[i-1]).

4. Print Solution:
•	Print the selected items that maximize the value of the knapsack.

5. Main Function:
•	Initialize vectors for values (val) and weights (wt).
•	Specify the knapsack weight limit (W).
•	Call the knapsackDP function to compute the maximum value and print the selected items.

Time Complexity:
1.	Best-case time complexity: O(n*W), where n is the number of items and W is the maximum capacity of the knapsack.
2.	Average-case time complexity: O(n*W), typical for most inputs.
3.  Worst-case time complexity: O(n*W), which occurs when the knapsack capacity is large compared to the number of items.





                                           PRACTICAL 2
Aim: Write a program for minimizing the scalar matrix multiplications.

Description: 
The algorithm for minimizing scalar matrix multiplication using dynamic programming involves finding the optimal order of multiplying matrices to minimize the total scalar multiplications. It creates a matrix to store intermediate results and computes the minimum cost recursively. The time complexity is O(n^3), where n is the number of matrices.

Algorithm:

1. Initialization:
•	Create a 2D array m[n][n] to store the minimum number of multiplications for multiplying matrices.
•	Create a 2D array brac[5][5] (using fixed size for demonstration) to store information about the optimal placement of parentheses for matrix multiplication.
2. Base Case:
•	Set m[i][i] = 0 for all diagonal elements, representing the base case where a single matrix multiplication requires no additional multiplications.
Dynamic Programming Loop:
•	Use nested loops to fill the m array diagonally.
•	Iterate over different chain lengths L (from 2 to n, where n is the number of matrices).
•	For each chain length, iterate over all possible starting indices i.
•	Compute the minimum number of multiplications m[i][j] required to multiply matrices from index i to j using a third index k as a split point.
•	Update m[i][j] and brac[i][j] if a better (minimum) number of multiplications is found.
3. Optimal Parenthesization:
•	Use a recursive function printParenthesis to print the optimal placement of parentheses for matrix multiplication based on the information stored in the brac array.
4. Main Function:
•	Initialize an array arr with the dimensions of matrices.
•	Call the MatrixChainOrder function to compute the minimum number of multiplications and print the optimal parenthesization.

Time complexity:
Therefore, the time complexity of the Matrix Chain Multiplication algorithm using dynamic programming is:
1.	Best-case time complexity: O(n^3)
2.	Average-case time complexity: O(n^3)
3.	Worst-case time complexity: O(n^3)



                                           PRACTICAL 3
Aim: Write a program N-Queens.

Description:
The N-Queens problem algorithm using backtracking involves placing N queens on an N×N chessboard such that no two queens threaten each other. It recursively explores possible placements and backtracks when a conflict is encountered. 

Algorithm:
1.	Function place(k, i)
•	Inputs: k represents the current row being considered, and i represents the column to be checked for placing a queen.
•	Output: Returns true if a queen can be placed at position (k, i) without conflicting with previously placed queens, false otherwise.
•	Iterate over all previously placed queens (from 1 to k-1) and check if the current position conflicts with any of them:
•	If the current position is in the same column as a previous queen (x[j] == i), or
•	If the current position is in the same diagonal as a previous queen (abs(x[j] - i) == abs(j - k)), indicating a diagonal conflict.
•	Return true if no conflicts are found, indicating that a queen can be placed at the current position without attacking other queens.
2.	Function Nqueens(k, n)
•	Inputs: k represents the current row being processed, and n is the total number of rows/columns (size of the chessboard).
•	Recursively attempts to place queens on each row starting from row 1 up to row n.
•	For each row, iterates over all columns (from 1 to n) and checks if placing a queen at that position is valid using the place function.
•	If a valid position is found (place(k, i) returns true), marks that position as a queen (x[k] = i) and recursively calls Nqueens(k + 1, n) to move to the next row.
•	If all queens are successfully placed (k == n), prints the arrangement of queens as a solution.
•	Backtracks by undoing the placement of the queen and exploring other positions if no valid position is found for a given row.
3.	Main Function:
•	Takes input for the number of queens (n).
•	Calls the Nqueens function to start the recursive search for solutions.
•	Prints solutions found during the recursive search.

Time Complexity:
For the N-Queens problem algorithm using backtracking, the time complexity is as follows:
1.	Best-case time complexity: O(1) when the solution is found quickly (rare in practice).
2.	Average-case time complexity: O(n!) for typical scenarios where backtracking explores various possibilities.
3.	Worst-case time complexity: O(n!) when backtracking explores all possibilities extensively.




                                                                              LAB 8
                                           PRACTICAL 1
Aim: Write a program Knapsack using backtracking.

Description:
The Knapsack problem using backtracking involves finding the optimal combination of items to maximize the value while respecting a weight constraint. It explores different combinations recursively, making decisions at each step based on whether adding an item is feasible and improves the total value. It backtracks when a dead-end is reached, optimizing the selection process for efficiency.

Algorithm:
1. Function print(s):
•	Print the elements of the set.
2. Function find_max_value(s):
•	Find the maximum value (first element) in the set.
3. Function find_max_path(s, max_value, p, w):
•	Find the path of items that contribute to the maximum value.
•	Iterate through the set and select items that contribute to the maximum value without exceeding weight constraints.
4. Function merge_purge(s1, s2, W):
•	Merge two sets while purging elements that violate weight constraints.
•	Iterate through elements of both sets, checking weight constraints and maximizing value.
5. Function knapsackMP(n, p, w, W):
•	Initialize an empty set s1 with a single element {0, 0}.
•	Iterate through each item:
•	Create a new set s2 by adding the current item to each element of s1.
•	Merge s1 and s2 while purging elements violating weight constraints.
•	Print the resulting set s1.
•	Find the maximum value in s1 using find_max_value.
•	Find the path of items contributing to the maximum value using find_max_path.
•	Print the maximum value and the selected items contributing to it.
6. Main Function:
•	Initialize input variables (number of items n, values p, weights w, and knapsack capacity W).
•	Call knapsackMP with the input parameters.

Time complexity:
For the N-Queens problem algorithm using backtracking, the time complexity is as follows:
1.	Best-case time complexity: O(1) when the solution is found quickly (rare in practice).
2.	Average-case time complexity: O(n2) for typical scenarios where backtracking explores various possibilities.
3.	Worst-case time complexity: O(n2) when backtracking explores all possibilities extensively.
The O(2n) complexity arises because backtracking explores both including and excluding each item in the knapsack, leading to an exponential number of subproblems and choices. However, pruning techniques like memoization or dynamic programming can improve the average-case performance significantly in practice.




                                           PRACTICAL 2
Aim: Write a program for coloring m nodes using backtracking.

Description:
Coloring m nodes involves assigning colors to a graph's nodes such that no two adjacent nodes share the same color, using a maximum of m colors. The algorithm recursively explores possible color assignments, backtracking when conflicts arise until a valid coloring or a failure is reached. It optimizes the coloring process by making efficient color choices and exploring different possibilities.

Algorithm:
1. Define Global Variables:
•	Create a global array x to store colors for vertices. Initialize all elements to 0 initially.
•	Set a constant infinity to represent an invalid color.
2. Define Functions: 
a. nextval(k, n, m, G):
•	Increment the color of vertex k by 1 (x[k] = (x[k] + 1) % (m + 1)).
•	If the color becomes 0 (meaning all colors have been tried), return.
•	Check if the new color conflicts with adjacent vertices:
•	For each vertex i connected to k (i.e., G[k][i] != 0), if x[i] == x[k], there is a conflict. In this case, break the loop.
•	If no conflicts are found, continue the loop.
          b. mcoloring(k, G, n, m):
•	Call nextval(k, n, m, G) to assign colors to vertex k.
•	If x[k] becomes 0 (no valid color found), return.
•	If all vertices are colored (k == n), print the colors in x and return.
•	Otherwise, recursively call mcoloring(k + 1, G, n, m) to color the next vertex.
3. Main Function:
•	Initialize the graph G, number of vertices n, and number of colors m.
•	Call mcoloring(0, G, n, m) to start coloring the vertices.

Time Complexity:
Time complexity for coloring m nodes:
1.	Best-case Time Complexity: O(m^n)
2.	Average-case Time Complexity: O(m^n * n^2)
3.	Worst-case Time Complexity: O(m^n * n^2)



                                           PRACTICAL 3
Aim: Write a program for finding sum of subsets using backtracking.

Description:
The Sum of Subsets problem using backtracking involves finding all subsets of a given set whose elements sum up to a specified target sum. The algorithm explores different combinations of elements, tracking the current sum and including or excluding elements to meet the target sum. It backtracks when a subset exceeds the target sum or when all possibilities are exhausted, efficiently exploring only promising paths.

Algorithm:
  1. Initialize arrays w[] (weights), x[] (solution vector), and variables m (target sum), n   (size of the array), r (sum of all elements).
  2. Define the function sumofsubsets(s, k, sum):
    a. Set x[k] = 1, representing including the k-th element in the subset.
    b. If the current sum s + w[k] equals the target sum m, print the subset and backtrack.
    c. Else, if including the next element (w[k + 1]) along with the current sum is still within the target sum (s + w[k] + w[k + 1] <= m), recursively call sumofsubsets with updated parameters.
    d. Set x[k] = 0, representing excluding the k-th element in the subset.
    e. If excluding the k-th element keeps the sum within the target range and there are more elements to consider, recursively call sumofsubsets with updated parameters.
  3. In the main function:
    a. Input the size of the array n and the target sum m.
    b. Input the array elements w[] and calculate the total sum r.
    c. Call sumofsubsets(0, 0, r) to start the backtracking process from the first element with an empty subset and the total sum.
    
Time complexity:
The time complexity of the Subset Sum problem solved using backtracking can be summarized as follows:
1.	Best-case time complexity: O(2^n) when the target sum is achieved early in the search tree, resulting in a quick solution.
2.	Average-case time complexity: O(2^n) for typical scenarios where the search explores various branches of the search tree before finding a solution.
3.	Worst-case time complexity: O(2^n) when the search tree is fully explored, considering all possible subsets.
