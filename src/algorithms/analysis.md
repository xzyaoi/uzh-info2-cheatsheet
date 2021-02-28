# Algorithms Analysis

**<u>Algorithms Complexity</u>**

Linear Search -> O(n)

Binary Search -> O(log(n))

**Data Strucutres:**

Stack : Push, Pop, Top -> O(1)

Queue : Insert, Remove -> O(1)

Set, Hashmap: Insert, Contains -> O(1). Bad hashing functions could increase up to O(n)

Binary Search Trees: Insert, Delete, Search -> O(n). In theory, it performs on average about O(log(n))

Red Black Trees: Insert, Delete, Search O(log(n)), guarantee by the Red Black Property.

**Sorting:**

InsertionSort, BubbleSort -> O(n^2)

Quick Sort -> O(n^2) but typically towards O(n * log(n))

Merge Sort -> O(n * log(n))
Theoretical Limit for Comparison Based Sorting is O(n * log(n)). More cool things about sorting at [sorting](https://theartofmachinery.com/2019/01/05/sorting_is_nlogn.html)

**Graph Theory:** V -> Vertices E -> Edges

DFS, BFS -> Full Search is O(V+E)
Djikstra -> Single Source SP is O((V+E)log(V))

**Dynamic Programming:**

**<u>Master Theorem</u>**

