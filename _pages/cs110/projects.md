---
permalink: "/cs110/projects.html"
layout: cs110_page
title: Projects
order: 5
---

There are 6 projects in all. These are due at midnight (11:59 PM to be precise) on the dates indicated on the [Calendar](calendar.html) page.

| **#** | **Assignment** |
1 | Straight-line Programs ([writeup](https://www.cs.umb.edu/~siyer/teaching/cs110/project1.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs110/project1.zip))|
2 | Programs with Control Flow ([writeup](https://www.cs.umb.edu/~siyer/teaching/cs110/project2.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs110/project2.zip))|
3 | Mozart Waltz Generator ([writeup](https://www.cs.umb.edu/~siyer/teaching/cs110/project3.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs110/project3.zip))|
4 | RSA Cryptosystem ([writeup](https://www.cs.umb.edu/~siyer/teaching/cs110/project4.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs110/project4.zip))|
5 | Atomic Nature of Matter ([writeup](https://www.cs.umb.edu/~siyer/teaching/cs110/project5.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs110/project5.zip))|
6 | Markov Model ([writeup](https://www.cs.umb.edu/~siyer/teaching/cs110/project6.pdf) \| [zip](https://www.cs.umb.edu/~siyer/teaching/cs110/project6.zip))|

The writeup contains simple programming exercises on concepts related to the project and the project problems along with directions on how to approach those problems. The zip file contains starter files for the exercises and problems, `report.txt` file for the project report, and any data files.

### Grading Scheme

#### Code Correctness and Style

Your solution to each programming exercise or problem will be evaluated by an autograder for correctness and style. Each test that is used to evaluate the correctness of your solution is worth some number of points; your solution will receive all the points from a test that passes and 0 points from a test that does not pass. Your solution will receive 2 points if there are no style errors, and 0 points otherwise. Your overall correctness and style score will be normalized to 60 points.

#### Code Clarity and Efficiency

Your solution to each programming problem will additionally be checked by the TAs for clarity and efficiency. Your code will receive 10 points if it meets our expectations (must include adequate comments, must follow good programming principles, and must meet any project-specific requirements such as corner cases and running times), and marked down otherwise.

#### Report

For each project, you are expected to submit a report with a brief description of how you solved each problem, mentioning any difficulties you encountered and how you overcame those difficulties. Write your report by updating the regions marked `...` in the file `report.txt`. Your report will recieve 30 points if it meets our expectations (see [report guidelines](/public/cs110/cs110_report_guidelines.pdf)), and marked down otherwise.

### Submitting Your Work

You will use [Gradescope](https://gradescope.com/) to submit your work, which will include programs (ie, `.py` files) and `report.txt`. Make sure that you only submit files listed under the "Files to Submit" section of the project writeup.

You may submit your files as many times as you like, up until the project deadline. The most recent submission is considered *active* by default and your score on the active submission is your official score for the project as well. You have the option of making any of your previous submissions active.

Note: If your active submission is partial, your project score will also be partial, so in order to be eligible for full credit, make sure you have an active submission containing all the required files for the project. 

Before you submit your programs, make sure that they meet the coding style. You may check a program, for example `helloworld.py`, for coding style by running the following command on the terminal:

```
$ pycodestyle helloworld.py
```

### Leaderboard

Each project will have a leaderboard where you can fiercely compete for the highest rank. Your rank will depend on your leaderboard score `S` in %, which will be calculated from your autograder score `X` in % and submission time score `Y` in %.

```
S = 0.5 * X + 0.5 * Y
```

For `Y`, you get 100 points if your submission is within the first tenth of the alotted duration, 90 points if it is within the second tenth, and so on.

To keep the results anonymous, when you submit your work, you will be required to submit a pseudonym for the leaderboard.

**Note:** The purpose of the leaderboard is simply to challenge you to solve the project problems correctly and quickly --- your leaderboard rank will **not** affect your grade in any manner.
