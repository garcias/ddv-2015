# 02 Solving problems

## Computing *e*

This exercise models the process of implementing a solution to a problem.


### Problem statement

- Compute *e*
- Don’t use a pre-defined function, e.g., `math.e`, `math.exp(1)`


### Research the problem

To start out a simple project like this, we need to do some research on how *e* might be computed. You can (a) ask a mathematician, (b) derive it from your knowledge of mathematics, or (c) [look it up](https://goo.gl/V81mD).

*Solution.* The simplest approach is a Taylor series:

- e<sup>x</sup> = &sum; x<sup>n</sup> / n!


### Diagram the implementation

A common technique in software development is to **diagram** the implementation of a solution. At the simplest level, such a diagram just starts with the end goal, and breaks it down into components, so that you can focus your attention on each component in turn. 

*Solution.* To calculate e<sup>x</sup>, we need to be able to do three things:

- calculate the factorial of n = 0, 1, 2, ...
- raise the parameter x to an integer power n
- add successive terms of the series


### Identify a test case

Developers specify **unit tests** at an early stage of design to specify the desired performance of code. We won’t do formal unit testing, but we’ll adopt the concept of a **test case** from it. A test case specifies what a component should be able to do, even if other components aren’t working yet. 

*Solution.* The test case for each task:

- **factorial:** factorial(0) = 1, factorial(1) = 1, factorial(3) = 6
- 


## Keeping track of the approximation as *n* increases


### Problem statement

- Compute *e* for different values of *n*
- Store estimates of *e* as a function of *n* in a list structure


### Introducing lists

A list is a **data structure**: it stores other types of information (integers, floats, strings, *etc*) according to an **index** numbered from 0 to *n*. A list has specific functions, called **methods**, for adding, removing, and finding items within it.

- Find out how to add an item to the *end* of a list
 

### Diagram the implementation

An advantage of diagramming now becomes clear: We can reuse the previous implementation, and simply attach a new task to it.

- Draw a diagram representing your current implementation.
- Draw a new task and show where it connects to the existing tasks.


### Identify test cases

Since you are new to lists, make sure you understand how to append an item to it, and then find that item later.

- Create an empty list named `estimate`
- Create a test case: add the number 3.14 to the list, then add the number 0 to the list
- Create a test case: print the *first* item of the list, and verify that it is 3.14.



## Refactoring your code 

Currently the computation of *e* is mixed in with maintenance of the `estimate` and `error` lists. This is fine if the purpose of the lists is to study just the code. But what if your code is working well, and you anticipate no further changes to it? Then it’s time to **refactor**. 

When you refactor code, *the overall functionality stays the same*, but you reorganize different tasks. In this case, we’re going to separate the task of estimating *e* from the task of storing its value. Structurally, this means **encapsulating** the computation as a **function** of *n*.


### Analyze code

Select your working code cell and press `C` to copy it, then paste it below. Identify which sections of code should be separated from each other. 

- Move the code for building the lists into a different code cell.
- Place the remaining code (for computing *e*) into a **function block**. Define an interface for this function and call it `compute_e(n)`. Then specify its return value.
- Test that the function returns values you expect
- Create a loop that builds the lists `estimate` and `error` by using the function `compute_e()`.


## Assignment

Now that you are familiar with lists, get more practice with them. Complete the [Codecademy tutorials](https://www.codecademy.com/en/tracks/python) on [Python Lists and Dictionaries](https://www.codecademy.com/courses/python-beginner-en-pwmb1/0/1). If you want even more practice, try [A Day at the Supermarket](https://www.codecademy.com/courses/python-beginner-en-IZ9Ra/0/1), but be aware that the later parts of it require you to have mastered [Functions](https://www.codecademy.com/courses/python-beginner-c7VZg/0/1), which is one of the longer tutorials. 