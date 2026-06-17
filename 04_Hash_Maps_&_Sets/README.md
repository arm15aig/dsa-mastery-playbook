# Topic 4: Hash Maps & Sets

* **Sample Practice Focus**: *Ice Cream Parlor*, *Colorful Number*.

---

## 🛠️ Core Pattern: Complement Lookup (Target Match)
Instantly checking if a required counterpart element exists in the dataset while iterating through it.

### Pseudocode Blueprint
```text
FUNCTION findPairs(array, target):
    Initialize empty Hash Map (value -> index)
    
    FOR index, current_value IN array:
        complement = target - current_value
        
        IF complement EXISTS IN Map:
            RETURN [Map.get(complement), index]
            
        Map.put(current_value, index)
        
    RETURN empty_list