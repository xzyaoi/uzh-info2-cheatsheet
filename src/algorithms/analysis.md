# Algorithms Analysis

**<u>Complexity of Search Algorithms</u>**

Linear Search -> $O(n)$

Binary Search -> $O(log(n))$

**<u>Data Strucutres</u>**

Stack: Push, Pop, Top -> $O(1)$

Queue: Insert, Remove -> $O(1)$

Set, Hashmap: Insert, Contains -> $O(1)$. Bad hashing functions could increase up to $O(n)$

Binary Search Trees: Insert, Delete, Search -> $O(n)$. In theory, it usually performs a bit worse than $O(log(n))$

Red Black Trees: Insert, Delete, Search $O(log(n))$, guarantee by the Red Black Property.

**<u>Sorting</u>**

Insertion Sort, Bubble Sort -> $O(n^2)$

Quick Sort -> $O(n^2)$ but typically towards $O(n * log(n))$

Merge Sort -> $O(n * log(n))$

Theoretical Limit for Comparison Based Sorting is $O(n * log(n))$. More cool things about sorting at [sorting](https://theartofmachinery.com/2019/01/05/sorting_is_nlogn.html)

**<u>Graph Theory</u>** V -> Vertices E -> Edges

DFS, BFS -> Full Search is $O(V+E)$

Djikstra -> Single Source SP is $O((V+E)log(V))$

**<u>Master Theorem</u>**

If a recurrence relation is defined as $T(n)=aT(\frac{n}{b})+f(n)$ where 
* $a\geq 1$
* $b\geq 1$
* $f(n)$ asymptotically positive.

Then there are three cases:

* Case 1: $f(n)=O(n^{\log_b a-\epsilon})$ for some $\epsilon>0$, i.e. $f(n)$ grows polynomially slower than $n^{\log_b a}$. In this case, the work at leaves dominates: $T(n)=\Theta(n^{\log_b a})$.
* Case 2: $f(n)=\Theta(n^{\log_b a})$, i.e. $f(n)$ and $n^{\log_b a}$ are asymptotically the same. In this case, the work is evenly distributed: $T(n)=\Theta(n^{\log_b a}\log_b n)$.
* Case 3: $f(n)=\Omega(n^{\log_b a+\epsilon})$ for some $\epsilon>0$, i.e. $f(n)$ grows polynomially faster than $n^{\log_b a}$. In this case, the work at root dominates: $T(n)=\Theta(f(n))$.

