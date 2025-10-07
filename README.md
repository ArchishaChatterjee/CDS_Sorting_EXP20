# Experiment 20: Sorting Algorithms in C++

---

## Aim
To understand and implement different **Sorting Algorithms** in C++ and compare their logic and performance.  
Specifically:
1. **Bubble Sort**  
2. **Quick Sort**  
3. **Selection Sort**

---

## Tools
- **Programming Language**: C++  
- **Compiler**: g++ / MinGW / Turbo C++  
- **IDE/Editor**: Code::Blocks, Dev C++, or Visual Studio Code  
- **Operating System**: Windows / Linux / macOS  

---

## Theory
Sorting is the process of arranging data in a particular order (ascending or descending).  
Efficient sorting improves the performance of searching and other algorithms.  

Different sorting algorithms use different strategies to organize data, and each has unique advantages and limitations in terms of **time complexity**, **space usage**, and **stability**.

---

### 1. Bubble Sort
Bubble Sort is a **simple comparison-based algorithm** that repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order.  
Each iteration “bubbles” the largest element to the end of the array.

**Characteristics:**
- Easy to implement.  
- Inefficient for large datasets.  

**Time Complexity:**  
- Best Case: O(n)  
- Average Case: O(n²)  
- Worst Case: O(n²)

---

### 2. Quick Sort
Quick Sort is a **divide-and-conquer algorithm**.  
It selects a pivot element, partitions the array into two sub-arrays such that elements smaller than the pivot go to one side, and larger elements to the other.  
Then, it recursively sorts the sub-arrays.

**Characteristics:**
- Very efficient for large data sets.  
- Recursive in nature.  
- In-place sorting algorithm.  

**Time Complexity:**  
- Best Case: O(n log n)  
- Average Case: O(n log n)  
- Worst Case: O(n²) (rare, when pivot selection is poor)

---

### 3. Selection Sort
Selection Sort repeatedly finds the smallest (or largest) element from the unsorted portion and swaps it with the first unsorted element.  

**Characteristics:**
- Simple but not very efficient.  
- Performs well on small datasets.  

**Time Complexity:**  
- Best Case: O(n²)  
- Average Case: O(n²)  
- Worst Case: O(n²)

---

## Algorithm

### A. Bubble Sort
1. Start the program.  
2. Take an array of `n` elements.  
3. Repeat for each element:  
   - Compare adjacent elements.  
   - Swap them if they are out of order.  
4. Continue until no swaps are needed.  
5. Display the sorted array.  
6. Stop.  

---

### B. Quick Sort
1. Start the program.  
2. Select a pivot element.  
3. Partition the array:  
   - Elements smaller than pivot on the left.  
   - Elements larger than pivot on the right.  
4. Recursively apply steps 2–3 to each sub-array.  
5. Display the sorted array.  
6. Stop.  

---

### C. Selection Sort
1. Start the program.  
2. Take an array of `n` elements.  
3. For each position `i` from 0 to n-1:  
   - Find the smallest element in the unsorted portion.  
   - Swap it with the element at position `i`.  
4. Display the sorted array.  
5. Stop.  

---

## Functions Used
- **`bubbleSort(int arr[], int n)`** – Performs bubble sort on the given array.  
- **`quickSort(int arr[], int low, int high)`** – Recursively sorts the array using partitioning.  
- **`partition(int arr[], int low, int high)`** – Helps quick sort by finding the correct pivot position.  
- **`selectionSort(int arr[], int n)`** – Finds and places the smallest element iteratively.  
- **`display(int arr[], int n)`** – Prints the array elements.  

---

## Conclusion
Through this experiment, we successfully:  
1. Implemented **three sorting algorithms** — Bubble Sort, Quick Sort, and Selection Sort.  
2. Understood the differences in their working mechanisms and performance.  
3. Observed that:
   - **Bubble Sort** is easiest but inefficient for large datasets.  
   - **Quick Sort** is the fastest among the three for most inputs due to divide-and-conquer logic.  
   - **Selection Sort** is simple but also quadratic in time complexity.  

We conclude that while **simple sorting algorithms** are useful for learning, **efficient algorithms like Quick Sort** are preferred in real-world applications due to their scalability and speed.
