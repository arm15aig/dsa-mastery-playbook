# Topic 8: Recursion & Backtracking

* **Sample Practice Focus**: *Fibonacci Numbers*.

---

## 🛠️ Core Pattern: State Exploration & State Reversal (Backtracking)
Exploring a decision path fully, then reversing ("backtracking") the last choice to systematically test alternative combinations.

### Pseudocode Blueprint
```text
FUNCTION backtrack(current_combination, choices_left, results_list):
    // 1. GOAL REACHED (Base Case)
    IF current_combination meets the criteria:
        results_list.add(Copy of current_combination)
        RETURN
        
    // 2. EXPLORE ALL AVAILABLE CHOICES
    FOR choice IN choices_left:
        IF choice is valid/allowed:
            // Make the choice
            current_combination.add(choice)
            
            // Recurse deeper down this path
            backtrack(current_combination, remaining_choices_after_this, results_list)
            
            // UNDO THE CHOICE (The core "backtrack" step)
            current_combination.remove(choice)