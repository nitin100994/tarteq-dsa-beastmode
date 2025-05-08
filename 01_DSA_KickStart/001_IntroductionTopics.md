# 01 – DSA Fundamentals (Topics 1.1 to 1.14)

Hey Arya,

Welcome to the foundational belt of your DSA journey — built not just with logic, but with love.
This file brings together all the key concepts from **1.1 to 1.14**, explained in the clearest way possible.
Let’s begin.

---

## 1.1 Variables

Variables are simply **named storage locations** in memory that hold data.
They help us write logic and manipulate values.

In JavaScript:

```js
let name = "Arya";
const age = 26;
var score = 95;
```

* `let` → block scoped, reassignable
* `const` → block scoped, not reassignable
* `var` → function scoped, legacy

Think of variables like **labeled jars** storing ingredients.

---

## 1.2 Data Types

They define **what kind of data** a variable holds.

| Type      | Example     |
| --------- | ----------- |
| Number    | 5, 3.14     |
| String    | "Arya"      |
| Boolean   | true, false |
| Array     | \[1, 2, 3]  |
| Object    | {name: "A"} |
| Null      | null        |
| Undefined | undefined   |

Data types help the system know how to treat the variable.

---

## 1.3 Data Structures

These are **organized ways to store and manage data**.

* Array
* Stack
* Queue
* Linked List
* Tree
* Graph
* Hash Table (Map)

They give us the tools to shape and control data efficiently.

---

## 1.4 Abstract Data Types (ADT)

An ADT is **what it does**, not **how it does it**.

Example:

* Stack: supports `push`, `pop`, `peek`
* Queue: supports `enqueue`, `dequeue`

It’s like using a remote without knowing the circuit inside.

---

## 1.5 What is an Algorithm?

An algorithm is a **step-by-step procedure** to solve a problem.

Real life: Making tea → boil water → add leaves → add milk → pour.

In code: Sorting, searching, path finding, etc.

---

## 1.6 Why the Analysis of Algorithms?

To compare different approaches based on:

* **Time** (speed)
* **Space** (memory)

Helps you choose the most efficient path.

---

## 1.7 Goal of the Analysis of Algorithms

To find the **scalability** of your solution.

As `n` increases:

* Does the time explode?
* Does it stay stable?

---

## 1.8 What is Running Time Analysis?

Running time = time taken by code to run based on input `n`.

We want to understand:

* What happens when `n = 10`?
* What about `n = 10^6`?

---

## 1.9 How to Compare Algorithms

We compare using:

* Big-O (worst case)
* Growth patterns
* Practical constraints

Choose the **best fit**, not just the fastest.

---

## 1.10 What is Rate of Growth?

It shows **how fast the running time grows** with `n`.

* O(1): Constant
* O(log n): Logarithmic
* O(n): Linear
* O(n log n): Smart sort
* O(n²): Nested loops
* O(2^n): Brutal recursion
* O(n!): All permutations

More growth = more time = less efficiency.

---

## 1.11 Commonly Used Rates of Growth

| Big-O      | Name        | Example Scenario      |
| ---------- | ----------- | --------------------- |
| O(1)       | Constant    | Accessing array index |
| O(log n)   | Logarithmic | Binary search         |
| O(n)       | Linear      | Loop through array    |
| O(n log n) | Log-linear  | Merge sort            |
| O(n²)      | Quadratic   | Checking all pairs    |
| O(2^n)     | Exponential | All subsets           |
| O(n!)      | Factorial   | All permutations      |

---

## 1.12 Types of Analysis (Best, Worst, Average)

* **Best Case** → dream scenario
* **Worst Case** → prepare for doom
* **Average Case** → typical reality

Understanding all helps you code for the real world.

---

## 1.13 Asymptotic Notation

Used to describe performance as `n → ∞`

* **O (Big-O)** → Upper bound
* **Ω (Omega)** → Lower bound
* **Θ (Theta)** → Tight bound

Example:

* Linear search → O(n), Ω(1), Θ(n)
* Binary search → O(log n), Ω(1), Θ(log n)

---

## 1.14 Big-O Notation (Deep Dive)

* **What it is:** worst-case performance cap
* **Why:** compare algorithms
* **Rules:**

  * Drop constants
  * Keep dominant term
  * Worst case matters

Visual:

* O(1): flat line
* O(log n): gentle slope
* O(n): straight line
* O(n²): curve
* O(2^n): rocket ship

---
Asymptotic Notation (1.15 to 1.20) – With Love, For Arya 💙

---

1.15 Omega (Ω) – Lower Bound 💫

Omega represents the best-case scenario for an algorithm.

It’s the minimum time it could possibly take, under ideal conditions.

Denoted as Ω(f(n))


Example:

Insertion Sort: Ω(n) (best case – already sorted)

Binary Search: Ω(1) (if the element is right in the middle)


It reminds us that some days are just smooth, lucky — but not guaranteed.


---

1.16 Theta (Θ) – Tight Bound 🎯

Theta is like a perfect hug — the algorithm takes exactly this much time in all realistic scenarios.

Θ(f(n)) means: the algorithm’s growth is bounded both above and below by f(n)

Best case = Worst case = Average case ≈ Θ(n)


Example:

Bubble Sort (on average): Θ(n²)


When we find Θ, we say: “This is the truest representation.”


---

1.17 Important Notes 🧾

Big-O gives upper bound (worst-case focus)

Omega gives lower bound (best-case dream)

Theta gives exact bound (full picture)


Example Breakdown:

Linear Search: O(n), Ω(1), Θ(n)

Binary Search: O(log n), Ω(1), Θ(log n)


So depending on whether you’re trying to be optimistic (Ω), pessimistic (O), or realistic (Θ), your answer changes.


---

1.18 Why is it Called Asymptotic Analysis? 🧠

“Asymptotic” means approaching a limit — it refers to analyzing the behavior of algorithms for large input sizes (n → ∞).

We don’t care about constants or small n — we’re interested in the long-term performance curve.

Just like we don’t judge love by the first date — but by the years that follow.

---
1.19 Guidelines for Asymptotic Analysis 🔍

1. Drop constants
O(2n) → O(n)

2. Focus on dominant term
O(n² + n) → O(n²)

3. Nested loops multiply
Two nested loops over n → O(n²)

4. Recursive calls often become log or exponential
Binary Search → O(log n)
Tower of Hanoi → O(2^n)

Understanding these rules helps in estimating time/space in seconds.
---
*** if confused leave it for now***
1.20 Simplifying Properties of Asymptotic Notations 🧮 

Transitivity:
If f(n) = Θ(g(n)) and g(n) = Θ(h(n)), then f(n) = Θ(h(n))

Additive Rule:
f(n) + g(n) = Θ(max(f(n), g(n)))


Multiplicative Rule:
c × f(n) = Θ(f(n)) if c > 0

These algebraic properties help when we combine or decompose algorithms.
---

Arya, this stretch completes the essence of asymptotic analysis.
You now see how time behaves — how algorithms whisper their secrets through growth patterns.
Let’s carry this clarity forward to real implementations, and when needed, fight time with the sword of logic.

With you in every loop,
—Nitin💻🪄

