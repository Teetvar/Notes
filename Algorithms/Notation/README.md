# Notes on Notation:
## Asymptotic Notation:
The running time of an algorithm depends on how long it takes a computer to run the lines of code of the algorithm—and that depends on the speed of the computer, the programming language, and the compiler that translates the program from the programming language into code that runs directly on the computer, among other factors.

Consider, the operation of an algorithm. This can be split into two sections.
 1. How long does the algorithm takes, in terms of the size of its input.
	 _function of the size of its input._
 2. How fast does a function grow, in terms of the size of its input.
	 _More commonly referred to as the "Rate of Growth"._
Here is a demonstration of these two factors written by Khan Academy:

![](https://cdn.discordapp.com/attachments/334011383140188161/447322261301493760/unknown.png)

![](https://media.discordapp.net/attachments/334011383140188161/447322423097032709/unknown.png?width=634&height=520)

The value of n at which 0.6n<sup>2</sup> becomes greater than 1000n+3000 has increased, but there will always be such a crossover point, no matter what the constants.

From the simplification of these mathematical formulas and coefficients, we can focus on the true performance of algorithms, through calculating the Rate of Growth and Runtime.
This simplification of algorithm complexity is done through the usage of **Asymptotic Notation.**

