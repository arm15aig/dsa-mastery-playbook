# dsa-mastery-playbook
Data Structure and Algorithm Mastery 

# DSA Technical Screen Interview Preparation

This repository contains curated structural blueprints, core patterns, algorithmic pseudocode, and complexity analysis guides.

## 📂 Repository Directory Map

Each subfolder contains a dedicated `README.md` breaking down the core structural patterns, algorithmic blueprints, Big-O metrics, and target interview checklists:

* **[Topic 1: Arrays & Strings](./01_arrays_and_strings)**
  * *Pattern*: Two-Pointer / Sliding Window ($O(N)$ Time, $O(1)$ Space)
  * *Practice Targets*: Designer PDF Viewer, Left Rotation

* **[Topic 2: Linked Lists](./02_linked_lists)**
  * *Pattern*: Floyd's Tortoise and Hare Cycle Detection ($O(N)$ Time, $O(1)$ Space)
  * *Practice Targets*: Insert a Node at a Position, Cycle Detection

* **[Topic 3: Stacks & Queues](./03_stacks_and_queues)**
  * *Pattern*: LIFO Symmetry Tracking ($O(N)$ Time, $O(N)$ Space)
  * *Practice Targets*: Balanced Brackets, Queue Using Two Stacks

* **[Topic 4: Hash Maps & Sets](./04_hash_maps_and_sets)**
  * *Pattern*: Complement Target Lookup ($O(N)$ Time, $O(N)$ Space)
  * *Practice Targets*: Ice Cream Parlor, Colorful Number

* **[Topic 5: Sorting Algorithms](./05_sorting_algorithms)**
  * *Pattern*: Preprocessing & Divide and Conquer ($O(N \log N)$ Time)
  * *Practice Targets*: Insertion Sort part 2, Quicksort part 2

* **[Topic 6: Trees](./06_trees)**
  * *Pattern*: Recursive Subtree Depth Calculation ($O(N)$ Time, $O(H)$ Space)
  * *Practice Targets*: Binary Tree Insertion, Height of a Binary Tree, QHeap1

* **[Topic 7: Graphs (BFS & DFS)](./07_graphs)**
  * *Pattern*: Breadth-First Level Traversal ($O(V + E)$ Time, $O(V)$ Space)
  * *Practice Targets*: Breadth-First Search Snakes and Ladders

* **[Topic 8: Recursion & Backtracking](./08_recursion_and_backtracking)**
  * *Pattern*: State Exploration & Reversal / Backtracking ($O(K^N)$ Time, $O(N)$ Space)
  * *Practice Targets*: Fibonacci Numbers

* **[Topic 9: Dynamic Programming](./09_dynamic_programming)**
  * *Pattern*: Memoized Top-Down State Overlap ($O(\text{States})$ Time, $O(\text{States})$ Space)
  * *Practice Targets*: Optimization and State Memoization Caching

---

## ⚡ Master Interview Day Checklist

Before beginning any problem, run through this universal operational execution sequence:
- [ ] **The 2-Minute Requirement Check**: Do not type immediately. Ask clarifying questions on constraints (e.g., negative numbers, empty arrays, null structures).
- [ ] **State a Brute Force Baseline**: Explicitly state the simple, non-optimal solution (e.g., $O(N^2)$ nested loop) to set a time complexity benchmark.
- [ ] **Propose the Optimization**: Formulate an argument explaining *why* a specific data structure (e.g., Hash Map, Queue) lowers the runtime bounds.
- [ ] **Speak Aloud While Coding**: Continuously communicate your logic and structural implementation choices to the interviewer.
- [ ] **Dry-Run Trace**: Verbally track a custom test case through your completed function line-by-line to catch logical syntax bugs or edge cases before hitting compile.
