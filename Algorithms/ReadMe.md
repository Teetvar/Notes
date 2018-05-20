# Algorithms and their Application Notes:
Everything you need to know.

<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Algorithms and their Application Notes:](#algorithms-and-their-application-notes)
	- [The Foundations of Algorithm Analysis](#the-foundations-of-algorithm-analysis)
		- [Runtime](#runtime)
		- [Asymptotic Analysis](#asymptotic-analysis)
			- [What does Asymptotic Analysis mean?](#what-does-asymptotic-analysis-mean)
			- [Estimating "Running Time"](#estimating-running-time)
		- [T(_n_) & O(_n_)](#tn-on)
		- [Pseudo-Code](#pseudo-code)
			- [Pseudo-Code Details](#pseudo-code-details)
			- [Pseudo-Code Details Continued](#pseudo-code-details-continued)
			- [Variables](#variables)
			- [If Statements](#if-statements)
			- [For Loops](#for-loops)
		- [Primitive Operations](#primitive-operations)
		- [Counting Primitive Operations](#counting-primitive-operations)
	- [Mathematical Foundation of Algorithms](#mathematical-foundation-of-algorithms)
		- [variables](#variables)
		- [Sets](#sets)
		- [Set Operators](#set-operators)
		- [Equations](#equations)
		- [Function:](#function)
			- [Exponential Function:](#exponential-function)
		- [Subscripts](#subscripts)
		- [Summation](#summation)
		- [Products](#products)
		- [Factorial](#factorial)
		- [Permutation](#permutation)
		- [Combination](#combination)
		- [Permutations and Combinations](#permutations-and-combinations)
		- [Floor and Ceiling Functions](#floor-and-ceiling-functions)
			- [Floor](#floor)
			- [Cieling](#cieling)
		- [Logarithms](#logarithms)
		- [Other topics of Mathematical Foundatation which maybe of interest:](#other-topics-of-mathematical-foundatation-which-maybe-of-interest)
	- [Time Complexity and Aymptotic notation](#time-complexity-and-aymptotic-notation)
		- [Why Sorting?](#why-sorting)
			- [Selection Sort Algorithms](#selection-sort-algorithms)
		- [How fast is the Algorithm?](#how-fast-is-the-algorithm)
			- [The Number of Operations](#the-number-of-operations)
		- [The Big-Oh notation](#the-big-oh-notation)
		- [Example: Binary Search](#example-binary-search)
			- [Binary Search Example](#binary-search-example)
		- [Big-Oh Rules](#big-oh-rules)
		- [Asymptotic Algorithm Analysis](#asymptotic-algorithm-analysis)
		- [The Classes of Algorithms](#the-classes-of-algorithms)
		- [Examples of NP-COMPLETE problems](#examples-of-np-complete-problems)
		- [Consequences of P=NP](#consequences-of-pnp)
		- [Big-Oh and Growth Rate](#big-oh-and-growth-rate)
		- [Relatives of Big-Oh](#relatives-of-big-oh)
		- [Asymptotic Notation](#asymptotic-notation)
		- [Why is Big-Oh the interesting one?](#why-is-big-oh-the-interesting-one)
	- [Data Strucutres and their Applications:](#data-strucutres-and-their-applications)
		- [A note on Complexity](#a-note-on-complexity)
		- [Why study Data Structures?](#why-study-data-structures)
		- [Lists](#lists)
			- [Two ways to implement lists:](#two-ways-to-implement-lists)
		- [Stacks](#stacks)
			- [Using Stacks](#using-stacks)
		- [Queues](#queues)
			- [Using Queues](#using-queues)
			- [How to Implement Queues](#how-to-implement-queues)
		- [Hash Tables](#hash-tables)
			- [How to Implement Hash Tables](#how-to-implement-hash-tables)
		- [Applications](#applications)
		- [Graphs](#graphs)
		- [An Abstract View of Graphs](#an-abstract-view-of-graphs)
		- [Why Study Graphs?](#why-study-graphs)
		- [How can graphs help?](#how-can-graphs-help)
		- [How to define a graph?](#how-to-define-a-graph)
		- [Graph Definitions](#graph-definitions)
			- [Directed Graphs](#directed-graphs)
			- [Undirected Graphs](#undirected-graphs)
			- [Complete Graphs](#complete-graphs)
			- [Paths](#paths)
			- [Connectivity](#connectivity)
			- [Weighted Graph](#weighted-graph)
		- [Connected Graph](#connected-graph)
		- [Weighted Graph](#weighted-graph)
		- [How to Represent a Graph](#how-to-represent-a-graph)
		- [Trees](#trees)
	- [Classic Algorithms - Sorting](#classic-algorithms-sorting)
		- [What Sorting Algorithms?](#what-sorting-algorithms)
		- [A nate of Growth Rates](#a-nate-of-growth-rates)
		- [Why Sorting?](#why-sorting)
		- [Formal Definition of sorting](#formal-definition-of-sorting)
		- [Bubble Sorting](#bubble-sorting)
		- [Bubble Sort: An Example](#bubble-sort-an-example)
		- [Bubble Sort Summary](#bubble-sort-summary)
		- [Bubble Sort](#bubble-sort)
		- [Best-Case Analysis](#best-case-analysis)
		- [Worst-Case Analysis](#worst-case-analysis)
		- [Average-Case Analysis](#average-case-analysis)
		- [Quick Sort](#quick-sort)
		- [Quick Sort Example](#quick-sort-example)
		- [The Quick Sort Algorithms](#the-quick-sort-algorithms)
			- [The Quick Sort Algorithm](#the-quick-sort-algorithm)
			- [The PivotList Algorithm](#the-pivotlist-algorithm)
		- [Worst-Case and Best-Case Analysis](#worst-case-and-best-case-analysis)
			- [Worst Case](#worst-case)
			- [Best Case](#best-case)
		- [Average-Case Analysis](#average-case-analysis)
		- [Comparison of Sorting Algorithms](#comparison-of-sorting-algorithms)
		- [Radix Sort](#radix-sort)
	- [Classic Algorithms - Graph Traversal](#classic-algorithms-graph-traversal)
		- [What is "Search" in Graphs?](#what-is-search-in-graphs)
		- [What is "Depth-First"?](#what-is-depth-first)
		- [What is "Depth-First Search"?](#what-is-depth-first-search)
		- [DFS Undirected graphs](#dfs-undirected-graphs)
		- [Algorithhm: DFS(G, n)](#algorithhm-dfsg-n)
		- [DFS RUnning Time Analysis](#dfs-running-time-analysis)
		- [Other Types of GrThere are other ways to search a graph other than visiting all nodes](#other-types-of-grthere-are-other-ways-to-search-a-graph-other-than-visiting-all-nodes)
		- [The Exhaustive Searching](#the-exhaustive-searching)
		- [Algorithm: Exhaustive(G, n, p)](#algorithm-exhaustiveg-n-p)
		- [Exhaustive Running Time](#exhaustive-running-time)
		- [Bredth-First Searching](#bredth-first-searching)
		- [Best-Fit Search](#best-fit-search)
		- [A* Search](#a-search)
		- [The A* Algorithm](#the-a-algorithm)
		- [A* Search](#a-search)
		- [Minimum Spanning trees](#minimum-spanning-trees)
		- [Prim's Algorithm for most](#prims-algorithm-for-most)
		- [Prim's Algorithm Example](#prims-algorithm-example)
		- [Applications for MST](#applications-for-mst)
		- [Other "Famous" Graph algorithms](#other-famous-graph-algorithms)
		- [Brief look at Floyd-Warshall](#brief-look-at-floyd-warshall)
	- [Search Algorithms, Representation, Fitness and Fitness Landscapes.](#search-algorithms-representation-fitness-and-fitness-landscapes)
		- [Definition of a Search Problem:](#definition-of-a-search-problem)
		- [What is a Heuristic?](#what-is-a-heuristic)
		- [Search Problems](#search-problems)
		- [Fitness](#fitness)
		- [Fitness Landscapes](#fitness-landscapes)
		- [Global and Local Optima](#global-and-local-optima)
		- [Representation](#representation)
		- [The Scales Problem](#the-scales-problem)
	- [Heuristic Search, Hill Climbing and Simulated Annealing](#heuristic-search-hill-climbing-and-simulated-annealing)
		- [Heuristic Search](#heuristic-search)
		- [There is no Free Lunch!](#there-is-no-free-lunch)
		- [Random numbers](#random-numbers)
		- [The Exponential Function](#the-exponential-function)
		- [Random Mutation Hill Climbing](#random-mutation-hill-climbing)
		- [Random Start and Small Change Pseudocode:](#random-start-and-small-change-pseudocode)
		- [Stochastic Hill climbing](#stochastic-hill-climbing)
		- [Random Restart Hill Climbing](#random-restart-hill-climbing)
		- [Simulated Annealing](#simulated-annealing)
		- [SA Convergence  Graph](#sa-convergence-graph)
		- [A noteabout HC and SA](#a-noteabout-hc-and-sa)
	- [The Simulated Annealing Algorithm](#the-simulated-annealing-algorithm)
	- [Parameter Optimisation](#parameter-optimisation)
		- [Optimisation Definitions](#optimisation-definitions)
		- [Optimisation Problems](#optimisation-problems)
		- [Parameter Optimisation:](#parameter-optimisation)
		- [Combinatorial Optimisation:](#combinatorial-optimisation)
		- [Subset Selection](#subset-selection)
		- [Permutation Problems](#permutation-problems)
		- [Data Clustering](#data-clustering)
		- [Bin Packing](#bin-packing)
		- [Multi Objective Optimisation](#multi-objective-optimisation)
		- [Weighted Fitness](#weighted-fitness)
		- [Pareto Optimality](#pareto-optimality)
		- [Constraint Satisfaction Problems](#constraint-satisfaction-problems)
		- [CSP Applications](#csp-applications)
		- [CSP Strategies](#csp-strategies)
	- [Tabu Search and ILS](#tabu-search-and-ils)
		- [Popuar Heuristics](#popuar-heuristics)
		- [Tabu (Taboo) Search](#tabu-taboo-search)
		- [Tabu Search - Key Concepts:](#tabu-search-key-concepts)
		- [Tabu Search Stopping Conditions](#tabu-search-stopping-conditions)
		- [Parameters of Tabu Search](#parameters-of-tabu-search)
		- [The Pros and Cons for Tabu Search](#the-pros-and-cons-for-tabu-search)

<!-- /TOC -->

## The Foundations of Algorithm Analysis
### Runtime
The running time of an algorithm varies with the input and typically grows with the input size. An algorithm may run faster on certain data sets than on others hence it would have the following run times:
 - Best case
	 - The best case is not very informative
 - Average case
	 -	The average case can be difficult to determine
 - Worst case
	 - Easier to analyse
	 - Crucial to applications such as air traffic control, surgery, finance,…
		 - E.g. Real time applications

### Asymptotic Analysis
#### What does Asymptotic Analysis mean?
 - For our purpose, it means the long term behavior of something, in this case, an Algorithm.
 - The technique uses a high-level description of the algorithm instead of an implementation.
 - Takes into account all possible inputs
 - Allows us to evaluate the speed of an algorithm independently of the hardware/software environment

#### Estimating "Running Time"
 - Write down an algorithm.
	 - Using Pseudo-Code
 - In terms of a set of primitive operations:
	 - Count the number of steps In terms of primitive operations, considering worst case input.
	 -  Bound or “estimate” the running time.
		 - Ignore constant factors
		 - Bound fundamental running time
 - This leads onto the Big-Oh (Big-O) notation for computational complexity.

### T(_n_) & O(_n_)
 - We estimate the running time/computation of an algorithm.
 - We refer to this resultant formula as T(_n_) where _n_ is the size of the input.
 - If there is more than one input we might have T(_n,m_) (etc…) where *n* and *m* are the sizes of the input.
 - We can use *T(n)* to compute a very important property called the big-O ***O(n)***.

### Pseudo-Code
 - Pseudo-Code is a cross between a programming language and written text.
 - It is used to represent algorithms in a programming language independent manner.
 - We often specify the input and output and number the lines.
 - **The additional notes from this point forward will be based on The Universal Pseudo-Code format, created by Dr. Stephen Swift:**

![](https://media.discordapp.net/attachments/334011383140188161/447331830740418570/unknown.png?width=558&height=384)

 - We use the normal concepts of variables, loops and conditional statements.
 - Often we use mathematical notation:
	-	, e.g. sets, equations, etc…
 - We do not call functions unless we describe the Pseudo-Code for them or describe what they do:
	-	For example we would not say:
		-	X = Y.toLowerCase();
	-	However we could say:
		-	Let X equal the lower case version of Y
		-	Unless we have previous defined the method, function, sub-routine, algorithm, etc…

#### Pseudo-Code Details
 - Control flow:
  - `If … Then … [Else …] End If`
- `While … End While`
- `Repeat … Until …`
- `For …End For …`
 - Indentation replaces braces [as in Python]
 - Method/algorithm declaration:
	`Algorithm number name (arguments/parameters)`
	`Input …`
`...`
`Output …`
-	Method/algorithm calls
	-	Call name `(arguments/parameters)`

#### Pseudo-Code Details Continued
-	Expressions
	-	We use a single = sign for both assignment and equality testing
	-	`Let x = 0`
	-	`If x = y Then...`
	-	The context differentiates the meaning of the usage…
-	n<sup>2</sup> superscripts, subscripts n<sub>i</sub> and other mathematical formatting is allowed
-	We often write the algorithm in a different font such as Courier New for Mono-spacing and Clarity.

#### Variables
![](https://cdn.discordapp.com/attachments/334011383140188161/447334384836542475/unknown.png)

#### If Statements
![](https://cdn.discordapp.com/attachments/334011383140188161/447334543851126814/unknown.png)

#### For Loops
![](https://cdn.discordapp.com/attachments/334011383140188161/447334688432979971/unknown.png)

### Primitive Operations
-	Basic computations performed by an algorithm.
-	Identifiable in Pseudo-Code.
-	Largely independent from the programming language.
-	Examples:
	-	Evaluating an expression (x>y?)
	-	Assigning a value to a variable (x=0)
	-	Indexing into an array (for A[0] or A[i] we might use the mathematical notation a<sub>0</sub> or a<sub>i</sub>)
	-	Calling a method
	-	Returning from a method

![](https://cdn.discordapp.com/attachments/334011383140188161/447336167122141184/unknown.png)

-	The most difficult part of the process is getting all of the nested loops correct.
-	We will see that later on that if you count 5 primitive operations for a line instead of 6 it does not really matter
	-	However if you get the loops wrong, the error will matter.
-	This is why getting the correct level of indentation is important
	-	It helps to show the structure of the loops and conditionals and thus helps with the calculations

### Counting Primitive Operations
-	By inspecting the Pseudo-Code, we can determine the maximum number of primitive operations executed by an algorithm, as a function of the input size (n)

![](https://cdn.discordapp.com/attachments/334011383140188161/447336726906667015/unknown.png)

![](https://media.discordapp.net/attachments/334011383140188161/447337001423863808/unknown.png?width=580&height=274)

## Mathematical Foundation of Algorithms
- Mathematics is a decriptive language.
- It can be used to precisely describe how numerical items relate to each other.
- it can be used to model the real world.
- We can model the performance and efficiencyc of algorithms using mathematics.

### variables
- A variable is a symbol used to represent a mathematical construct
  - E.g. numbers, sets, lists , vectors, matrices, …
- Often lower case letters or Greek letters are used
  - E.g. _x, y, z, Ω, α, β, …_
- Variables in Mathematics are treated the same as variables within a programming language.
  - They can be thought of as a box containing a value that can be read from or written to

### Sets
- A set is a finite or infinite collection of items
- A set has no order
- You cannot index a set…
- A set only contains one copy of an item
- We write a∈A to say item a is a member of set A
- ∉: not a member
- The empty set: ϕ
- |A| is the cardinality of A, i.e. How many items in A
- Some well known sets:
  - R: Real numbers
  - Z: Integers
  - N: Natural numbers (integers ≥ 0)
  - The alphabet

### Set Operators
- Creating: A = {<variable> : <inclusion criteria>}
- A = {n<sup>2</sup> : n is an integer and 0 ≤ n ≤ 5}
- A = {0, 1, 4, 9, 16, 25}
- Union:
  - A = B ∪ C, A = {a : a∈B OR a∈C}
  - A contains all of B and C
- Intersection:
  - A = B ∩ C, A = {a : a∈B AND a∈C}
  - A contains only what B and C have in common
- Subset:
  - If A is a set then B ⊆ A (B is a subset of A)
  - if every element of B is also in A, i.e. B is contained in A, e.g. N ⊆  Z , i.e. all natural numbers are integers

- Set Subtraction: A = C\B, A = {a : a∈C AND a∉B}
  - A is B with all the elements of C removed

### Equations
- An equation uses mathematical operators to relate one set of variables or numbers to another set of variables or numbers.
  - 2+2 = 4 (a very simple equation)
  - y = _mx_ + _c_ (a straight line)
  - _ax<sup>2</sup> + bx + c_ = 0
    - (a quadratic equation)
  - _(x-a)<sup>2</sup>+(y-b)<sup>2</sup>=r<sup>2</sup>_
    - (a circle of radius r with centre a,b)
- Often we have to simplify an equation.
  - This often means adding up similar terms and ordering the powers
    - (n-1)(n-2)(n-3)=(n<sup>2</sup>-2n-n+2)(n-3)=(n<sup>2</sup>-3n+2)(n-3)=n<sup>3</sup>-3n<sup>2</sup>-3n<sup>2</sup>+9n+2n-6
      - Equals n<sup>3</sup>-6n<sup>2</sup>+11n-6
      - Do not mistake this for nXnXn = 3N

### Function:
- A function is a relation that uniquely associates members of one set with members of another set:
  - Functions can take parameters
    - f(x,y)= 2x+y
  - Functions can be many to one
    - f(x) = 7
  - Functions can be one to one
    - f(x) = 7x + 3.21
  - Functions can be one to many
    - f(x) = √x

#### Exponential Function:
  - f(x) = exp(x) = e<sup>x</sup>
    - where e = 2.718…
  -  ![](https://camo.githubusercontent.com/225c6e59a72973b06c9ab5fae8a8e63f8332b35a/687474703a2f2f6d617468776f726c642e776f6c6672616d2e636f6d2f696d616765732f696e7465726163746976652f4578705265616c2e676966)

### Subscripts
  - A subscript is a natural number that indexes a list of variables.
  - For example:
    - Let X be the list (or vector) [x<sub>1</sub>,...,x</sub>n</sub>], then to access any element we use the notation x<sub>i</sub>, where 1≤i ≤n
  - We use the notation |X| to refer to the number of elements in the list X, which is n in this case
  - For Example:
    - X = [5,2,-8,3.6,88,2000.003]
  - Then x1=5, x2 = 2, x3 = -8 etc…
  - Note also that |X|=6
  - Note also that we use double subscripts for arrays (matrices)

### Summation
- Let X be the list [x1,…,xn], then if we want sum all of the elements up, we would use the notation:

| Summation | Ouput |
|:----------:|:----------:|
| ![](https://camo.githubusercontent.com/7a076bc62991d68c7e7a2ed2b3ef88fd81548f9b/68747470733a2f2f6c617465782e636f6465636f67732e636f6d2f6769662e6c617465783f25323425323453253230253344253230253543646973706c61797374796c6525354373756d5f25374269253344312537442535452537424e253744253230585f69253234253234) | S = X<sub>1</sub> + X<sub>2</sub> + X<sub>3</sub>+ …X<sub>n</sub> |

- Note that we are arbitrarily assigning the result to s. If we wanted to sum the squares:

| Summation | Ouput |
|:----------:|:----------:|
| ![](https://camo.githubusercontent.com/dc5cbb7ed52c1f4288b41f46e444a8744de27467/68747470733a2f2f6c617465782e636f6465636f67732e636f6d2f6769662e6c617465783f25323425323453253230253344253230253543646973706c61797374796c6525354373756d5f25374269253344312537442535452537424e253744253230585f6925323025354525374232253744253234253234) | S = X<sub>1</sub><sup>2</sup> + X<sub>2</sub><sup>2</sup> + X<sub>3</sub><sup>2</sup>+ …X<sub>n</sub><sup>2</sup> |

As with a for loop, the bottom value is the starting value, and the top value is the end value
Note that i can be replaced by any other variable name, as long as you are consistent.
By convention the variables i,j and k are often used for subscripts

### Products
- Let X be the list [x<sub>1</sub>,…,x<sub>n</sub>], then if we want multiple together all of the elements, we would use the notation:

| Product | Ouput |
|:----------:|:----------:|
| ![](https://camo.githubusercontent.com/f3aed8f7b13b4db60013efa38ce9af6d77790dcc/68747470733a2f2f6c617465782e636f6465636f67732e636f6d2f6769662e6c617465783f25323425323453253230253344253230253543646973706c61797374796c6525354370726f645f25374269253344312537442535452537424e253744253230585f69253234253234) | S = X<sub>1</sub>,X<sub>2</sub>,X<sub>3</sub>,…X<sub>n</sub> |

| Product | Ouput |
|:----------:|:----------:|
| ![](https://camo.githubusercontent.com/d17b1fd5780e08d954c627d8e0eeab197755f155/68747470733a2f2f6c617465782e636f6465636f67732e636f6d2f6769662e6c617465783f25323425323453253230253344253230253543646973706c61797374796c6525354370726f645f25374269253344312537442535452537424e253744253230585f6925323025354525374232253744253234253234) | S = X<sub>1</sub><sup>2</sup>,X<sub>2</sub><sup>2</sup>,X<sub>3</sub><sup>2</sup>,…X<sub>n</sub><sup>2</sup> |

### Factorial
- The Notation _n_! (n Factorial) is defined as multiple all of the integers between 1 and _n_ together!

| Factorial |
|:---------:|
| ![](https://media.discordapp.net/attachments/334011383140188161/447370999801970718/unknown.png?width=382&height=138)  |

| Example! |
|:---------:|
| 6! = 1.2.3.4.5.6 = 720 |

- n! also gives the number of possible arrangements of n items.
- Note that 0! = 1, undefined for n < 0

### Permutation
- The number of ways that r_ odered items can be picked from _n_ items is defined as:
![](https://cdn.discordapp.com/attachments/334011383140188161/447371765648195585/unknown.png)

### Combination
- The number of ways that _r_ unordered items can be picked from _n_ items is defined as:
![](https://cdn.discordapp.com/attachments/334011383140188161/447372090216022016/unknown.png)

### Permutations and Combinations
- If the order is important thhen we use permutations otherwise we use combinations.
- For example, if the key code to a lock is 745, then 574 would not open it!
  - Permuations, there are P<sub>3</sub><sup>10</sup> = 720 ways of choosing a 3-diget key code from the 10 digets.
- If we like a fruit salad containing banana, pear and grapes, then the order doesn't matter!
  - Combinations, there are C<sub>3</sub><sup>10</sup> = 120 ways of choosing three fruits from ten fruits.

### Floor and Ceiling Functions
#### Floor
- ⌊*x*⌋ is the largest integer less than or equal to *x*
- ⌊*x*⌋ ≤ *x*
- ⌊*17.3*⌋ = 17

#### Cieling
- ⌈*x*⌉ is the smallest integer greater than or equal to x.
- ⌈*x*⌉  ≤ *x*
- ⌈*17.3*⌉ = 18

### Logarithms
| Logarithm  | Meaning                |
|:----------:|:----------------------:|
| Log<sub>b</sub>(x)=y|x = b<sup>y</sup>|
| Log<sub>b</sub>(b)|1<br>b<sup>1</sup>=b for all b ≠ 0|
| Log<sub>b</sub>(1)|0<br>b<sup>0</sup>=1 for all b ≠ 0|
| Log<sub>b</sub>(xy)|Log<sub>b</sub>(x)+Log<sub>b</sub>(y)|
| Log<sub>b</sub>(x/y)|Log<sub>b</sub>(x)-Log<sub>b</sub>(y)|
| Log<sub>b</sub>(xy)|yLog<sub>b</sub>(x)|
| Log<sub>b</sub>(x)|Loga(x)/Loga(b)|
| Log<sub>b</sub>(x)|Log<sub>b</sub>(x) where x ≤ 0 is undefined |

- For Example:
  - Log<sub>10</sub>(1000) = 3.
  - Log<sub>2</sub>(8) = 3
- Note that:
  - if *y* = *exp(x)* then *ln(y) = x*
  - This is known as Natural Logarithm
- if *y = a<sup>x</sup>b<sup>z</sup>* Then
  - ln(*y*) = ln(*a<sup>x</sup>*)+ln(b<sup>z</sup>) = xln(*a*) + zln(*b*)

### Other topics of Mathematical Foundatation which maybe of interest:
- Probability
  - Generating 1 in n chances
- Summing Series
  - Adding up 1+2+3+4+....+n
- Summary Statistics
  - Mean, median, variance, etc...

## Time Complexity and Aymptotic notation
### Why Sorting?
- Sorting is one of the most common tasks in data analysis
  - Examples:
    - Print out a collection of employees sorted by salary
    - Print out a list of names in alphabetical order
- There are many sorting algorithms
- The Selection Sort algorithm repeatedly finds the smallest element in the unsorted tail region of an array and moves it to the front.
  - Question: How do you sort 11,9,17,5,12?

#### Selection Sort Algorithms
  - Sorting an Array of Integers...
  - Array in Original Order:
    - [11][09][17][05][12]
  - Find the smallest and swap it with the first element:
  - - [**11**][09][17][**05**][12]
    - [**05**][09][17][**11**][12]
  - Find the next smallest
    - [**05**][**09**][17][11][12]
  - It is already in the correct place.
    - [**05**][**09**][17][11][12]
  - Find the next smallest and swap it with the first element of the unsorted portion.
    - [**05**][**09**][***17***][***11***][12]
    - [**05**][**09**][***11***][***17***][12]
  - Repeat.
    - [**05**][**09**][**11**][***17***][***12***]
  - When the unsorted portion is of length 1, we are done.
    - [**05**][**09**][**11**][**12**][**17**]

### How fast is the Algorithm?
- In an array of size n, count how many primitive operations are needed.
- To find the smallest, visit n elements + 2 operations for the swap.
- To find the next smallest, visit (n-1) elements + 2 operations for the swap.
- The last term is 2 elements visited to find the smallest + 2 operations for the swap

#### The Number of Operations
  - (n + 2) + [(n-1) + 2] +[(n-2) +2] + . .. +(1+ 2) + 2
  - This can be simplified to n2/2  +  5n/2  + 2
  - 5n/2 +2 is small compared to n2/2 - so let's ignore it.
  - Also ignore the 1/2 - use the simplest  expression of the class.
  - The number of visits is of the order n2

### The Big-Oh notation
  - The number of visits is the order n<sup>2</sup>
  - Using Big-Oh Notation:
    - The number of visits is O(*n<sup>2</sup>*)

![](https://cdn.discordapp.com/attachments/334011383140188161/447384949532786688/unknown.png)

  - The Exact number of operations is not so important.
    - For n=100
      - O(n) = 100
      - O(n<sup>2</sup>) = 10000
      - O(2<sup>n</sup>) = ![](https://cdn.discordapp.com/attachments/334011383140188161/447385507245326346/unknown.png)
        - 1,267,650,600,228,229,401,496,703,205,376
        - (~1.267  1030 = 1.267E30)

### Example: Binary Search
  - Task: search for a key in a **sorted** list.
  - First check the middle list element.
  - If the key matches the middle element, we are done.
  - If the key is less than the middle Element, the key must be in the first half.
  - If the key is larger than the middle lement, the key must be in the second half.
      - Examples?
        - Spell Checkers, Phone Books, Internet Browser Cache

#### Binary Search Example
| Media | Notes: |
|:------------------------------:|:----------:|
| ![](https://cdn.discordapp.com/attachments/334011383140188161/447386533603835907/unknown.png) | Binary search is an O( log2(n) ) algorithm. </br> The Binary search algorithm is much faster that the linear search algorithm of order O(n) </br>But it only works on ordered data.... |

### Big-Oh Rules
  - If *f(n)* is a polynomial of degree *d*, then *f(n)* is O(*n<sup>d</sup>*), i.e.,
    - Drop lower-order terms.
    - Drop constant factors.
  - Use the simplest espression of the class.
    - Say "*3n + 5 is O(n)*" instead of "*3n + 5 is O(3n)*"

### Asymptotic Algorithm Analysis
  - The asymptotic analysis of an algorithm determines the running time in Big-Oh notation.
    - The word asymptotic refers to long term (large input) algorithmic trends.
  - To perform the asymptotic analysis:
   - We find the worst-case number of primitive operations executed as a function of the input size, T(n)
    - We express this function with Big-Oh notation
  - Example:
    - We have already known that the algorithm ArrayMax executes at most T(n) = 8n  5 primitive operations
    - We say that algorithm ArrayMax “runs in O(n) time”
  - Since constant factors and lower-order terms are eventually dropped, we can disregard them when counting primitive operations
    - This is why we do not have to be 100% accurate as long as we get the powers of n correct
    - I.e. we do not miscount n3 as n2 etc…
    - Confusing 7n for 5n **WILL MATTER**.

### The Classes of Algorithms
  - Algorithms are divided up into a number of classes:

| Classification | Definition |
|:--------------:|:----------:|
| Computable  | Problems that can be solved using a computer |
| Non Computable | Problems that cannot be solved using a computer |
| P Problems | Problems that can be solved in a reasonable amount of time (polynomial Time) |
| NP Problems | Problems that can sometimes be solved in a reasonable amount of time.<br>Non-Deterministic Algorithms.</br>The exhaustive search can be done in polynomial time. |
| NP-COMPLETE Problems | The hardest problems in NP. </br> The exhaustive search is not polynomial. |
| NP-HARD Problems  | Really, really difficult to solve problems, which cannot be done in a reasonable amount of time.</br> The exhaustive search is not polynomial  |

### Examples of NP-COMPLETE problems
  - The travelling salesman problem
  - Finding the shortest common superstring
  - Checking whether two finite automata accept the same language
  - Given three positive integers a, b, and c, do there exist positive integers (x and y) such that ax2 + by2 = c

### Consequences of P=NP
  - If this was found to be true, the news would make world headlines!
  - Modern society as we know it would be completely and utterly **Doomed!**
  - All passwords could be cracked in polynomial time (very, very fast)
  - You would not be able to secure any computer or device on the internet, wireless or mobile networks.....
  - Algorithms that currently take years might take minutes!
  - Proof [that NP≠P] was put forward in 2010, but has since been refuted…

### Big-Oh and Growth Rate
  - The Big-Oh notation gives an upper bound on the growth rate of a function
  - The statement “f(n) is O(g(n))” means that the growth rate of f(n) is no more than the growth rate of g(n)
  - f(n) grows no faster than g(n)
  - We can use the Big-Oh notation to rank functions according to their growth rate

### Relatives of Big-Oh

| Relative | Symbol | Summary |
|:--------:|:------:|:-------:|
| Big-Omega | Ω(g) | functions that grow at least as fast as g|
| Big-Theta | Θ(g) | functions that grow at the same rate as g|
| Big-Oh | O(g) | functions that grow no faster than g|

### Asymptotic Notation
![](https://cdn.discordapp.com/attachments/334011383140188161/447397303175610378/unknown.png)

### Why is Big-Oh the interesting one?
  - Because we are interested in efficiency, Ω(g) will not be of much interest to us because  Ω(n<sup>2</sup>) includes all functions that grow faster than n<sup>2</sup>, for example, n<sup>3</sup> and 2<sup>n</sup>
  - For a similar reason, we are not much interested in Q(g), the class of functions that grow at the same rate as the function *g*
  - Big-Oh is the class of functions that will be of the greatest interest to us
  - Considering two algorithms, we will want to know if the first is in Big-Oh of the second
  - If yes, we know that the second algorithm does not do better than the first in solving the problem

## Data Strucutres and their Applications:

### A note on Complexity
  - Regarding NP-Hard and NP-Complete problems…
    - The best algorithm to solve them is often O(2n) at best…
    - We show that a problem resembles a known NP-Complete/NP-Hard problem…
    - We then know what we are dealing with…
    - That is why in this module we will look at what might seem “toy” problems…

### Why study Data Structures?
  - Data structures are the “foundations” of all algorithms
    - Do not build on bad foundations…
  - Representing the problem you are solving correctly will vastly help in designing a solution
  - The use of the correct data structure will speed up an algorithm
    - E.g. Sorting a list of 1,000 names
      - You would use a string array rather than 1,000 string variables!

### Lists
  - A list is a sequence of zero or more data items
  - The total number of items is said to be the length of the list
  - The length of a given list can grow and shrink on demand
  - Items can be accessed, inserted, or deleted at any position in a list

#### Two ways to implement lists:
  - Array Limitation:
    - "Remember" where the end of the list is.
      - ![](https://cdn.discordapp.com/attachments/334011383140188161/447402629467734027/unknown.png)
  - Linked List implementation
    - Use a class that contians both the data and a pointer / reference to the next item in the lists.
      - ![](https://cdn.discordapp.com/attachments/334011383140188161/447402778906722314/unknown.png)
  - Both representations have their pros and cons.

### Stacks
  - A stack is a special kind of list in which all insertions and deletions take place at one end
  - This is called the top
  - It has another name: “pushdown list‘”
  - Its items are added and deleted on a **last-in-first-out (LIFO) basis**

#### Using Stacks
  - To add an item to a stack, you push an item onto the top
  - To remove an item from the top you pop it
  - In the example below the top of the stack is on the right hand side

![](https://cdn.discordapp.com/attachments/334011383140188161/447403324208185344/unknown.png)

### Queues
  - A queue is another special kind of list
    - Items are inserted at one end (the rear)
    - Items deleted at the other end (the front)
  - A queue is a FIFO type data structure
    - The items are deleted in the same order as they were added
    - On a **first-in-first-out basis**
  - For a queue structure, we have two special names for insertion and deletion:
    - **ENQUEUE**
    - **DEQUEUE**

#### Using Queues
![](https://cdn.discordapp.com/attachments/334011383140188161/447403966394007552/unknown.png)

#### How to Implement Queues
  - How do we make both the enqueue and dequeue operations efficient?
    - Avoid shifting items
  - **Enqueue**
    - tail=(tail+1) mod size
  - **Dequeue**
    - head=(head+1) mod size

![](https://cdn.discordapp.com/attachments/334011383140188161/447404393617162241/unknown.png)

### Hash Tables
  - A Hash table or Hash Map is a data structure that maps a Key to a Value
  - A special function called a Hash Function performs this mapping
  - This function usually maps the key to an index in an array

![](https://media.discordapp.net/attachments/334011383140188161/447404648848949248/unknown.png?width=492&height=213)

#### How to Implement Hash Tables
  - An initial set of space is allocated in the array
  - The hash function maps the key to an array index
  - The function should map within the array bounds
  - Care must be taken to avoid collisions
  - Different keys mapping to the same index

![](https://cdn.discordapp.com/attachments/334011383140188161/447405116333490177/unknown.png)

### Applications
  - Lists
    - Often used to implement queues and stacks
    - Used for sparse matrices
    - Matrices where most of the elements are zero…
  - Stacks
    - Expression evaluation
    - Compilers – syntax evaluation
    - Calculators employing Reverse Polish notation (ab+)
  - Queues
    - Printer queues
    - Email – message queues
    - Network routing
  - Hash Tables
    - Address books
    - Storing passwords (we don’t store the actual password)
    - Caching

### Graphs
  - We are going to look in depth at a very useful data structure
  - This is the **Graph**
  - Example of uses include:
    - Road maps
    - Project networks
    - Electrical circuits
    - Molecules
      - Relationships between genes, proteins, pathways
    - Relationships
      - Family tree
      - Students on courses

### An Abstract View of Graphs
  - A graph is a collection of nodes (**Vertices**) which may be connected in pairs by line segments called **Edges**.

![](https://cdn.discordapp.com/attachments/334011383140188161/447406196840988672/unknown.png)

### Why Study Graphs?
  - Example:
    - Airline Rout Maps - An Undirected Graph.
    - Cities - Points(Nodes, Vertex)
    - Non-Stop-Flights - lines connecting two cities (edges, arcs)

  - Computer Networks!
    - Computuers - Points (Nodes, Vertex)
    - Cables - Lines connecting two computers (edges, arcs).

  - What are the possible tasks of graphs!
    - Shortest Cables,
    - Lowest Costs
    - Quickest Delivery
    - Reliable
    - Fault-Tolerant
      - Many many more applications (tube, sat-nav).

### How can graphs help?
  - Questions
    - What is the cheapest way to fly from London to Rome?
    - Which route has the least flying time?
    - If Heathrow is closed by bad weather, can you still fly between every other pair of cities, such as Edinburgh-Rome, Manchester-Rome?
    - If one computer in a network goes down, can email be sent between every other pairs of computers in the network?
  - Graph algorithms can solve the above problems!

### How to define a graph?
  - What are the basic components of a graph?
  - A graph G = (V,E) is composed of:
    - V: a set of vertices or nodes
    - E: a set of edges or lines connecting the vertices in V
    - An edge e=(u,v) is a connection between the vertices u and v
  - In the example below:
    - V={1,2,3,4,5}
    - E={(1,2),(1,3),(3,5),(2,5),(5,4)}

![](https://cdn.discordapp.com/attachments/334011383140188161/447457398618324992/unknown.png)

### Graph Definitions
#### Directed Graphs
  - A Directed graph is a pair G=(*V,E*)
  - Where V is the set of vertices, and E is a set of ordered pairs of elements of V
  - For directed edges (v, w) is in E, v is tail, w is head
  - It can be represented as v -> w or vw

![](https://cdn.discordapp.com/attachments/334011383140188161/447458122748002305/unknown.png)

#### Undirected Graphs
  - An undirected graph is a pair G=(V, E), where E is a set of unordered pairs of distinct elements of V
  - For undirected graphs, vw = wv

![](https://cdn.discordapp.com/attachments/334011383140188161/447458450138726410/unknown.png)

#### Complete Graphs
  - A complete graph is normally an undirected graph with an edge between each pair of vertices
  - G=(V, E)
  - ∀e ∈ V*x*V -> e ∈ E
    - We've not covered this but "*∀*" means "for all" but is also a symbol for "Universal Quantifier".

![](https://cdn.discordapp.com/attachments/334011383140188161/447459736229773332/unknown.png)

#### Paths
  - A sequence of k vertices, [v<sub>1</sub>, v<sub>2</sub>, ..., v<sub>k</sub>], such that any pair of consecutive vertices, v<sub>i</sub>, v<sub>i+1</sub> are adjacent (connected by an edge) is called a **path** (sometimes called a **walk**).
  - [1,2,3,4,5] is a path.
  - [1,5,2,4] is not a path.
  - [1,2,3,1] is a path that contains a **cycle**.

![](https://cdn.discordapp.com/attachments/334011383140188161/447460564952940575/unknown.png)

#### Connectivity
  - n undirected graph is connected if and only if for each pair of vertices v and w, there is a path from v to w
  - A directed graph is strongly connected if and only if for each pair of vertices v and w, there is a path from v to w

#### Weighted Graph
  - A weighted graph is a triple G=(V, E, W)
  - Where W:E -> R
  - W(e) is called the weight of edge e

### Connected Graph
![](https://cdn.discordapp.com/attachments/334011383140188161/447461083255668739/unknown.png)

### Weighted Graph
![](https://cdn.discordapp.com/attachments/334011383140188161/447461315901128704/unknown.png)

### How to Represent a Graph
  - We often represent a graph as a matrix (2D array), although other data structures can be used depending on the application
  - If we have N nodes to represent
    - For an N by N matrix G, a non zero value of g<sub>i</sub><sub>j</sub> (ith row, jth column of G) means there is an edge between node i and j
  - Undirected
    - We assume that g<sub>i</sub><sub>j</sub> is the same as gji
  - Directed
    - g<sub>i</sub><sub>j</sub> is not always the same as gji
  - Non-weighted
    - g<sub>i</sub><sub>j</sub> is either one for an edge or zero for no edge
  - Weighted
    - g<sub>i</sub><sub>j</sub> is the edge weight or zero for no edge
  - Complete
    - g<sub>i</sub><sub>j</sub> is never zero

### Trees
  - These are a special graphs without cycles
  - Hieratical graph
  - Root
    - The only node at the topmost part of the tree
  - Child nodes have parents
  - All of the rest of the nodes must be linked to a parent note, and may have zero or more child nodes
  - Leaf
    - A Node without children

![](https://cdn.discordapp.com/attachments/334011383140188161/447463143741063168/unknown.png)

  - A binary tree is a special type of tree where the maximum number of children is two
  - Trees are usually ordered from the top to the bottom and left to right
  - The height of a tree is the number of levels
  - Trees are very fast to search
    - Binary search
  - Trees can be implemented in a manner similar to a linked list, but each node can point to two (or more) other nodes
  - There are a very large number of applications of trees
    - Spell checkers
    - Parse trees in compilers
    - Computer file systems
    - Organisational structures and hierarchies
    - Gene ontology data (functional relationships)
      - Etc...

  - We assume, when searching Trees that the left side elements are before the parent in terms of value, such as alphabetical order.
  - We assume Right Side elements are higher value or "after" the parent.

  - To add a node, we first search for the node we are adding
    - Searching for Stan
      - Start at the root node Mary
      - Greater than Mary, move to Tina
      - Less than Tina, move to Paul
      - Greater than Paul, no right node, failure to find key...
  - Now we add the node where we expected to find it
    - Deleting is more difficult...
    - What if we delete Mary?

![](https://cdn.discordapp.com/attachments/334011383140188161/447464377122160660/unknown.png)

  - Trees can become unbalanced
  - Especially if we add and remove a large number of nodes
  - The height of the tree can grow until the tree becomes a **linked list**
  - Special types of self balancing trees have been developed
    - AVL, Red-Black, etc…

## Classic Algorithms - Sorting
### What Sorting Algorithms?
  - Bubble Sorting
  - Quick Sorting
  - Radix Sorting
    - And others.

### A nate of Growth Rates
![](https://cdn.discordapp.com/attachments/334011383140188161/447468028678897684/unknown.png)

  - A plot of n against a number of possible T(n)
  - The y axis is in logarithmic scale so that all the data can be viewed
    - I am using log base 10, but often log base 2 is used
  - When n = 100
    - log(n) = 2, n = 100, nlog(n) = 200, n2 = 10,000 and n3 = 1,000,000

### Why Sorting?
  - Sorting applications are one of the most common algorithms
  - There are implemented in computer games, network routing software, operating systems, AI algorithms, bin packing algorithms, etc….
  - The sorting problem itself is easily understood
    - It does not require a large amount of background knowledge before you can start implementing it
  - The algorithms are quite small and manageable
    - They can be implemented in a short period of time
    - They are relatively simple to analyse

### Formal Definition of sorting
  - The sorting problem is a mapping from x to y, where
    - x and y are both n length real vectors (lists and/or arrays)
    - x is a permutation of y (different ordering)
    - y<sub>i</sub> < y<sub>i+1</sub> for all i=0,...,n-1
  - All of the algorithms will apply to whether we want the list sorted from largest to smallest.
  - The algorithms can easily be applied to integers or character vectors
    - Sorting whole numbers
    - Sorting names and/or addresses

### Bubble Sorting
  - How do we sort the list?
  - Apart from selection sort is there any other obvious way?
  - Directly from the formal definition of sorting we can see that for a sorted list, any adjacent elements are in order
  - So what about comparing each pair of neighbouring elements and swap them if there are any out of order?
  - _This is the idea of the Bubble Sort_
    - Why “bubble”?

![](https://cdn.discordapp.com/attachments/334011383140188161/447469606580256778/unknown.png)

### Bubble Sort: An Example
  - Observations:
    - After the first pass, the list has not been sorted yet!
    - 8 (or n-1) comparisons have been made!
    - The largest element (the bubble), 9, has been moved to the end!
    - The smaller elements have been shifted towards to the beginning

  - Questions:
    - How many elements do we need to sort in the next pass?
    - When will the sort algorithm stop?
    - What about the best case? How many passes?
    - What about the worst case? How many passes?

![](https://media.discordapp.net/attachments/334011383140188161/447469954782986260/unknown.png)

  - Overall Result:
![](https://cdn.discordapp.com/attachments/334011383140188161/447470832940351518/unknown.png)

### Bubble Sort Summary
  - If we compare pairs of adjacent elements and none are out of order, the list is sorted
  - If any are out of order, we must have to swap them to get an ordered list
  - Bubble sort will make passes though the list swapping any elements that are out of order
  - After the first pass, we know that the largest element must be in the correct place
  - After the second pass, we know that the second largest element must be in the correct place
  - Because of this, we can shorten each successive pass of the comparison loop

### Bubble Sort
```Java
Algorithm 1. BubbleSort(x)
Input: x - a list of n numbers
 1) Let NoSwaps = False
 2) While NoSwaps = False
 3)    Let NoSwaps = True
 4)    For i = 0 to n-2
 5)       If xi > xi+1 then
 6)          Swap xi and xi+1
 7)          Let NoSwaps = False
 8)       End If
 9)    End For
10) End While
Output: x – sorted (ascending)
```

  - The algorithm works by running through the list of numbers, swapping pairs that are out of order
  - The algorithm terminates when no swaps need to be made
  - Smaller numbers “bubble” to the top whilst larger numbers sink to the bottom
  - Line 5 needs changing to < in order to get the algorithm to sort the list in descending order
  - Note: to fit the pseudo code onto one slide, I have not reduced the list size by one each iteration…

### Best-Case Analysis
  - If the elements are in sorted order at the start, the for loop will compare the adjacent pairs but not make any changes
  - This means that the `NoSwaps` variable will remain `true`
  - The `While` loop is only done once
  - There are n-1 comparisons in the best case
  - B(n)≡O(n)

### Worst-Case Analysis
  - If in the best case the while loop is done once, in the worst case the while loop must be done as many times as possible
  - This will be when the data is in **reverse order**
  - Each pass of the For loop must make at least one swap of the elements
  - The number of comparisons will be:

![](https://cdn.discordapp.com/attachments/334011383140188161/447472176443031554/unknown.png)

### Average-Case Analysis
  - Much more difficult…
  - How many passes do we need?
  - We can potentially stop after any of the (at most) n-1 passes of the For loop
  - This means that we have n-1 possibilities
  - Our average case is given by

![](https://cdn.discordapp.com/attachments/334011383140188161/447472477522624542/unknown.png)

  - Where C(*i*) is the word done in the first *i* passes.

  - On the first pass, we do n-1 comparisons
  - On the second pass, we do n-2 comparisons
  - The number of comparisons in the first i passes, in other words C(i), is given by:

![](https://cdn.discordapp.com/attachments/334011383140188161/447472913612800001/unknown.png)

  - Putting the equation for C(i) into the equation for A(n) we get:

![](https://cdn.discordapp.com/attachments/334011383140188161/447473081498337281/unknown.png)

### Quick Sort
  - Quicksort is a divide and conquer algorithm
  - Quicksort picks an element from the list as the pivot, and partitions the list into two pieces:
    - Those elements smaller than the pivot value (not necessarily in order)
    - Those elements larger than the pivot value (not necessarily in order)
  - Quicksort is then called recursively on both pieces

### Quick Sort Example
![](https://cdn.discordapp.com/attachments/334011383140188161/447473521879285760/unknown.png)

![](https://cdn.discordapp.com/attachments/334011383140188161/447473715748405248/unknown.png)

### The Quick Sort Algorithms
#### The Quick Sort Algorithm
```Java
Algorithm 2. QuickSort(List,First,Last)

Input: List, the elements to be put into order
       First, the index of the first element
       Last, the index of the last element

1) If First < Last Then
2)    Let Pivot = PivotList(List,First,Last)
3)    Call QuickSort(List,First,Pivot-1)
4)    Call QuickSort(List,Pivot+1,Last)
5) End If

Output: List in a sorted order
```

#### The PivotList Algorithm
```Java
Algorithm 3. PivotList(list,first,last)

Input: List- the elements to be put into order
       First- the index of the first element
       Last- the index of the last element

1) PivotValue = list[first]
2) PivotPoint = first
3) For index = first+1 to last
4)    If list[index] < PivotValue Then
5)       PivotPoint=PivotPoint+1
6)       Swap(list[PivotPoint],list[index])
7)    End if
8) End For
9) Swap(list[first],list[PivotPoint])

Output: PivotPoint
```

  - Pick the First Element as the Pivot.
  - Set the Pivot Point as the first location of the list.
  - Move through the list comparing the pivot element to the rest.
  - If an element is smaller, increase the Pivot Point.
  - Swap this element into the new Pivot Point Location.
  - Move Pivot Value into the correct place.

### Worst-Case and Best-Case Analysis
#### Worst Case
  - In the worst case, `PivotList` will do n-1 comparisons, but creates one partition that has n-1 elements and the other will have no elements
    - When will this happen?
  - Because we wind up just reducing the partition by one element each time, the worst case is given by:

![](https://cdn.discordapp.com/attachments/334011383140188161/447475071024627712/unknown.png)

#### Best Case
  - `PivotList` creates two parts that are the same size
  - And then all subsequent parts are the same size as the algorithm calls itself, this can be modelled as a binary tree
  - Summing up over the partitions we get B(n)=O(nLog2(n))

### Average-Case Analysis
  - In the average case, we need to consider all of the possible places where the pivot point winds up
  - Because for one partition of the list, there are n-1 comparisons done, and there are n ways to partition the list, we have:

![](https://cdn.discordapp.com/attachments/334011383140188161/447475578866499595/unknown.png)

- Algebra can be used to simplify this recurrence relation to:

![](https://cdn.discordapp.com/attachments/334011383140188161/447475788246417410/unknown.png)

- This will then solve to:

![](https://media.discordapp.net/attachments/334011383140188161/447475926075441162/unknown.png?width=303&height=44)

- Therefore, A(n)≡O(nLog<sub>2</sub>(n))

### Comparison of Sorting Algorithms

| Method | Best | Average | Worse |
|:------:|:------:|:------:|:------:|
| Bubblesort | O(n) | O(n<sup>2</sup>) | O(n<sup>2</sup>) |
| Insertion Sort | O(n) | O(n<sup>2</sup>) | O(n<sup>2</sup>) |
| Mergesort | O(*n*Log<sub>2</sub>(*n*)) | O(*n*Log<sub>2</sub>(*n*)) | O(n<sup>2</sup>) |
| Selection Sort | O(n<sup>2</sup>) | O(n<sup>2</sup>) | O(n<sup>2</sup>) |

### Radix Sort
  - The Radix sort method works only on binary or integer data
  - In a computer all numbers are represented as binary
  - Radix sort works by using a binary bucket sort for each binary digit
  - We first sort by the least significant bit 2<sup>0</sup>, then 2<sup>1</sup>, 2<sup>2</sup>, 2<sup>3</sup>, …
  - Integers in Java have 32 bits (or 64…)

```Java
Algorithm 4. RadixSort(List,Bits)
Input: List- the elements to be put into order
       Bits- the numbers of bits of each List[i]

1) For i = 0 to Bits-1
2)    Let b = 2i
3)    Bucket sort list on bit mask b
4) End If

Output: list in a sorted order
```

- Bucket sorting into two buckets involves dividing the data into two lists (for each 0 and 1)
- The two lists are then merged
- The ordering of the data as they are put in each bucket must be maintained

- The Radix sort takes O(*nb*) time complexity
  - n is the numbers items
  - b is the numbers of bits
  - Best, worse and average case
- Can be used for alphabetical sorting, i.e. strings
- It is very, very fast!

## Classic Algorithms - Graph Traversal

### What is "Search" in Graphs?
  - When we work with graphs, we often wish to do something to each node in the graph exactly once
  - Visit each node once and only once
  - Examples:
    - A piece of information that needs to be distributed to all the computers on a network
    - Look for information among computer in a network

### What is "Depth-First"?
  - Depth-First: the traversal will go as far as possible down a path until a **“Dead End”** is reached
  - Dead End:
    - In an undirected graph:
      - A node is a dead end if all of the nodes adjacent to it have already been visited
    - In a directed graph:
      - If a node has no outgoing edges, it is called a dead end

### What is "Depth-First Search"?
  1. We visit the starting node and then proceed to follow links through the graph until we reach a dead end
  2. We then back up along our path until we find an unvisited adjacent node, and continue in that new direction
  3. The process completes when we back up to the starting node and all the nodes adjacent to it have been visited
  4. If presented with two choices, we choose the node with numerically and alphabetically smaller label (just for convenience)

### DFS Undirected graphs
![](https://media.discordapp.net/attachments/334011383140188161/447492572848324608/unknown.png?width=268&height=293)
![](https://media.discordapp.net/attachments/334011383140188161/447492698375716881/unknown.png?width=322&height=295)
![](https://cdn.discordapp.com/attachments/334011383140188161/447492888616632320/unknown.png)
![](https://cdn.discordapp.com/attachments/334011383140188161/447493006862450689/unknown.png)
![](https://cdn.discordapp.com/attachments/334011383140188161/447493154514403339/unknown.png)

  - We continue to back up, without visiting notes 4,3,2, until we reach the starting node
  - Since all nodes adjacent to node 1 have been visited, we are done
  - The order that the nodes are visited: 1,2,3,4,7,5,6,8,9

![](https://cdn.discordapp.com/attachments/334011383140188161/447493371209187329/unknown.png)

  - Starting from the node 1, what is the order that the nodes will be first visited?
    - 1,4,2,3,7,6,5

![](https://cdn.discordapp.com/attachments/334011383140188161/447493569524006912/unknown.png)

  - The order that the nodes will be first visited:
    - 1,2,3,4,6,5,7
  - If undirected:
    - 1,2,3,4,5,6,7

![](https://cdn.discordapp.com/attachments/334011383140188161/447493781843869740/unknown.png)

  - The order that the nodes will be first visited:
    - 1,2,3,7,4,6,5
  - If undirected:
    - 1,2,3,4,5,6,7

### Algorithhm: DFS(G, n)
```Java
Algorithm 1. DFS(G,n)

Input: G- the graph
       n- the current node

1) Visit(n) [Do something to/at node n...]
2) Mark(n)
3) For every edge nm (from n to m) in G do
4)    If m is not marked then
5)       DFS(G,m)
6)    End If
7) End For

Output: Depends on the purpose of the
        search...

```

### DFS RUnning Time Analysis
- Remember:
    - DFS is called on each node exactly once
    - n nodes : O(n)
    - Every edge is examined exactly twice, once from each of its vertices/nodes
  - m edges: O(2m)
- O(n) + O(2m)  O(n+m)
- If we assume that the work done as we visit each node is the most complex part of the process, the traversal is of order O(n)

### Other Types of Graphs
	- There are other ways to search a graph other than visiting all nodes
	  - Finding a path between two nodes
	  - Finding the shortest path between two nodes (number of edges)
	  - Finding the cheapest path between two nodes (a function of edge weight)

### The Exhaustive Searching
  - The exhaustive search systematically evaluates every possible path in a graph
  - This methods is guaranteed to find the what we are looking for
  - However this method is unsuitable for most real world problems
    - The time it takes to search all possible paths is combinatorial explosive as the number of nodes and edges increase

### Algorithm: Exhaustive(G, n, p)
```Java
Algorithm 2. Exhaustive(G, n, p)

Input: G- the graph
       n- the current node
       p– the path so far

1) For every edge nm (from n to m) in G do
2)    If m  p then
3)       p = p  {m}
4)       Exhaustive(G, m, p)
5)    End If
6) End For

Output: Depends on the purpose of the
        search...
```

### Exhaustive Running Time
- This is very complicated to compute
- It depends on how the nodes and edges are organised
- If we look at the worse case, that of a complete graph:
  - Here all the nodes are connected to each other
  - For the first node in the path there are n-1 edges to follow
  - For the second, n-2
  - For the third, n-3, ...
  - Hence we get (n-1)(n-2)(n-3)...1 = O((n-1)!)

### Bredth-First Searching
  - This search method considers neighbouring nodes first
    - All the neighbours of the start node are expanded first
    - Then the neighbours of the neighbours
    - Until the goal state is found
  - This search is very expensive since all the partial paths being considered must be stored
  - Similar to depth-first search, breadth-first search will eventually find a path to the goal, but it may not be the best path
  - The algorithm is similar to the exhaustive search algorithm, but it stops when the goal node is reached
    - Exhaustive generates all paths

### Best-Fit Search
  - Best-first search is an improvement upon depth-first search
  - A heuristic is used to decide which node is explored next
    - A **heuristic** is a rule of thumb or best practice
    - We will look at heuristics in much more detail later
  - For example nodes are expanded in order of lowest cost

### A* Search
  - The A* (A Star) search method is an example of a best-first search
  - Very good for route finding applications
    - The AA website
    - The tube
  - In order for the search to work, two estimates must be available
    - How much a partial path has cost
    - An estimate (an under estimate) of how far is left to the goal state
    - E.g. a lower bound on how far to travel
  - The A* algorithm will find an optimal path without necessarily considering all the routes

  - The algorithm scores each partial path with the following function: **f = g + h**
  - Where **g** is the cost so far and **h** is the estimate of the cost to the goal state. (E.g. as the crow-flies distance)
  - If **h** is always zero (i.e. we do not have any information about how far away the goal is), then the algorithm becomes similar to depth-first search
  - If g is always zero, then the algorithm is called a **Greedy Search**

### The A* Algorithm
```Java
Algorithm 3. AStar(G,S,E)

Input: G- The graph being searched
       S- The start node
       E- The goal node

1) Let P be a list of routes, currently empty,
   this set is ordered on f, with the head of P
   being the smallest value in f
2) Expand all one step nodes leading from S,
   and add them to P (ordered on f)
3) While P ∉ ∅ and E not reached by head of P
   Expand the head of P and add them to P
5)    Order P according to f
6) Wend

Output: Head of P if it exists
```

### A* Search
  - Consider the following Graph / Map:

![](https://cdn.discordapp.com/attachments/334011383140188161/447670881184120833/unknown.png)

  - Expand S – two choices
    - [S,A] f=1+5=6
    - [S,B] f=2+6=8
  - Expand [S,A] – two choices
    - [S,B] f=2+6=8
    - [S,A,X] f=(1+4)+5=10
    - [S,A,Y] f=(1+7)+8=16
  - Expand [S,B] – two choices
    - [S,A,X] f=(1+4)+5=10
    - [S,B,C] f= (2+7)+4=1
    - [S,A,Y] f=(1+7)+8=16
    - [S,B,D] f= (2+1)+15=18
  - Expand [S,A,X] – one choice (E - GOAL!)
    - [S,A,X,E] is the best path... (costing 7)

### Minimum Spanning trees
  - A spanning tree is a sub-graph that is also a tree (no cycles) that contains all of the nodes of the super-graph
    - The super-graph is usually a complete graph
    - The edges can only come from the super-graph
  - A graph may have many spanning trees
  - The cost of a spanning tree is the sum of all the edge weights
  - A minimum spanning tree (MST - there may be many) is the spanning tree with the minimum cost
    - For n nodes there will be n-1 edges [retained/copied]…

### Prim's Algorithm for most
```Java
Algorithm 4. PrimsMST(G=(V,E))

Input: G- a weighted graph (V- vertices, E- Edges)

1) Let x be a random node from V
2) Let Vnew = {x}
3) Let Enew = {}
4) While Vnew  V
5)    Choose an edge (u,v) with minimal weight,
      such that u  Vnew and v  Vnew
6)    Vnew = Vnew  {v}
7)    Enew = Enew  {(u,v)}
8) Wend

Output: Gnew = (Vnew,Enew)
```
  - Complexity O(*n<sup>2</sup>*) where *n* is the number of nodes.

### Prim's Algorithm Example
  - Before MST:
![](https://media.discordapp.net/attachments/334011383140188161/447672591298068481/unknown.png?width=178&height=168)

  - After MST:
![](https://media.discordapp.net/attachments/334011383140188161/447672840842379285/unknown.png?width=183&height=178)

  - Method:
    - Randomly choose A
    - Vnew={A}
    - Enew={}
    - Select (A,B) (1)
    - Vnew={A,B}
    - Enew={(A,B)}
    - Select (A,C) (2)
    - Vnew={A,B,C}
    - Enew={{A,B),(A,C)}
    - Select (C,E) (1)
    - Vnew={A,B,C,E}
    - Enew={{A,B),(A,C),(C,E)}
    - Select (E,D) (2)
    - Vnew={A,B,C,E,D}
    - Enew={{A,B),(A,C),(C,E),(E,D)}

### Applications for MST
  - Cancer imaging
    - The British Columbia Cancer Research centre uses them to describe the arrangements of nuclei in skin cells
  - Detecting actin fibres in cell images
    - A biomedical image analysis application
  - CfA redshift survey
    - MSTs used for understanding the large-scale structure of the universe

### Other "Famous" Graph algorithms
  - Dijkstra's algorithm
    - Shortest path algorithm similar to A*
    - Given a start and a goal the algorithm finds the shortest path between the two points by computing a series of shortest paths
    - Used in network routing
    - Complexity O(n2) where n is the number of nodes
  - Floyd–Warshall algorithm
    - This algorithm computes how far each node is from every other node
    - Computes 1-step paths, 2-step paths, etc...
      - Is it shorter to go to a node via a node rather than directly to it?
    - It does not return the paths
    - Complexity O(n3) where n is the number of nodes

### Brief look at Floyd-Warshall
```Java
Algorithm 5. FW(D)

Input: D, an n by n matrix representing distance
          pairs between nodes, if there is no edge
          then dij = + (large values are poor)

1) Let P = D
2) For i = 1 to n
3)    For j = 1 to n
4)       For k = 1 to n
5)          pij = Min(pij,pik+pkj)
6)       End For
7)    End For
8) End For

Output: P, the shortest paths between all nodes
```

## Search Algorithms, Representation, Fitness and Fitness Landscapes.

### Definition of a Search Problem:
  - For some problems we need to search for a solution from a (usually) very large number of possibilities
    - **Search problems**, i.e. searching for the answer in some solution space
  - The solution spaces for many every day problems can be very, very large, too large to search exhaustively [see last lecture…]
  - We often need special search algorithms known as meta-heuristics

### What is a Heuristic?
  - A heuristic is a “rule of thumb” or some loose set of guidelines
    - Getting out of a maze by keeping your hand against the maze wall
  - Artificial Intelligence these are used to improve the performance of methods, in our case, search methods
    - Expert knowledge
    - Common sense

### Search Problems
  - Many problems can be thought of as searching through candidate solutions to find one that is optimal
    - Systematically search through potential solutions without considering all of them…
  - Need some way to evaluate the fitness of the candidate solutions
    - Optimal = fittest
  - Some sense of the adjacency (similarity) of solutions (or neighbourhood)

### Fitness
  - In order to search for a solution we must be able to compare potential solutions
  - E.g. Is solution s1 better than solution s2?
    - Thus we have the concept of fitness
  - We must derive a function (the fitness function) that maps a solution to a value that rates how good the solution solves the problem in hand
  - The **fitness** of a solution
  - We either try and **maximise** or **minimise** the fitness
  - A slight change in solution quality should result in a corresponding change in the fitness
    - Solution quality goes down  Fitness goes down (decreases)
    - Solution quality goes up  Fitness goes up (increases)

### Fitness Landscapes
  - It can be helpful to think of searching a landscape of solutions where:
    - The x and y co-ordinates represent a particular solution
    - Altitude (z axis) represents the fitness of that solution
  - This leads to the analogy that we wish to search for or climb peaks (or descend…)
  - Describing the nature of a landscape characterises (in an abstract way) classes of problem
  - Search methods usually explore solutions over several variables or features
      - E.g. searching gene expression data can involve searching over thousands of variables
  - The collection of all possible solutions can be considered as a high dimensional space, called the **search space** or **fitness landscape**
  - Often some concept of distance between solutions exists and some concept of how “good” each point in the search space is (fitness/objective function)
  - Techniques exist to map a high dimensional space to a two dimensional space so we can plot the space/landscape

- Smooth and regular spaces are easy to search:
![](https://cdn.discordapp.com/attachments/334011383140188161/447678865335386112/unknown.png)

- Irregular Spaces are difficult to search:
![](https://cdn.discordapp.com/attachments/334011383140188161/447679083006918667/unknown.png)

### Global and Local Optima
  - The **global optimum** is the point or points in the search space with the best objective function evaluation
  - A **local optimum** is the point or points in a subset or section of the search space  with the best objective function evaluation
  - Note that the subset or section of the search space in question may contain the global optima
  - Many search techniques can find local optima, but get “stuck” at them and cannot move on to find the global optima
  - E.g. Random Mutation Hill Climbing

### Representation
  - When we are trying to solve a search based problem we need a way to represent a potential solution
  - This is usually a mathematical and/or data structure based way of describing the solution to a problem
  - A good representation:
    - Should be a one to one mapping
    - No redundancy
    - No ambiguities
    - All potential solutions should be represented

### The Scales Problem
  - We are going to spend some time looking at a particular problem in detail
  - We are going to design the fitness function for this problem and use it in a number of worksheet exercises
  - The aim is to see how a number of different heuristic search methods perform against this problem

```
  Given n objects of various weights,

  split them into two equally heavy piles

  (or as equal as possible)
```

## Heuristic Search, Hill Climbing and Simulated Annealing

### Heuristic Search
  - Recall that some (if not all) difficult problems (NP-Hard) cannot be solved in a straight forward manner
  - We need to develop approximation algorithms to solve these problems
  - A type of method called **Heuristic Search** can be used to try and find a solution
  - We search for the best solution from a very large number of potential solutions
  - We score the worth of each solution using a **Fitness Function**
  - We try and find a solution that minimises or maximises the fitness
    - Depending on how we rate the solution
  - The computational complexity of Heuristic search methods is often very difficult to define
  - We therefore often rate their performance in terms of the number of fitness function calls
    - We compute the Big-O of this function…
  - We aim to choose the method that finds us the global optimum in the smallest number of fitness function evaluations
    - However back in the real world...

### There is no Free Lunch!
  - There is a theorem in heuristic search called the        No Free Lunch Theorem
    - This is not a joke!
  - This theorem states that just because method X is great at solving problem Y it might be no use at solving problem Z
  - Even if problem Y and Z are very, very similar...
  - This makes our lives as implementers of these types of algorithms rather difficult
  - The correct use of heuristic search methods is almost like an “art”

### Random numbers
  - A random number is a number chosen/generated by chance
  - A uniformly distributed real valued random number between **a** and **b** has equal chance of assuming any of the values between **a** and **b**
    - We use the notation `UR(a,b)`
    - We use `UI(a,b)` for uniformly distributed random integers
  - If an event has a x% chance of occurring then we generate `UR(0,1)` and see if it less than x/100
    - 83.2% is equivalent to 0.832-
  - Check that `UR(0,1)` < 0.832 for the event to occur
  - We need random numbers for various search based methods
  - Some of these methods decide on what action to do based on random numbers
  - This is rather like tossing a coin to decide on which way to go
  - Methods based on generating random numbers are often referred to as **Stochastic** and/or **Monte-Carlo** methods

  - The function `UR(a,b)` canbe implemented in Java as follows:
```Java
import java.util.*;
public class HCSA
{
   static private Random rand = null;
   static public void main(String args[])
   {
      for(int i=0;i<10;++i) System.out.println(UR(3,4));
   }
   static public double UR(double a,double b)
   {
      if (rand == null)
      {
         rand = new Random();
         rand.setSeed(System.nanoTime());
      }
      return((b-a)*rand.nextDouble()+a);
   }
}
```

### The Exponential Function
  - The exponential function, exp(x), is a mathematical function that is very important in all areas of mathematics
  - This function raises the mathematical constant e to the power of **x**
    - `e = exp(1)` = 2.718... (infinite number of decimal places [d/p])
    - `exp(-2)` = 1/e2 = 0.135 (3 d/p)
    - e has an infinite number of decimal places and is a **Transcendental** number, as is π
    - All possible sequences will eventually occur…
    - For example the sequence 230612 appears at position 537,886 (decimal point)…
    - You call it in Java by using the Math.exp(x) function
  - This function is used in the Stochastic Hill Climbing and Simulated Annealing algorithms

### Random Mutation Hill Climbing
  - The Random Mutation Hill Climbing (RMHC) algorithm is an iterative search methods that aims to find a point in the search space that maximises some objective function (fitness)
  - The RMHC algorithm starts off at some **random** point in the search space
  - It then looks randomly at its **close neighbours** until it find one with a **better** fitness
  - The hill climbing algorithm then continues searching for improvement from this **new point**
  - The idea is that the algorithms locates points that lead up (or down) a slope in the fitness space
  - This is rather like the analogy of a hill walker trying to climb up a hill in the fog
  - They feel around themselves until they find a nearby direction that goes up
  - They then move to this higher point and continue searching
  -  The RMHC is implemented in Java as follows:

```Java
Algorithm 1. RMHC(ITER)

Input: ITER- the number of iterations to run for

1) Let S be a random point in the search space,
   let F be its fitness
2) For i = 1 to ITER (number of iterations)
3)    Let S’ be a random point close to S,
      Let F’ be its fitness
4)    If F’ is better than F Then
5)       Let S = S’ and Let F = F’
6)    End If
7) End For

Output: S- a solution
```

- The hill climbing algorithm can easily get "stuck in local optima":

![](https://cdn.discordapp.com/attachments/334011383140188161/447684556351471627/unknown.png)

- From the starting point, the algorithm will never reach the global optima

### Random Start and Small Change Pseudocode:
```Java
Algorithm 2. RandomStart(n)

Input: n- the number of weights
1) Let S be a n length binary string (or array)
2) For i = 1 to n
3)    Let si = |Random Integer| Mod 2
4) End For

Output: S- a random solution to the Scales Problem
```
```Java
Algorithm 3. SmallChange(Sold)

Input: Sold- A binary string of length n
1) Let S = Sold
2) Let i be a random integer between 1 and n inclusive
3) If si = 0 Then Let si = 1 Else Let si = 0

Output: S- a solution to the Scales Problem close to Sold
```




### Stochastic Hill climbing
  - The RMHC algorithm can have very variable performance
  - We need to improve upon it to escape local optima
  - We can do this by letting the algorithm accept worse fitness function values during its search
  - This is the basis of the Stochastic Hill Climbing (SHC) algorithm
    - The chance of accepting is a function of how bad the change is
    - A very bad change will have a small chance of being accepted
    - A slightly bad change will be accepted more often
    - There are many ways of doing this, the example **decision** function in the next slide is just one of these ways…

  - We accept (line 4 in the RMHC algorithm) a new solution according to the following equation:

![](https://cdn.discordapp.com/attachments/334011383140188161/447686716481077248/unknown.png)

  - Here:
    - f<sup>n</sup> is the new fitness (line 3 in the RMHC algorithm)
    -f is the old fitness
    - T is a parameter (set to 25 for the 1,000 primes scales problem)
  - The correct choice of T can be **very** difficult...
  - Note that f<sup>n</sup> and f should be “swapped” (order) for a maximisation problem
  - We get an average best of 8.0
    - 10 runs of 1,000 iterations as in the RMHC example

### Random Restart Hill Climbing
  - A very effective version of the Hill Climbing algorithm is the Random Restart (RRHC) version
  - Here we run the normal RMHC algorithm a number of times and record the best
    - I.e. we start off in different sections of the search space
    - For example we might run it 10 times for 100 iterations rather than once for 1,000 iterations
  - For our Scales example we get an average best of 6.2
    - 10 runs of 10*x*100 iterations

### Simulated Annealing
  - Simulated Annealing is another attempt to improve the Hill Climbing algorithm
  - It allows a worse solution to be accepted so that local maximums can be circumnavigated
    - Under certain conditions - similar to SHC
  - The term “annealing” refers to the fact that the chance of accepting a worse solution reduces as the algorithm progresses
    - An analogy to the annealing process in metal work
    - A function of the iteration count
  - The annealing process is simulated through maintaining a decreasing temperature
  - This temperature should have reached zero at the end of the algorithms run
  - Note that the parameters T0 and λ need defining, along with the acceptance function PR
  - Note that if ITER is known (this is a user defined parameter that determines how long the algorithm runs for) then we can calculate a value for λ
  - For TITER we choose a small value greater than zero, e.g. 0.001

![](https://cdn.discordapp.com/attachments/334011383140188161/447688157258055700/unknown.png)

  - So now we only have two parameters to determine, T0 and ITER
  - ITER can be selected by trial and error, the algorithm is very fast so we can select a large value and reduce it if necessary
    - E.g. 1,000 in our 1,000 Primes Scales example
  - Determining T0 can be a problem
  - Too small and the algorithm will behave like a hill climber
  - Too large and the algorithm may never converge
  - There are some quite **complex** methods however…
  - The acceptance function PR is defined as follows

![](https://cdn.discordapp.com/attachments/334011383140188161/447688438158721024/unknown.png)

  - Note that |x| means the absolute value of x, and equals –x if x <0 or x if x ≥ 0

### SA Convergence  Graph
  - Averaged over 10 runs, note that this is a plot of current fitness and not the best

![](https://cdn.discordapp.com/attachments/334011383140188161/447688856515510273/unknown.png)

### A noteabout HC and SA
  - All of the HC and the SA algorithm search for a good solution by starting at a random point and then examining neighbouring points
  - This type of search is known as a **local or neighbourhood search methods**
  - Later on in this module we will look at a number of global search methods that are based on maintaining a population of potential solutions

## The Simulated Annealing Algorithm
```Java
Input: T0 Starting temperature
Iter Number of iterations

λ) The cooling rate

1)	Let x = a random solution
2)	For i = 0 to Iter-1
3)		Let f = fitness of x
4)		Make a small change to x to make x’
5)		Let f’ = fitness of new point x’
6)		If f’ is worse than f Then
7)			Let p = PR(f’,f,Ti)
8)			If p < UR(0,1) Then
9)				Reject change (keep x and f)
10)			Else
11)				Accept change (keep x’ and f’)
12)			End If
13)		Else
14)			Let x = x’
15)		End If
16)		Let Ti+1 = λTi
17)	End For

Output: The solution x
```

![](https://cdn.discordapp.com/attachments/334011383140188161/447690705390010378/unknown.png)

## Parameter Optimisation

### Optimisation Definitions
  - **“The process of making something optimal”**

  - For the purposes of this module, the “thing” that we are making optimal is a solution to a problem
  - We will often look for the highest or lowest value of a fitness function
  - The elements that we change to seek an optimal solution are often called **parameters, variables *and/or* features**
    - We change the allocation of weights to optimise how well balanced a set of scales is using Hill Climbing to solve the Scales problem

### Optimisation Problems
  - Parameter Optimisation
  - Combinatorial Optimisation
    - Subset selection
    - Permutation problems
    - Grouping (Clustering) problems
    - Bin Packing
  - Multi Objective Problems
  - Constraint Satisfaction Problems

### Parameter Optimisation:
  - This is where we are searching for the values of a set of numbers that solve a problem, typically expressed as an equation
    - I.e. The maximisation or minimisation of a function
  - More formally:
    - Find the X that maximises/minimises F(X) given:
    - X = (x1, x2, x3, ..., xn)
    - xi is a number
  - Note that the exact definition of F(X) is problem dependant
  - An example parameter optimisation problem is that of a very long range cannon
    - We have two parameters that need to be chosen so that we accurately hit a target
    - We cannot use the laws of motion since air density and drag need to be accounted for
  - We can search for the optimal set of parameters
    - Hill Climbing
    - Simulated Annealing
    - Many, many more....
    - We will cover this topic in this weeks laboratory...

### Combinatorial Optimisation:
  - **
“The process of finding an
optimal ordering or set from
a number of objects or items”
**

### Subset Selection
  - Given a set of items, select a subset of the set that optimises some requirement
  - More formally:-
    - Given X, find a Y ⊆ X such that F(Y) is a  maximum/minimum where X is a set of objects/items
  - If you can solve the **Scales** problem then you can solve the subset selection problem
  - A good example of Subset Selection is the **Feature Subset Selection** problem
  - This is where we are trying to model a set of data, but have too many features/variables/
  description
  - We wish to select the best subset that models the problem

### Permutation Problems
  - A **permutation** is defined as a shuffling of a set of objects
  - A **permutation** of A, B, C, D is B, C, A, D
  - A **permutation** of 1, 2, 3, 4 is 4, 1, 2, 3
  - If we have N objects then there are N! possible permutations
  - 4! = 24, 10! = 3,628,800, 100! = 9.333 10157
  - Without loss of generality we will assume that our solution is a permutation of the numbers
    - X = [1, 2, ..., N]
  - We will use the notation Y = π(X) to denote that Y is a permutation of X
  - We formally define the permutation problem as find a Y = π(X) such that F(Y) is a maximum/minimum
  - Note that the exact definition of F(Y) is problem dependant
  - Without loss of generality we will assume that our solution is a permutation of the numbers
    - X = [1, 2, ..., N]
  - We will use the notation Y = π(X) to denote that Y is a permutation of X
  - We formally define the permutation problem as find a Y = π(X) such that F(Y) is a maximum/minimum
  - Note that the exact definition of F(Y) is problem dependant
  - **The Travelling Salesman Problem (TSP)** is a classic example of a permutation problem
    - A sales person has to visit N cities as part of their job
    The aim is to start off at one of the cities, visit each city exactly once and then to arrive back at the starting city
    - This is called a tour
    - The objective is to find a tour where the sum of the total distance travelled is a minimum
    - I.e. This is analogous to the sales person trying to minimise their petrol costs
  - Examples include parcel delivery, general vehicle routing and road gritting

### Data Clustering
  - Data Clustering is the process of arranging objects (as points) into a number of sets (k) according to “distance” or similarity
  - Each set will be referred to as a cluster/group
  - For the purposes of this module, each set is mutually exclusive, i.e. an item cannot be in more than one Clustering
  ![](https://cdn.discordapp.com/attachments/334011383140188161/447696269415284736/unknown.png)
  - Why Cluster?
    - Knowing which objects are highly related to other objects is very useful within data analysis
    - Less complex to model
    - May give insight into the unknown properties of some of the objects
    - A useful pre-processing tool
  - The number of applications of data clustering is extensive
    - Gene Expression Data
    - Software Modularisation
    - Clustering Customer Behaviour
        - Etc...

### Bin Packing
  - The **bin packing problem** is where a number of n items of size x1,…,xn, need putting into the smallest number of bins (or boxes) of size/capacity c

![](https://cdn.discordapp.com/attachments/334011383140188161/447696775969505290/unknown.png)

  - There are a large number of bin packing applications:
    - 1-dimensional e.g. CD compilations
    - 2-dimensional e.g. stock cutting
    - 3-dimensional e.g. van packing

### Multi Objective Optimisation
  - Some optimisation problems have more than one quality or fitness function
  - Thus with these types of problems we might have more than one way of rating a solution
  - For example we might be trying to optimise X = (x1, x2, x3, ..., xn)
  - We might have a number of fitness function F1(X), F2(X), ..., Fm(X)
  - The problem is how to compare two potential solutions when only some of the fitness function evaluations are better
  - For example if we had two potential solutions X1 and X2 and three fitness functions such that:
    - F1(X1) = 10, F2(X1) = 20 and F3(X1) = 30
    - F1(X2) = 20, F2(X2) = 10 and F3(X2) = 31

### Weighted Fitness
  - One solution to this problem is to assign a numerical weight or importance to the fitness functions
  - For example:
    ![](https://cdn.discordapp.com/attachments/334011383140188161/447697339935883267/unknown.png)
  - This assumes that we can assign a weight
  -  We must have some prior knowledge of how important each function is
  -  This also requires us to be aware of what the ranges of the fitness functions are
  -  For example if one function is always less than 1 and another is always greater than 1,000,000 then equal weights would be pointless

### Pareto Optimality
  - Pareto optimality is a very straight forward but highly effective technique
  - If we have two solutions X1 and X2 then we say that X1 **Pareto Dominates** X2 if Fi(X1) is better than Fi (X2) for all i
  - We use the notation:
![](https://media.discordapp.net/attachments/334011383140188161/447697705771204609/unknown.png?width=109&height=44)

  - If neither solution dominates each other then they are **Pareto Equivalent**
  - Thus we could search for a solution to a problem which is not dominated by any other solution
  - The **Pareto Front** is the set of **Pareto Equivalent** solutions that are not **dominated** by any other solution
  - Multi Objective Optimisation has a number of applications:
    - Manufacturing
    - Telecommunications and computer networks
    - Logistics and transportation
    - Timetabling and scheduling

![](https://cdn.discordapp.com/attachments/334011383140188161/447698272858144778/unknown.png)

### Constraint Satisfaction Problems
  - Constraint Satisfaction Problems (CSP) are optimisation problems, where the valid solutions are constrained by a set of conditions
  - For example, if we are seeking to optimise:-
    - X = (x1, x2, x3, ..., xn)
  - We might have a set of constraints such as
    - ![](https://cdn.discordapp.com/attachments/334011383140188161/447698758050906112/unknown.png)

### CSP Applications
  - Advanced Planning and Scheduling
    - Train scheduling
    - Production scheduling
  - Assignment problems
    - Gate allocation for airports
    - Balancing work among different people
  - Network management and configuration
    - Planning of cabling of telecommunication networks
    - Network reconfiguration without service interruptions
  - Database systems
    - Ensure and/or restore data consistency
  - Molecular biology
    - DNA sequencing
    - Chemical hypothesis reasoning
    - Protein docking
  - Electrical engineering
    - Fault location
    - Circuit layout computation

### CSP Strategies
  - Often Heuristic Search methods are used to solve CSP
  - General Strategy
    - Instantiate all variables randomly
    - Use a repair or update strategy to move towards a more and more complete solution
    - Stop if a complete solution is found
  - Hill Climbing
    - Modify the value of one variable such that more constraints are satisfied
    - Restart with a random assignment if no more constraints can be satisfied (local minimum)
  - Minimising conflicts
    - Randomly choose a variable that is involved with an unsatisfied constraint
    - Pick a value that reduces the number of unsatisfied constraints
    - If no such value exists pick a random value which does not increase the number of unsatisfied constraints

## Tabu Search and ILS

### Popuar Heuristics
  - Hill Climbing
    - Always go up hill (accept only better quality solutions)
  - Simulated Annealing
    - The concepts of annealing and temperature
  - Iterated Local Search
  - Tabu Search
  - Genetic Algorithms
    - Simulated evolution
  - Ant Colony Optimisation
    - Pheromones and cooperation
  - Particle Swarm Optimisation
    - Swarming

### Tabu (Taboo) Search
- Tabu search tries to model human memory processes
    - Key idea: Use aspects of search history (memory) to escape from local minima
  - A **tabu-list** is maintained throughout the search
    - Associate **tabu attributes** with candidate solutions or solution components
    - Moves according to the items on the list are forbidden

![](https://cdn.discordapp.com/attachments/334011383140188161/447703680624623616/unknown.png)

### Tabu Search - Key Concepts:
  - A search (similar to Hill Climbing) that remembers sets of points in the search space
    - These are called the **Tabu** list and are to be avoided
  - The idea is that this helps in avoiding local optima
  - However if a point is evaluated to be better than any points discovered so far, then the Tabu list may be updated
    - Aspiration Criteria

### Tabu Search Stopping Conditions
  - Some immediate stopping conditions:
    - No feasible solution in the neighborhood of solution
    - The maximum amount of iterations or CPU time has been exceeded
    - The number of iterations since the last improvement is larger than a specified number
    - Evidence can be given than an optimum solution has been obtained

### Parameters of Tabu Search
  - Local search procedure
  - Neighborhood structure
  - Tabu attributes
  - Aspiration conditions
  - of tabu moves
  - Maximum size of tabu list
  - Stopping rule

### The Pros and Cons for Tabu Search
  - Pros:
    - The use of a Tabu list
    - Can be applied to both discrete and continuous solution spaces
    - A meta-heuristic that guides a local search procedure to explore the solution space beyond local optimality
    - For larger and more difficult problems (scheduling, quadratic assignment and vehicle routing), tabu search obtains solutions that rival and often surpass the best solutions previously found by other approaches
  - Cons:
    - Too many parameters to be determined
    - Number of iterations could be very large
    - Global optimum may not be found, depends on parameter settings
    - Tabu list can grow out of control

### Iterated Local Search(ILS) Key Concepts
  - ILS uses another local search algorithm as part of the algorithm
    - E.g. Hill Climbing
  - It uses information regarding previously discovered local optima (and/or starting points) to locate new (and hopefully better) local optima
  - The key algorithmic steps are as follows:

```Java
s0 = Generate initial solution

s* = LocalSearch(s0)

history = Φ
Repeat
	history = history ∪ s* [Remember previous optima and maybe start]
	scurrent = Perturb(s*,history) [Try to avoid similar starting points]
	scurrent* = LocalSearch(scurrent)
	s* = Accept(s*, scurrent*, history) [Often just accept best]
Until termination condition met
```

  - Care must be taken to assure that the perturbation step is not just mimicking the local search algorithm
  - Note: Random Restart Hill Climbing is NOT ILS

### Iterated Local Search
  - ILS can be interpreted as walks in the space of local optima
  - Perturbation is key
    - Needs to be chosen so that it cannot be undone easily by subsequent local search
    - It may consist of many perturbation steps
    - Strong perturbation: more effective escape from local optima but similar drawbacks as random restart
    - Weak perturbation: short subsequent local search phase but risk of revisiting previous optima
  - Acceptance criteria: usually either the more recent or the best
  - Often leads to very good performance
  - Only requires few lines of additional code to existing local search algorithm
  - State-of-the-art results with further optimisations

### ILS and The Scales
  - Representation
    - At the moment we are representing a solution as a Binary String or Array of Integers
    - Is this a good idea?
    - How much redundancy is there in the representation?
    - Each digit or part is either 0 or 1
    - This just needs one bit, but we are using 32 bits!!! (or 64 bits – I will we assume we are using 32…)
    - This is like writing on a pad of paper by using one sheet per letter…
    - We can save space and thus efficiency (speed) by just using the number of bits we need
    - For n weights and b bits (32) we would need the following number of integers (m)
    ![](https://cdn.discordapp.com/attachments/334011383140188161/447710265837092864/unknown.png)
    - to represent our weight/scales allocation
  - We would need 32 integers for 1000 weights...

  - We would need 32 integers for 1000 weights...
  - Luckily! Java has an in-built method for this!

```Java
import java.util.BitSet;

public class BitSetTest
{
   public static void main(String args[])
   {
      int n = 25;
      BitSet bs = new BitSet(n);
      bs.set(0,n,true);
      ShowBits(bs,n);
      bs.flip(0,n);
      ShowBits(bs,n);
      bs.set(17,true);
      ShowBits(bs,n);
   }
   private static void ShowBits(BitSet bs,int n)
   {
      for(int i=0;i<n;++i) System.out.print((bs.get(i))?"1":"0");
      System.out.println();
   }
}

`
- Fitness
  - Our fitness function for the Scales problem is an O(n) algorithm
  - However note the following:
    - If we record and remember the LHS and RHS totals and the position (index) of the last small change
    - If we changed a ‘1’ to a ‘0’ (moved from right to left)
      - NewLHS = LHS + weight(index)
      - NewRHS = RHS – weight(index)-
  - If we changed a ‘0’ to a ‘1’ (moved from left to right)
    - NewLHS = LHS – weight(index)
    - NewRHS = RHS + weight(index)
  - Thus we have created an updatable fitness function
    - New Fitness = Old Fitness + Value based on small change
  - We have reduced our time complexity from O(n) to O(1) [the notation for constant time]
  - I.e. For 1000 weights our program could be up to 1000 times faster!!!
  - Combining this with the more compact representation discussed previously we now have a much more efficient algorithm
