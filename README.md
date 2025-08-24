# Getting Started with Algorithm

This guide covers essential algorithms, data structures, and mathematical concepts frequently encountered in competitive programming.

**A crucial piece of advice**: Merely understanding how an algorithm works is only the first step. True mastery comes from applying these concepts to solve problems. You must practice implementing these algorithms and adapting them to new challenges on your own. There is no substitute for hands-on problem-solving.

**Note**: Some problem descriptions linked here are in Chinese. You can often use an online translator or ask an LLM for assistance if you get stuck.

## Resource

This section lists highly recommended platforms, books, and tools for practice and learning. For most of the topics below, you can find excellent tutorials on sites like [CP-Algorithms](https://cp-algorithms.com/) or Wikipedia.

### Online Judging System

- [Luogu](https://www.luogu.com.cn): A Chinese OJ platform with a vast collection of problems from informatics olympiads.
- [AtCoder](https://atcoder.jp): A popular Japanese platform known for high-quality, math-oriented contests.
- [Codeforces](https://codeforces.com): The most popular platform for competitive programming, hosting regular contests for all skill levels.
- [SPOJ](http://www.spoj.com/): A classic online judge with a large number of problems, often used for practicing specific, well-known algorithms.
- [LeetCode](https://leetcode.com): Excellent for practicing specific topics and preparing for technical interviews.

### Books

- *Introduction to Algorithms* - Thomas H.Cormen/Charles E.Leiserson/Ronald L.Rivest/Clifford Stein
- [Competitive Programmer’s Handbook](https://cses.fi/book/book.pdf) - Antti Laaksonen
- *Algorithms Illuminated* - Tim Roughgarden

### Tools & Utilities

- [Algorithm Visualizer](http://algorithm-visualizer.org/)
- [The On-Line Encyclopedia of Integer Sequences (OEIS)](https://oeis.org)
- [Wolfram Alpha](https://www.wolframalpha.com/)

## Core Algorithmic Techniques

### Binary Search

[Wikipedia](https://en.wikipedia.org/wiki/Binary_search)
[CP](https://cp-algorithms.com/num_methods/binary_search.html)

A powerful search algorithm that finds the position of a target value within a sorted array by repeatedly dividing the search interval in half.

- [Problem 1](https://codeforces.com/contest/1173/problem/C)
- [Problem 2](https://codeforces.com/contest/51/problem/C)

### Dynamic Programming

An optimization technique that solves complex problems by breaking them down into simpler subproblems, storing their results to avoid redundant computations.

- [DP Tutorial and Problem List](https://codeforces.com/blog/entry/67679)

### Overloading Operators

A programming language feature that allows you to define custom behavior for operators (like `+`, `-`, `<`) with your own data types (e.g., structs or classes). This can make code for concepts like vectors, matrices, or modular arithmetic much cleaner and more intuitive.

## Sorting Algorithms

### Merge Sort

[Wikipedia](https://en.wikipedia.org/wiki/Merge_sort)

An efficient, stable, comparison-based sorting algorithm that works by dividing an array into halves, sorting them recursively, and then merging the sorted halves.

### Heap (Priority Queues)

[Wikipedia](https://en.wikipedia.org/wiki/Heap_(data_structure))

A specialized tree-based data structure that satisfies the heap property. It's perfect for efficiently finding and extracting the minimum or maximum element.

## String Algorithms

### Hash

A technique that converts a string into a numeric value (a hash) to allow for fast comparisons. Polynomial rolling hash is a common and powerful method used to solve many problems involving string matching and palindromes.

[Wikipedia](https://en.wikipedia.org/wiki/Hash_function)
[CP](https://cp-algorithms.com/string/string-hashing.html)

- [Problem 1](https://codeforces.com/contest/1200/problem/E)
- [Problem 2](https://www.spoj.com/problems/ADACLEAN/)

### KMP Algorithm (Prefix Function)

An efficient string-searching algorithm that preprocesses the pattern to skip unnecessary comparisons, achieving linear time complexity.

[Wikipedia](https://en.wikipedia.org/wiki/Knuth–Morris–Pratt_algorithm)
[CP](https://cp-algorithms.com/string/prefix-function.html)

- [Problem 1](https://www.spoj.com/problems/ADAPET/)
- [Problem 2](https://codeforces.com/contest/808/problem/G)

### Z Algorithm

[CP](https://cp-algorithms.com/string/z-function.html)

Creates an array (the Z-array) where `Z[i]` is the length of the longest common prefix between the original string and the suffix starting at `i`. Useful for various pattern-matching problems.

- [Problem 1](https://www.spoj.com/problems/SUFEQPRE/)
- [Problem 2](https://codeforces.com/contest/119/problem/D)

### Trie (Prefix Tree)

[Wikipedia](https://en.wikipedia.org/wiki/Trie)

A tree-like data structure that stores a dynamic set of strings, enabling fast retrieval and prefix-based searches.

### Aho-Corasick Algorithm

[Wikipedia](https://en.wikipedia.org/wiki/Aho–Corasick_algorithm)
[CP](https://cp-algorithms.com/string/aho_corasick.html)

A string-searching algorithm that can find all occurrences of a set of keywords in a text simultaneously. It combines a trie with failure links, similar to KMP.

- [Problem 1](https://codeforces.com/problemset/problem/346/B)
- [Problem 2](https://codeforces.com/contest/696/problem/D)

## Graph Algorithms

### DFS & BFS (Depth-First & Breadth-First Search)

Two fundamental graph traversal algorithms. DFS explores as far as possible along each branch before backtracking, while BFS explores all neighbor nodes at the present depth prior to moving on to nodes at the next depth level.

### Shortest Path (Dijkstra & Bellman–Ford & Johnson)

- [Problem 1](http://www.spoj.com/problems/ADATRIP/)
- [Probelm 2](http://codeforces.com/contest/144/problem/D)

### Tarjan's Algorithm for Strongly Connected Components (SCCs)

A DFS-based algorithm that finds the strongly connected components (maximal subgraphs where every vertex is reachable from every other vertex) in a directed graph.

- [Problem 1](https://www.spoj.com/problems/ADAPANEL/)
- [Problem 2](https://codeforces.com/problemset/problem/427/C)

### Spanning Tree (Prim & Kruskal)

A minimum spanning tree (MST) is a subset of the edges of a connected, edge-weighted undirected graph that connects all the vertices together, without any cycles and with the minimum possible total edge weight.

- [Problem 1](http://codeforces.com/contest/908/problem/F)
- [Problem 2](http://codeforces.com/contest/76/problem/A)

### Topological Sorting

A linear ordering of vertices in a directed acyclic graph (DAG) such that for every directed edge from vertex `u` to vertex `v`, `u` comes before `v` in the ordering.

## Data Structure

### Segment Tree

[Wikipedia](https://en.wikipedia.org/wiki/Segment_tree)
[CP](https://cp-algorithms.com/data_structures/segment_tree.html)

A versatile tree-based data structure that allows for efficient range queries (e.g., sum, min, max) and point updates on an array.

- [Problem 1](https://codeforces.com/problemset/problem/242/E)
- [Problem 2](https://codeforces.com/problemset/problem/240/F)
- [Problem 3](https://www.spoj.com/problems/GSS2/)(a little difficult)

### Balanced Binary Search Trees (Splay, Scapegoat)

Advanced tree structures that automatically maintain a balanced height, ensuring that operations like search, insert, and delete remain efficient (logarithmic time). They are incredibly flexible for complex order-based problems.

### Persistent Data Structure

Structures where modifying the data structure creates a new version while keeping the old version accessible. This is useful for querying past states of the data.

- [Problem 0: kth smallest value in an interval](https://www.luogu.com.cn/problem/P3834) (online algorithm only, *the problem description is in Chinese)
- [Problem 1](https://codeforces.com/problemset/problem/242/E)
- [Problem 2: find the mex (smallest non-negative integer that does not appear in a set) of an interval ](https://www.luogu.com.cn/problem/P4137)(online algorithm, *the problem description is in Chinese)
- [Problem 3](https://codeforces.com/problemset/problem/1422/F)

### Square Root Decomposition

A technique that divides an array into blocks of size  
sqrt(N) to perform range queries and updates. It's often simpler to implement than more complex structures like segment trees and can be surprisingly versatile.

- [Problem 1](https://codeforces.com/problemset/problem/920/F) (also can be done by using segment tree)
- [Problem 2 (Mo's algorithm)](https://codeforces.com/problemset/problem/617/E)

## Mathematical Concepts

### Prime Numbers & Sieves (Euler's Sieve)

Fundamental concepts in number theory. Sieves, like the Sieve of Eratosthenes or Euler's Sieve, are highly efficient algorithms for finding all prime numbers up to a specified integer.

### Modular Multiplicative Inverse

The inverse of a number `a` modulo `m` is a number `x` such that `(a*x) % m = 1`. It's possible to precompute inverses for all numbers up to `n` in linear time.

### Game Theory (Nim Game)

A branch of mathematics concerned with strategy. The Nim Game is a classic impartial game whose solution often involves the Sprague-Grundy theorem and XOR operations.

- [Problem 0](https://www.luogu.com.cn/problem/P2197) (*the problem description is in Chinese)
- [Problem 1](https://www.luogu.com.cn/problem/P1247) (*the problem description is in Chinese)
- [Problem 2 (K-Nim, a little difficult)](https://www.luogu.com.cn/problem/P2490) (*the problem description is in Chinese)
- [Problem 3 (Anti-Nim)](https://www.luogu.com.cn/problem/P4279) (*the problem description is in Chinese)
- [Problem 4 (altered Nim Game)](https://www.luogu.com.cn/problem/P3480) (*the problem description is in Chinese)