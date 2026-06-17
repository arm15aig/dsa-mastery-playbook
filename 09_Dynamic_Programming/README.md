# Topic 9: Dynamic Programming (DP)

# Complexity
Time Complexity: O(Unique States) — With memoization, each distinct state configuration is calculated exactly once, turning exponential paths into clean, linear runtimes.

Space Complexity: O(Unique States) — Memory is required to maintain the lookup cache alongside the recursive call stack.

---

## 🛠️ Core Pattern: Memoized State Overlap (Top-Down DP)
Using a cache ("notebook") to store answers to subproblems so you never waste time calculating the exact same state twice.

### Pseudocode Blueprint
```text
FUNCTION solveDP(problem_state, memo_notebook):
    // 1. BASE CASES
    IF problem_state is invalid/terminal:
        RETURN baseline_value
        
    // 2. CHECK THE MEMO NOTEBOOK
    IF problem_state EXISTS IN memo_notebook:
        RETURN memo_notebook[problem_state]
        
    // 3. RECURSIVE CHOICES & OPTIMIZATION
    choice_A = solveDP(next_state_A, memo_notebook)
    choice_B = solveDP(next_state_B, memo_notebook)
    
    optimal_result = Max(choice_A, choice_B) 
    
    // 4. SAVE TO NOTEBOOK & RETURN
    memo_notebook[problem_state] = optimal_result
    RETURN optimal_result