# Topic 2: Linked Lists

* **Sample Practice Focus**: *Insert a Node at a Position*, *Cycle Detection*.

---

## 🛠️ Core Pattern: Floyd's Tortoise and Hare (Cycle Detection)
Used to detect loops or find midpoints in pointer-based linear structures efficiently without using extra storage.

### Pseudocode Blueprint
```text
FUNCTION hasCycle(headNode):
    Initialize slow_pointer = headNode
    Initialize fast_pointer = headNode
    
    WHILE fast_pointer IS NOT null AND fast_pointer.next IS NOT null:
        slow_pointer = slow_pointer.next          // Moves 1 step
        fast_pointer = fast_pointer.next.next     // Moves 2 steps
        
        IF slow_pointer EQUALS fast_pointer:
            RETURN True   // Cycle detected!
            
    RETURN False   // Reached the end of the list, no cycle