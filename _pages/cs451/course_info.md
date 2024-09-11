---
permalink: "/cs451/course_info.html"
layout: cs451_page
title: Course Info
order: 2
---

### Catalog Description

Introduction to compiler organization and implementation, including formal specifications and algorithms for lexical and syntactic analysis, internal representation of the source program, semantic analysis, run-time environment issues and code generation. Students will write a compiler for a reasonably large subset of a contemporary language, targeted to a virtual machine.

Prerequisites: [CS310](http://www.cs.umb.edu/academics/courses/CS310) and [CS420](http://www.cs.umb.edu/academics/courses/CS420) or [CS622](http://www.cs.umb.edu/academics/courses/CS622); or permission of the instructor.

Students who successfully complete this course will be able to: write parsers and produce an abstract syntax tree (AST); analyze and generate code for a programming construct represented by an AST; and allocate physical registers (a limited resource) to a program expressed in terms of virtual registers (an unlimited resource).

### Course Staff

| **Name** | **Role** | **Email** | **Office** | **Hours** |
Swami Iyer | Instructor | [siyer@cs.umb.edu](mailto://siyer@cs.umb.edu) | M-3-201-14 | In-person: Tue Thu 9:30 AM - 10:30 AM and 2:30 PM - 3:30 PM<br/> Remote: Wed 10:00 AM - 12:00 PM ([Zoom link](https://umassboston.zoom.us/j/8790346943?pwd=N1VCR0RnbnJhNVpBZEprbmdFcVF0Zz09)) |
Trinadhreddy Seelam | Teaching Assistant | [t.seelam001@umb.edu](mailto://t.seelam001@umb.edu) | M-3-201-10 | Mon Wed 2:00 PM - 3:00 PM |

**Note**: In case you want to email us, please start the subject line with `[CS451/651]`.

### Class 

| **When** | **Where** |
| Tue Thu 4:00 PM - 5:15 PM | W-2-0158

In each class, the instructor will present the material for that class for an hour, and conduct an online quiz on that material for the remaining fifteen minutes. You are strongly encouraged to review the [material](lecture_material.html) before each class, and review it again thoroughly soon after.

### Recommended Text

<table>
<tr>
<td style="background-color: white;">
<a href="http://www.amazon.com/dp/1439860882"><i>Introduction to Compiler Construction in a Java World</i></a> by Bill Campbell, Swami Iyer, and Bahar Akbal-Delibaş

<br/><br/>

The text enables a deep understanding of the Java programming language and its implementation. It covers all of the standard compiler topics, including lexical analysis, parsing, abstract syntax trees, semantic analysis, code generation, and register allocation.
</td>
<td width="150" height="180" style="background-color: white;">
<br/><img src="/public/cs451_text.png"/>
</td>
</tr>
</table>

### Grading Scheme

#### Assessments

| **Item** | **% of Final Grade** |
| Programming Assignments (best 4 out of 1, 2, 3, 4, and 6; and 5) | 40 |
| Exams (1 and 2) | 50 |
| Quizzes [best 8 (6 if you have accommodations) out of 10] | 10 |

- The goal of the programming assignments is to make sure that you can apply the concepts learned in class to enhance the functionality of the base *j\-\-* and *iota* compilers.
- The closed-book exams will test your understanding of the theoretical concepts covered in class.
- Each weekly quiz, conducted at the end of a class, will test your understanding of the material covered in that week. Each question in a quiz is worth 2 points (1 point for correct response and 1 point for responding). Each quiz score will be normalized to 100 points.
- You can earn 0.01x% extra points if x% of the class completes the end-of-semester course evaluation. 
- If your overall score falls within half a percent of a higher grade, your score will be elevated to that grade.

#### % Score to Letter Grade

`[93, 100]: A, [90, 93): A-, [87, 90): B+, [83, 87): B, [80, 83): B-, [77, 80): C+, [73, 77): C, [70, 73): C-, [67, 70): D+, [63, 67): D, [60, 63): D-, [0, 60): F`

### Software Needed

#### iClicker

We will use [iClicker](https://www.iclicker.com/) to conduct in-class quizzes, for which you will need an [iClicker Student App Subscription](https://www.iclicker.com/pricing#student-pricing).

#### Piazza

We will use [Piazza](https://piazza.com/umb/fall2024/cs451651) as the Q&A platform for the course. If you have any general questions about the assignments, exams, or the lecture material, the most effective way to get them answered is by posting them on Piazza. You can expect your questions to be answered by the course staff or your peers.

#### Gradescope

We will use [Gradescope](https://gradescope.com/) to grade your programming assignments and exams. 

#### Programming Environment

To write and execute Java programs in this course, you will need a laptop (Linux, Mac, or Windows) properly configured with the necessary software. Click [here](programming_environment.html) for setup instructions.

#### Zoom

We will use [Zoom](https://zoom.us/) to hold remote office hours.

<a name="cs_account"></a>
### CS Account

In order to use the computing resources of the department, and in particular, those in the UNIX/PC Lab (`M-3-0731`), you need to setup a CS account. With your CS account credentials, you can connect to our designated server (`users.cs.umb.edu`) remotely using SSH. With the same credentials, you can also sign into the Linux systems in the CS Lab. In addition, you can sign into the Windows systems in the lab with the same username and an initial password `abcd_1234`, which you must change the first time you sign in. 

Visit [CS Labs Portal](https://portal.cs.umb.edu/) to register for a portal/CS account and confirm via email. If you already have a CS account, use the same username. The next step is to sign into the portal and select your courses for the term. You will be notified via your UMB email once the course directories and your account are created.

### Policies

#### Classroom

Come to class on time and stay for the entire session. If you have to leave early, let the instructor know in advance. Have your mobile phone silenced or turned off during the entire session. Use of earphone/headphone during the session is not permitted. Use of a laptop during the session is permitted only for class purposes. Do not talk to each other during the session. If you have any questions, bring them up to the instructor.

#### Piazza

If you have a question, first make sure that it has not already been asked/answered. Clearer questions get better answers, so re-read your question before you post it. Ask your questions early. Posts are categorized using tags, so pick an appropriate tag for your post. Use the platform only for questions that can be asked in a general way, without sharing code or other assignment-related work. However, if you are stuck on a problem despite your valiant efforts to solve it, you may seek help from the course staff by posting your code privately, as properly formatted text (not images). Any post that is inappropriate or violates the academic honesty code will be deleted by the course staff.

#### Makeup Exam

You must provide appropriate documentation if you were/are unable to take an exam on the scheduled date and want to arrange a makeup exam. The documentation must be a letter from the [Dean of Students](https://cm.maxient.com/reportingform.php?UMassBoston&layout_id=24) if the type of your absence is among those listed on their website. For other types of absences, the supporting documentation must be emailed to the instructor directly.

**Note**: There will be no makeup for missed quizzes.
 
#### Late Days 

Assignment deadlines are firm and non negotiable, but you have up to 5 (10 if you have accommodations) late days that you may use to submit one or more assignments a bit late. You may request an extension for any assignment only once. To do so, you must send the instructor a request via email at least 48 hours prior to the assignment deadline, clearly stating the number of late days needed, or else your request will not be granted.

Unused late days will be converted into `x%` extra points, which will be added to your final grade. `x` will be calculated as `x = d / n`, where `n` is the number of late days allotted and `d` is the number of late days unused. For example, if `d = 3` and `n = 5`, then `x = 0.6%`.

#### Regrade Request

If you have any concerns about the grading of a particular assignment or exam, you may submit a [regrade request](https://www.gradescope.com/get_started#student-submission-view) via Gradescope. You must submit the request within a week from the date the assignment or exam grades are published, or else your request will be turned down.

#### Collaboration

Click [here](collaboration.html) for the collaboration policy and the penalties for infractions of the policy.
 
#### Accommodations for Students with Disabilities

Section 504 of the Americans with Disabilities Act of 1990 offers guidelines for curriculum modifications and adaptations for students with documented disabilities. If applicable, students may obtain adaptation recommendations from the [Ross Center for Disability Services](https://www.umb.edu/academics/seas/disability-services/). The student must present these recommendations and discuss them with the instructor within a reasonable period, preferably by the end of Add/Drop period. 

#### Campus Closure

In the event of a campus closure, all class-related activities will be conducted remotely, via Zoom. If there is an exam scheduled to take place on that day, the exam will be postponed to the next suitable date.
