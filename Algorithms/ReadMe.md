# Algorithms and their Application Notes:
Everything you need to know.
_How did Mann take the time to do this... It's like he programmed a bot to do it for him..._

## The Foundations of Algorithm Analysis:
### Runtime:
The running time of an algorithm varies with the input and typically grows with the input size. An algorithm may run faster on certain data sets than on others hence it would have the following run times:
 - Best case 
	 - The best case is not very informative
 - Average case 
	 -	The average case can be difficult to determine
 - Worst case
	 - Easier to analyse
	 - Crucial to applications such as air traffic control, surgery, finance,…
		 - E.g. Real time applications
		 - 
### Asymptotic Analysis:
#### What does Asymptotic Analysis mean?
 - For our purpose, it means the long term behavior of something, in this case, an Algorithm.
The technique uses a high-level description of the algorithm instead of an implementation
Takes into account all possible inputs
Allows us to evaluate the speed of an algorithm independently of the hardware/software environment
#### Estimating "Running Time":
 - Write down an algorithm.
	 - Using Pseudo-Code
 - In terms of a set of primitive operations:
	 - Count the number of steps In terms of primitive operations, considering worst case input.
	 -  Bound or “estimate” the running time.
		 - Ignore constant factors 
		 - Bound fundamental running time
This leads onto the Big-Oh (Big-O) notation for computational complexity.

### T(_n_) & O(_n_) :
 - We estimate the running time/computation of an algorithm. 
 - We refer to this resultant formula as T(_n_) where _n_ is the size of the input.
 - If there is more than one input we might have T(_n,m_) (etc…) where *n* and *m* are the sizes of the input. 
 - We can use *T(n)* to compute a very important property called the big-O ***O(n)***.

### Pseudo-Code:

 - Pseudo-Code is a cross between a programming language and written text.
 - It is used to represent algorithms in a programming language independent manner.
 - We often specify the input and output and number the lines.

#### The additional notes from this point forward will be based on The Universal Pseudo-Code format, created by Dr. Stephen Swift:
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
	`If … Then … [Else …] End If`
	`While … End While`
	`Repeat … Until …`
	`For …End For …`
 - Indentation replaces braces [as in Python]
 - Method/algorithm declaration:
	`Algorithm number name (arguments/parameters)`
	`Input …`
`...`
`Output …`
-	Method/algorithm calls
	-	Call name `(arguments/parameters)`

#### Pseudo-Code Details Continued:
-	Expressions
	-	We use a single = sign for both assignment and equality testing
	-	`Let x = 0`
	-	`If x = y Then...`
	-	The context differentiates the meaning of the usage…
-	n<sup>2</sup> superscripts, subscripts n<sub>i</sub> and other mathematical formatting is allowed
-	We often write the algorithm in a different font such as Courier New for Mono-spacing and Clarity.

#### Variables:
![](https://cdn.discordapp.com/attachments/334011383140188161/447334384836542475/unknown.png)
#### If Statements:
![](https://cdn.discordapp.com/attachments/334011383140188161/447334543851126814/unknown.png)
#### For Loops:
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
