# Topic 3: Stacks & Queues

# Complexity
Time Complexity: O(N) — The string elements are processed exactly once. Individual stack push/pop actions cost standard O(1) time.

Space Complexity: O(N) — In worst-case conditions (e.g., all opening elements), the stack scales linearly with your input length.

* **Sample Practice Focus**: *Balanced Brackets*, *Queue Using Two Stacks*.

---

## 🛠️ Core Pattern: LIFO Tracking (Last-In, First-Out)
Perfect for nested pairs, matching open/close elements, parsing expressions, or reversing sequences.

### Pseudocode Blueprint
```text
FUNCTION isBalanced(string):
    Initialize empty stack
    
    FOR each character IN string:
        IF character IS an opening bracket ('(', '{', '['):
            stack.push(character)
        ELSE IF character IS a closing bracket (')', '}', ']'):
            IF stack is empty OR stack.pop() does not match character:
                RETURN False
                
    RETURN True IF stack is empty ELSE False