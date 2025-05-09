## 🌟 Array Problem 1: Find the Maximum Number in an Array  
*Difficulty: Beginner | DSA Vibe: Soft Start with Power*

---

### 🧠 Problem Statement

**Given an array of integers, find the largest (maximum) number in it.**

🧺 *Think of this like searching for the most expensive diamond in a box of jewels. One by one, you compare and replace — until the most dazzling one is found.*

---

### 🛠️ Approach: Linear Search

1. Start with an assumption: the **first element** is the max.
2. Loop through the array.
3. If you find any number **greater** than the current max, update the max.
4. At the end, you'll have the **maximum** value.

---

### 🐍 Python Code (Simple & Sweet)
```python
def find_max(arr):
    max_num = arr[0]  # Assume first number is max
    for num in arr:
        if num > max_num:
            max_num = num  # Update max if larger found
    return max_num

# Example:
arr = [5, 2, 9, 1, 7]
print("Maximum number:", find_max(arr))  # Output: 9
```

---

### 🌐 JavaScript Code (With ❤️ for Pooja)
```javascript
function findMax(arr) {
    let maxNum = arr[0]; // 🌱 Start by assuming first number is max

    for (let i = 0; i < arr.length; i++) {
        if (arr[i] > maxNum) {
            maxNum = arr[i]; // 🔄 Replace max if current is bigger
        }
    }

    return maxNum;
}

// Example:
const arr = [5, 2, 9, 1, 7];
console.log("Maximum number:", findMax(arr)); // Output: 9
```

---

### 💡 Dry Run Example

🧮 `arr = [5, 2, 9, 1, 7]`

- `max = 5`  
- Compare `2` → not greater → max stays  
- Compare `9` → greater → `max = 9`  
- Compare `1` → not greater  
- Compare `7` → not greater

✅ Final answer: **9**

---

### 💞 Why This Matters?

- This is your **first DSA step**, Gulaboo.  
- Every large tech interview builds on these basics.  
- It’s not just about the max number — it’s about understanding how logic **grows** from simplicity.

---

**🌸 P.S.**  
You don’t have to be fast right now.  
Just stay consistent.  
*One max at a time... and soon, you'll be the max among millions.*

🦋