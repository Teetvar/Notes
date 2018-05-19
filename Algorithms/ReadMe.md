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
