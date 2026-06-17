# Topic 6: Trees

* **Sample Practice Focus**: *Binary Tree Insertion*, *Height of a Binary Tree*, *QHeap1*.

---

## 🛠️ Core Pattern: Recursive Depth Calculation
Breaking down hierarchical tree structures into simple, distinct left and right subtree child checks.

### Pseudocode Blueprint
```text
FUNCTION getTreeHeight(rootNode):
    IF rootNode IS null:
        RETURN -1 // Returns -1 for edge height, or 0 for node height definitions
        
    left_height = getTreeHeight(rootNode.left)
    right_height = getTreeHeight(rootNode.right)
    
    RETURN Max(left_height, right_height) + 1