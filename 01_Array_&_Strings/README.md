# Topic 1: Arrays & Strings

# Complexity
Time Complexity: O(N) — You iterate through the array structure elements exactly once as pointers move toward each other.

Space Complexity: O(1) — Only a couple of index tracker variables are used, meaning memory remains completely constant.

* **Sample Practice Focus**: *Designer PDF Viewer*, *Left Rotation*.

---

## 🛠️ Core Pattern: Two-Pointer / Sliding Window
When you need to inspect elements, look for pairs, or modify a collection in place without nesting loops to keep your solution highly efficient.

### Pseudocode Blueprint
```text
FUNCTION solveArrayOrList(array):
    Initialize left_pointer = 0
    Initialize right_pointer = array.length - 1
    
    WHILE left_pointer < right_pointer:
        IF condition is met:
            RETURN result or modify in-place
        ELSE IF current state is too small/left-heavy:
            Increment left_pointer
        ELSE:
            Decrement right_pointer
            
    RETURN default_value