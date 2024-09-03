---
permalink: "/cs451/assignments.html"
layout: cs451_page
title: Assignments
order: 5
---

There are 6 programming assignments in all. These are due at midnight (11:59 PM to be precise) on the dates indicated on the [Calendar](calendar.html) page.

| **#** | **Title** | **Goal** | **Links** |
1 | Supporting Simple Operations | Become familiar with the Java Virtual Machine (JVM) and the Marvin Machine; and extend the *j\-\-* language by adding support for some arithmetic operators, conditional expression, and do statement. | [writeup](https://www.cs.umb.edu/~siyer/teaching/cs451/simpleops.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs451/simpleops.zip) \| [discussion](https://www.cs.umb.edu/~siyer/teaching/cs451/simpleops_discussion.pdf) |
2 | Scanning | Modify the handcrafted scanner to support multiline comments; additional tokens (reserved words and operators); and `long` and `double` literals in *j\-\-*. | [writeup](https://www.cs.umb.edu/~siyer/teaching/cs451/scanning.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs451/scanning.zip) \| [discussion](TBD) |
3 | Parsing | Modify the handcrafted parser to support `long` and `double` basic types; additional operators; for, break, continue, and switch statements; exception handlers; and interface type declaration in *j\-\-*. | [writeup](https://www.cs.umb.edu/~siyer/teaching/cs451/parsing.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs451/parsing.zip) \| [discussion](TBD) |
4 | Scanning and Parsing with JavaCC | Modify the`j--.jj` file used for generating a scanner and parser (using JavaCC) for *j\-\-* to support multiline comments; `long` and `double` basic types; additional tokens (reserved words and operators); conditional expression; do, for, break, continue, and switch statements; exception handlers; and interface type declaration. | [writeup](https://www.cs.umb.edu/~siyer/teaching/cs451/javacc_frontend.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs451/javacc_frontend.zip) \| [discussion](TBD) |
5 | Type Checking and Code Generation | Implement type checking and JVM code generation for the programming constructs that were added to *j\-\-* in Assignment 3 (Parsing). | [writeup](https://www.cs.umb.edu/~siyer/teaching/cs451/codegen.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs451/codegen.zip) \| [discussion](TBD) |
6 | Register Allocation | Implement the graph coloring based register allocation algorithm in *iota*. | [writeup](https://www.cs.umb.edu/~siyer/teaching/cs451/register_allocation.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs451/register_allocation.zip) \| [discussion](TBD) |

The writeup file contains descriptions of the problems in the assignment. The zip file contains test programs, reference output files, and `notes.txt` file for the assignment. The discussion link provides additional explanation of the assignment problems and directions on how to solve them.

### Submitting Your Work

You will use [Gradescope](https://gradescope.com/) to submit your Java programs (ie, `.java` files) and the `notes.txt` file. Make sure that you only submit files listed under the "Files to Submit" section of the assignment writeup.

You may submit your files as many times as you like, up until the assignment deadline. The most recent submission is considered *active* by default and your score on the active submission is your official score for the assignment as well. You have the option of making any of your previous submissions active.

**Note**: If your active submission is partial, your assignment score will also be partial, so in order to be eligible for full credit, make sure you have an active submission containing all the required files for the assignment.

### How the Assignments will be Scored

#### Correctness

Your solution to each assignment problem will be evaluated for correctness by an autograder. Each test that is used for this purpose is worth some number of points; your solution will receive all the points from a test that passes and 0 points from a test that does not pass. Your overall correctness score will be normalized to 80 points.

#### Clarity and Efficiency

Your solution to each assignment problem will additionally be checked by a TA for clarity and efficiency. Your code will receive 10 points if it meets our expectations (must include adequate comments, must follow good programming principles, and must meet any problem-specific requirements), and will be marked down otherwise.

#### Notes File

The given `notes.txt` file for an assignment must be uploaded with the three sections (\#1 mandatory, \#2 if applicable, and \#3 optional) filled in as appropriate. Your notes file will receive 10 points if it meets our expectations (section \#1 must provide a clear high-level description of each problem in no more than 100 words), and will be marked down otherwise.
