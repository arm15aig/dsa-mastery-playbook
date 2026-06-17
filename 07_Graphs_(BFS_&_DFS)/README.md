# Topic 7: Graphs (BFS & DFS)



* **Sample Practice Focus**: *Breadth First Search Snakes and Ladders*.

---

## 🛠️ Core Pattern: Breadth-First Level Traversal (BFS)
Designed to locate shortest paths or minimum steps through a level-by-level frontier search.

### Pseudocode Blueprint
```text
FUNCTION graphBFS(startNode):
    Initialize empty Queue
    Initialize empty Set (visited)
    
    Queue.enqueue(startNode)
    visited.add(startNode)
    
    WHILE Queue IS NOT empty:
        currentNode = Queue.dequeue()
        Process(currentNode)
        
        FOR neighbor IN currentNode.getNeighbors():
            IF neighbor NOT IN visited:
                visited.add(neighbor)
                Queue.enqueue(neighbor)