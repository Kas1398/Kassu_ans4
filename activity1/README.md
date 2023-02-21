# Activities

## Task 1

- Refer to the following link. Discuss how Merge-sort works:
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Sorting/mergesortAV.html

Ans:
  - Merge sort is a sorting algorithm that works by dividing an array into smaller subarrays, sorting each subarray, and then merging the sorted subarrays back together to form the final sorted array.

- Merge-sort Practice. Refer to the following link. Merge the two sub-arrays into the larger array.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Sorting/MergesortMergePRO.html

## Task 2

- Refer to the following link. Discuss how Quick-sort works:  
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Sorting/quicksortAV.html
- Quick-sort Practice. Refer to the following link. Partition the array using quicksort.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Sorting/QuicksortPartitPRO.html

  Ans: 
    - Quicksort is one of the most efficient sorting algorithms. It works by breaking an array (partition) into smaller ones and swapping (exchanging) the smaller ones, depending on a comparison with the 'pivot' element picked.

## Task 3

- The following snippet is from `./src/quicksort.cpp` lines 32-43. Discuss in groups how the code works:

```cpp
void quickSort(int arr[], int low, int high)
{
    if (low < high)
    {
        //partition the array
        int pivot = partition(arr, low, high);

        //sort the sub arrays independently
        quickSort(arr, low, pivot - 1);
        quickSort(arr, pivot + 1, high);
    }
}
```
Answer:
    - The swap function is a utility function that takes two integer pointers and swaps their values.
The partition function takes an array 'arr', a lower index 'low', and a higher index 'high'. It selects the last element in the array as the pivot and partitions the array into two parts. The left part contains elements smaller than or equal to the pivot, and the right part contains elements greater than the pivot. It returns the index of the pivot.
The 'quickSort' function takes an array 'arr', a lower index 'low', and a higher index 'high'. It recursively partitions the array using the partition function and sorts the subarrays independently. It stops when the subarray has only one element.

- The following snippet is from `./src/quicksort.cpp` line 27. Discuss in groups how ìt works:

```cpp
swap(&arr[i + 1], &arr[high]);
```

## Task 4: Individual (at home)

1. Merge-sort has better worst case performance than quicksort. So why Quick-sort is considered better than Merge-sort? Refer to the following article
   https://www.geeksforgeeks.org/quicksort-better-mergesort/

Answer:
    - Auxiliary Space : Mergesort uses extra space, quicksort requires little space and exhibits good cache locality. 

    -The worst case of quicksort O(n2) can be avoided by using randomized quicksort.

    - Merge sort is better for large data structures: Mergesort is a stable sort, unlike quicksort and heapsort, and can be easily adapted to operate on linked lists and very large lists stored on slow-to-access media such as disk storage or network attached storage.


2. Refer to the following article. Analyze the complexity of the Merge-sort algorithm.
   https://www.softwaretestinghelp.com/merge-sort/

   Answer:
        - The time complexity for merge sort is the same in all three cases (worst, best and average) as it always divides the array into sub-arrays and then merges the sub-arrays taking linear time.
        - Merge sort uses the “divide and conquer” strategy which divides the array or list into numerous sub arrays and sorts them individually and then merges into a complete sorted array.

3. Refer to the following article. Analyze the complexity of the Quick-sort algorithm.
   https://www.softwaretestinghelp.com/quick-sort/

   Answer: 
        - Quicksort is faster and works efficiently for sorting data structures. Quicksort is a popular sorting algorithm and sometimes is even preferred over merge sort algorithm.
