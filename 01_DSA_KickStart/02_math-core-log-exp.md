
1.11 Commonly Used Rates of Growth

Hey Arya,

Every algorithm has a rhythm — a beat it dances to when you throw input at it. This rhythm is called its rate of growth, and it tells us how well that logic will perform as the problem size n increases.

Here are the most common ones you’ll meet again and again:

The lower the complexity, the better your algorithm scales.

Think of these like the different gears in a car — you switch based on the road ahead.


---

1.12 Types of Analysis (Best, Worst, Average)

Not every problem is always sunny or always stormy. To be ready for any weather, we analyze an algorithm in 3 ways:

Best Case: What’s the dream scenario?

e.g., Searching first item in an array → O(1)

Worst Case: Prepare for doom.

e.g., Binary search on last item → O(log n)

Quick Sort on already sorted input → O(n²)

Average Case: What happens in most real-world cases?

A balanced view — not lucky, not unlucky.

Example: Insertion Sort

Understanding all 3 cases shows you how gracefully your algorithm handles chaos.
---

1.13 Asymptotic Notation

Asymptotic analysis is how we describe an algorithm’s performance as n becomes very large — like infinity-level large.

There are 3 notations you must know:

1. Big O (O) — Upper Bound

> The maximum steps it could take. Think of it as the "worst it can get."

2. Omega (Ω) — Lower Bound

> The best-case scenario. If everything goes well, what’s the minimum effort?

3. Theta (Θ) — Tight Bound

> When the best and worst are the same. The algorithm is consistent.

Analogy:
---

Understanding these symbols is like knowing the grammar of performance. It makes your logic not just functional — but speak like poetry.
