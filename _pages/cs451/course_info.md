---
permalink: "/cs451/course_info.html"
layout: cs451_page
title: Course Info
order: 2
---

### Course Description

Introduction to compiler organization and implementation, including formal specifications and algorithms for lexical and syntactic analysis, internal representation of the source program, semantic analysis, run-time environment issues and code generation. Students will write a compiler for a reasonably large subset of a contemporary language, targeted to a virtual machine.

Prerequisites: [CS310](http://www.cs.umb.edu/academics/courses/CS310) and [CS420](http://www.cs.umb.edu/academics/courses/CS420) or [CS622](http://www.cs.umb.edu/academics/courses/CS622); or permission of the instructor.

Students who successfully complete this course will be able to: write parsers and produce an abstract syntax tree (AST); analyze and generate code for a programming construct represented by an AST; and allocate physical registers (a limited resource) to a program expressed in terms of virtual registers (an unlimited resource).

### Course Staff

| **Name** | **Role** | **Email** | **Office** | **Hours** |
Swami Iyer | Instructor | [siyer@cs.umb.edu](mailto:siyer@cs.umb.edu) | M-3-201-14 | In-person: Tue Thu 10:00 AM - 12:00 PM<br/> Remote: Wed 10:00 AM - 12:00 PM ([Zoom link](https://umassboston.zoom.us/j/8790346943?pwd=N1VCR0RnbnJhNVpBZEprbmdFcVF0Zz09)) |
Ramsey Harrison | Teaching Assistant | [ramsey.harrison001@umb.edu](mailto:ramsey.harrison001@umb.edu) | M-3-201-10 | Tue Thu 1:00 PM - 2:00 PM |

Note: In case you want to email us, please start the subject line with `[CS451/651]`.

### Lectures

We will have two lectures per week, during which I will present the material from the [slides](lecture_material.html). I strongly recommend skimming through the material before each lecture, and reading it again thoroughly soon after.

| **Section** | **When** | **Where** |
1 | Tue Thu 4:00 PM - 5:15 PM | Y-2-2110

### Text

<img src="/public/cs451_text.png" width="150" height="180"/>

[Introduction to Compiler Construction in a Java World](http://www.amazon.com/Introduction-Compiler-Construction-Java-World/dp/1439860882) by Bill Campbell, Swami Iyer, and Bahar Akbal-Delibaş

The text enables a deep understanding of the Java programming language and its implementation. It covers all of the standard compiler topics, including lexical analysis, parsing, abstract syntax trees, semantic analysis, code generation, and register allocation. It also demonstrates how JVM code can be translated to a register machine, specifically the MIPS architecture. In addition, the text covers recent strategies, such as just-in-time compiling and hotspot compiling.

### Grading

#### Assessments

| **Item** | **% of Final Grade** |
| Projects (1, 2, 3, 5, and best of 4 and 6) | 35 |
| Exams (1 and 2) | 60 |
| Attendance | 5 |

#### Scale

| **% Score** | **Grade** |
| [93, 100\] | A |
| [90, 93)  | A-  |
| [87, 90)  | B+ |
| [83, 87)  | B   |
| [80, 83)  | B-  |
| [77, 80)  | C+ |
| [73, 77)  | C   |
| [70, 73)  | C-  |
| [67, 70)  | D+ |
| [63, 67)  | D   |
| [60, 63)  | D-  |
| [0, 60)   | F   |

#### Note

- The goal of the projects is to make sure that you can apply the concepts learned in class to enhance the functionality of the base *j\-\-* compiler, ie, add new programming constructs to the language.
- The exams will test your understanding of the material covered in class as well as concepts from the projects.
- Each of the two closed-book exams will take place during a class period. You will be allowed to use a one-page (two sides) notes sheet.
- If you score at least 80% on both exams, the higher exam score will be considered as the exam average.
- Attendance score will be based on your attendance in class.
- You can earn up to 0.01x% extra points if x% of the class completes the end-of-semester course evaluation. 
- If your overall score falls within half a percent of a higher grade, your score will be elevated to that grade.

Click [here](grade.html) calculate your current course grade.

### iClicker

Starting from the second week, I will use [iClicker](https://app.reef-education.com/\#/login iClicker) to record your attendance in class. You will be able to mark yourself present, using your laptop or smart device, during the first 15 minutes of a class. In addition, I will take paper-based attendance on some undisclosed days. If I find any discrepancy in your attendance record on those days (ie, you were marked present on iClicker but absent on paper), you will receive a 0 for your overall attendance score.

### Piazza

I will use [Piazza](https://piazza.com/umb/spring2024/cs451651/home) as the online discussion forum for the course. If you have any general questions about the projects, lectures, textbook, or other course material, the most effective way to get them resolved is by posting them on Piazza. You can expect your questions to be answered by the course staff or one of your classmates. Remember that you can post anonymously, but you are anonymous only to your classmates and not to the course staff.

### Gradescope

I will use [Gradescope](https://gradescope.com/) to grade your projects and exams. 

### Programming Environment

To write and execute Java programs in this course, you will need a laptop (Linux, Mac, or Windows) properly configured with the necessary software. Click [here](programming_environment.html) for setup instructions.

<a name="cs_account"></a>
### CS Account

In order to use the computing resources of the department, and in particular, those in the UNIX/PC Lab (`M-3-0731`), you need to setup a CS account. With your CS account credentials, you can connect to our designated server (`users.cs.umb.edu`) remotely using SSH. With the same credentials, you can also sign into the Linux systems in the CS Lab. In addition, you can sign into the Windows systems in the lab with the same username and an initial password `abcd_1234`, which you must change the first time you sign in. 

Visit [CS Labs Portal](https://portal.cs.umb.edu/) to register for a portal/CS account and confirm via email. If you already have a CS account, use the same username. The next step is to sign into the portal and select your courses for the term. You will be notified via your UMB email once the course directories and your account are created.

### Policies

#### Classroom

- Come to each class on time and stay for the entire session. If you have to leave early, let the instructor know in advance.
- Have your mobile phone silenced or turned off during the entire session.
- Do not talk to each other during the session. If you have any questions, bring them up to the instructor.

#### Piazza

- If you have a question, first make sure that it has not already been asked/answered.
- Clearer questions get better answers, so re-read your question before you post it.
- Ask your questions early.
- Posts are organized in folders, so specify the right folder(s) for your post.
- Use the forum only for questions that can be asked in a general way, without sharing code or other project-related work. However, if you are stuck on a problem despite your valiant efforts to solve it, you may seek help from the course staff by posting your code privately, as properly formatted text (not images).
- Any post that is inappropriate or violates the academic honesty code will be deleted by the course staff.

#### Excused Absence and Makeup Exam 

You must provide appropriate documentation if: 

- You could/will not attend a lecture and want your absence to be excused. 
- You were/are unable to take an exam on the scheduled date and want to arrange a makeup exam. 

The documentation must be a letter from the [Dean of Students](https://cm.maxient.com/reportingform.php?UMassBoston&layout_id=24) if the type of your absence is among those listed on their website. For other types of absences, the supporting documentation must be shared with me directly.
 
#### Collaboration

Click [here](collaboration.html) for the collaboration policy and the penalties for infractions of the policy.
 
#### Late Days 

- Project deadlines are firm and non negotiable, but you have up to 5 (8 if you have accommodations through the Ross Center) late days that you may use to submit one or more projects a bit late. 
- You may request an extension for any project only once. To do so, you must send me a request via email (not Piazza) at least 48 hours prior to the project deadline, clearly stating the number of late days needed, or else your request will not be granted.

#### Regrade Request

- If you have any concerns about the grading of a particular project or exam, you may submit a [regrade request](https://www.gradescope.com/get_started#student-submission-view) via Gradescope. 
- You must submit your regrade request within a week from the date the project or exam grades are published, or else your request will be turned down.

#### Accommodations for Students with Disabilities

Section 504 of the Americans with Disabilities Act of 1990 offers guidelines for curriculum modifications and adaptations for students with documented disabilities. If applicable, students may obtain adaptation recommendations from the [Ross Center for Disability Services](https://www.umb.edu/academics/seas/disability-services/). The student must present these recommendations and discuss them with the instructor within a reasonable period, preferably by the end of Add/Drop period. 
