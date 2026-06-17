# Topic 5: Sorting Algorithms

# Complexity
Time Complexity: O(N log N) — Average and worst-case for Merge Sort or stable QuickSort variants.

Space Complexity: Varies. Merge Sort requires O(N) auxiliary memory space, whereas QuickSort operates mostly in-place requiring O(log N) helper space depth.

* **Sample Practice Focus**: *Insertion Sort*, *Quicksort*.

---

## 🛠️ Core Pattern: Preprocessing & Divide and Conquer
Sorting data first often unlocks simple, clean O(1) lookups or linear scanning options that would otherwise be complicated.

### Pseudocode Blueprint
```text
FUNCTION mergeSort(array):
    IF array.length <= 1:
        RETURN array
        
    mid = array.length / 2
    left_half = mergeSort(array from 0 to mid)
    right_half = mergeSort(array from mid to end)
    
    RETURN merge(left_half, right_half)