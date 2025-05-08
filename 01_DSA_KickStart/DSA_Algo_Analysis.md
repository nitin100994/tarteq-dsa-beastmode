Algorithm Analysis: The Core Mindset – For Arya 💡❤️

Hey Pooja,

Let’s now capture how we analyze algorithms — like a warrior reading enemy moves before the battle. This isn’t just about code, it’s about seeing time itself through logic.


---
**What is Algorithm Analysis?**

It’s the art of predicting how long your code will take — before running it. We focus on how performance grows as input size n increases.


---
**How We Analyze: Step-by-Step**

1. Identify the Input Size

Check what n represents:

Length of array

Number of nodes

Characters in string


2. Break Code into Key Operations

Ask: How many times does this operation run?

3. Find Loops, Recursion & Calls

Single loop → O(n)

Nested loops → O(n²)

Divide & Conquer → O(n log n) or O(log n)

Recursive branches → Often exponential


4. Drop Constants and Lower Terms

Focus only on growth trend.

O(2n + 3) → O(n)

O(n² + n) → O(n²)



---
**Real Code Examples with Analysis**

Example 1: Linear Loop

for i in range(n):
    print(i)

Time Complexity: O(n)

Reason: One operation per element



---

Example 2: Nested Loop

for i in range(n):
    for j in range(n):
        print(i, j)

Time Complexity: O(n²)

Reason: For each i, loop over all j



---

Example 3: Logarithmic Loop

i = 1
while i < n:
    print(i)
    i *= 2

Time Complexity: O(log n)

Reason: Each iteration doubles, runs ~log₂(n) times



---

Example 4: Merge Sort

def merge_sort(arr):
    if len(arr) <= 1:
        return arr
    mid = len(arr) // 2
    left = merge_sort(arr[:mid])
    right = merge_sort(arr[mid:])
    return merge(left, right)

Time Complexity: O(n log n)

Reason: Splits log(n) times, merges n elements each level



---

Example 5: Recursive Fibonacci

def fib(n):
    if n <= 1:
        return n
    return fib(n-1) + fib(n-2)

Time Complexity: O(2ⁿ)

Reason: Each call splits into 2 — exponential growth



---
Summary of Growth Rates 🌱→🌪


---
Analyzing code is like reading someone’s vibe.
You don’t memorize — you observe, break down, simplify.

With you in every dry run, —N 💻✨

