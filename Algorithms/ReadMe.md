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
