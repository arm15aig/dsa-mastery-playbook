# Topic 7: Graphs (BFS & DFS)

# Complexity
Time Complexity: O(V + E) where V means vertices and E is edges. For regular 2D coordinate matrices, this translates directly to O(M × N).

Space Complexity: O(V) — Your tracking collections (queue and visited set) will hold graph nodes as they explore the structure.

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