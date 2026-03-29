---
title: Syllabus
permalink: "/syllabus"
layout: default
nav_order: 1
---

# Syllabus, {{site.title}}

CMPSC 5B, Introduction to Data Science 2, Spring 2026

## What is this course about?

The Introduction to Data Science course series (CMPSC 5A/5B) teaches skills for analyzing real-world data using computational and statistical tools. 

We use the textbook [Computational and Inferential Thinking: The Foundations of Data Science, 2nd Edition](https://inferentialthinking.com/)
by Ani Adhikari, John DeNero, David Wagner.  This text was originally developed for the UC Berkeley course Data 8: Foundations of Data Science, and is [freely available online](https://inferentialthinking.com/).

* CMPSC 5A covers chapters 1-9
* CMPSC 5B reviews chapters 1-9, and then covers chapters 10-18

## Topics

We plan to cover the following topics in CMPSC 5B this quarter:

* [Ch10: Sampling and Empirical Distributions](https://inferentialthinking.com/chapters/10/sampling-and-empirical-distributions/)
* [Ch11: Testing Hypotheses](https://inferentialthinking.com/chapters/11/testing-hypotheses/)
* [Ch12: Comparing Two Samples](https://inferentialthinking.com/chapters/12/comparing-two-samples/)
* [Ch13: Estimation](https://inferentialthinking.com/chapters/13/estimation/)
* [Ch14: Applications of Mean/Variance/Std Deviation and the Central Limit Theorem](https://inferentialthinking.com/chapters/14/why-the-mean-matters/)
* [Ch15: Prediction/Correlation/Regresssion](https://inferentialthinking.com/chapters/15/prediction/)
* [Ch16: Inference for Regression](https://inferentialthinking.com/chapters/16/inference-for-regression/)
* [Ch17: Classification](https://inferentialthinking.com/chapters/17/classification/)
* [Ch18: Updating Predictions](https://inferentialthinking.com/chapters/18/updating-predictions/)

We will also review and reinforce the following skills from CMPSC 5A:
* Working with Jupyter notebooks in both JupyterHub and Google Colab
* Python programming skills
* Basic skills for working with datasets, `numpy`, `datascience` tables and `datascience` visualization.

We may also cover some basic git/github skills.

## Background Needed for CMPSC 5B

The background needed for CMPSC 5B is contained in Chapters 1 through 9 of [the CMPSC 5A/5B textbook](https://inferentialthinking.com/).

Here is a partial list of important topics from these chapters that students should be comfortable with (or quickly learn during the first week or two of CMPSC 5B).  For a full list, consult the textbook chapters directly.

(1) Basic Python programming skills from CMPSC 5A (or other coursework) including:
* Basic Python data types: int, float, string, bool, list
* Assignment statements, and operators
* defining Python functions with parameters, and calling those functions (the textbook uses the phrase "call expressions")
* if/elif/else statements
* for loops and while loops

(2) The following skills taught in CMPSC 5A that pertain to the `datascience` module from UC Berkeley, and related `numpy` and `matplotlib` concepts:

* The `table` abstraction: how to create tables using code, and by reading from data files
* How to pull out particular rows, columns, and values from `table` objects
* The `numpy` array data type (`ndarray`), and commmon `numpy` methods used in conjunction with the `datascience` module, and separately.
* How to sort `table` objects
* How to summarize, join, and pivot table objects
* How to perform basic visualizations on table objects, such as bar graph, histograms, and line graphs.

(3) A few basic concepts in statistics, including mean, variance, and standard deviation.

## Basic Facts

* **Instructor**:  [Phill Conrad](https://pconrad.github.io) (contact via Slack)
  * Use the "help" channel to ask for help or ask a question.
  * Use direct messages (DMs) to Prof. Conrad, TAs or ULAs *only* in cases where there is something
    confidential that you need to ask about; please do not use DMs for asking general questions.
* **Lecture**:
  * Mon/Wed 9:30-10:45 @ Buchanan 1930
  * You are expected to participate synchronously.  The mode of instruction is "in-person".  Having said that: accomodations will be made if students need to stay away due to illness: please *do not come to class* if you are sick.  Instead, contact the course staff for remote participation options.
* **TAs**: {{site.ta_list_full}} (contact via Slack)
* **LAs**: {{site.la_list_full}} (contact via Slack)
* **Lab** (50 minute discussion section)
  * {{site.discussion_section_day}} {{site.discussion_section_times}}
  * Attendance/Participation is expected/required.
  * Please participate in the section for which you are registered; if you need to change sections, contact the instructor via Slack DM.
* Office Hours: See: [https://ucsb-ds.github.io/5b-s26/office-hours.html](https://ucsb-ds.github.io/5b-s26/office-hours.html)


Course website: <https://ucsb-ds.github.io/5b-s26/>


## Missing homework/in-class activities: Drop the lowest n grades

If you miss a participation assignment, you miss the opportunity for the points on that participation assignment, or homework that was due.

Rather than providing a makeup opportunity, I will drop:

* the lowest n participation assignments
* the lowest k homework/quiz grades

Where both n and k are a function of the number of assignments in that category:

* <= 2 assignments, no dropped assignments
* 2 to 5 assignments: 1 dropped grades
* 6 to 8 assignments: 2 dropped grades
* 9 to 15 assignments: 3 dropped grades
* 16 or more: the "ceiling" of the number of assignments divided by 5 (i.e. next higher whole number if the number is not evenly divible by 5.)

This applies only to participation and homework assignments.

This should be sufficient to allow for occaisional personal situations that may prevent your participation; if there is some special circumstance beyond your control where greater consideration may be needed, please contact the instructor; they will consider these on a case-by-case basis.

Each homework and in-class-activity will be of equal value (100 pts).

## Use of a laptop is required

We'll be doing a lot of hands on work in both lecture and section.  Please bring a laptop to class.

Please make sure your laptop is charged before class, since power outlets may be unavailable.


## Support from the Teaching Staff


You are not alone in this course; the Teaching Assistants (TAs), Undergraduate Learning Assistants (ULA) and Instructor are here to support you as you learn the material. It's expected that some aspects of the course will take time to master, and the best way to master challenging material is to ask questions. For questions, use Slack. We will also hold Tutoring Hours for real-time discussions.

Your discussion TA will be your main point of contact for all course related questions/grade clarifications. The TAs are here to support you so please lean on your discussion TA if you need more support in the class or have any questions/concerns.

Tutoring Hours with ULAs will be available for students in need of additional support to develop confidence with core concepts. In past quarters, students who attended have found these sessions to be a great use of their time.

## Grading criteria 

Grades will be assigned using the following weighted components.  

The codes in the table correspond to the codes for the activities in the Canvas gradebook; for example, the In Class activities are numbered ic00, ic01, ic02, etc. while labs are numbered lab00, lab01, lab02, etc.

| Assignment Category | Prefix Code | Percentage of Final Grade |
|---------------------|-------------|---------------------------|
| In class and Homework | `ic` and `h` | 20% |
| Labs and Quizzes | `lab`, `quiz` | 20% |
| Project | `proj` | 30% |
| Exams | `lab` | 30% |


We will make every effort to post grades within about 1 week after the assignment's due date.

## PrairieLearn Assignments

We will be piloting the use of a platform that's new at UCSB, but which has been used at other Universities extensively for over 10 years called PrairieLearn.

PrairieLearn is an online platform for practice problems, homework, quizzes and exams.   

For many questions, it generates new question instances each time you try a problem.  

For example, suppose the problem is about how to interpret the * and + signs in Python, and how to use the "PEMDAS" rule to ensure that you do multiplication before addition.

* One student will get: 3 + 4 * 7
* But another student may get: 2 * 5 + 3

In some cases, you will be allowed multiple tries at the problem until you get it right.

Some PrairieLearn assignments will be for a grade, while others will be for practice.

The good part is that often your quizzes and exams will be based on the same "question generating code" that you got to practice with.

That means that if you are willing to put in the work, you can keep trying the problems until you are confident that you know how to do them, and you can go into the exams very well prepared to demonstrate your skills and knowledge.


## Quizzes and Exams

All exams and exams in this class will be taken on a computer in the UCSB Testing Center. You will schedule your own exam times for each exam window (during Testing Center hours) so that you can take the exams when they work best for you. 

Please read the following information about exams very closely.
* Exam windows are clearly indicated in the table below.
* You may begin scheduling your exam times two days before the exam window opens.
* You may change your exam time up to 2 hours before the exam.
* If you are more than 5 minutes late to your scheduled time, your appointment will be cancelled and you will need to reschedule. Note that additional exam time slots cannot be added to any exam window. (For this reason, you are encouraged to schedule early in the window if possible, rather than during the last available slot.)

You will schedule your exam via a link provided in Canvas. Exam slots are scheduled as available. If you have DSP time accommodations for an exam, they are already entered in the exam scheduler and attached to your exam.

### On the day of your exam:

Go to the Testing Center. Arrive at least 15 minutes before your scheduled exam time.
Bring with you:

* Photo ID
* Cellphone to log into computers (for Duo Multi-Factor Authentication)
* Your UCSB netID (“username) and UCSB password. 

If you do not have your username and password, you will be unable to take the exam.

You will take your exam in PrairieLearn on a Testing Center computer. The exam is proctored and monitored, and questions are randomized so that no students receive similar exams. 

I recommend that you visit the Testing Center prior to your scheduled exam time so that you’re familiar with where it is, how long it takes to get there, etc.

## Quiz and Exam Schedule

We will go over how to reserve appointments in class on Wednesday 04/01.

| name | duration  | percentage of final grade | week | first day | last day | registration opens |
|-|-|-|-|-|-|-|
| `quiz01` | 75 min | approx 2% | week 3 | Wed 04/15 | Fri 04/17 | registration opens | Wed 04/01 |
| `exam01` (midterm) | 75 min| 15% | week 7 |  Wed 05/13 | Fri 05/15 | Wed 04/29 | 
| `exam02` (final) | 150 min | 15% | finals week (week 11) | Mon 06/08 | Thu 06/11 | Fri 05/22 | 

## Labs

This course has a 50-minute weekly discussion section. During discussion sections, the TA will help you get started with your lab assignments. The weekly discussion section consists of a lab assignment that develops skills with computational and inferential concepts. You will also get a chance to interact with LLMs and use them for your labs! You are required to submit all your prompts and LLM responses. These lab assignments will be released at the start of the Discussion section and due the following week at 11:59pm the day before your discussion section.  Labs will be accepted up to two days after the deadline with a 10% deduction per day late.
Projects

Data science is about analyzing real-world data sets, and so you will also complete two projects involving real data. On each project, you may work with one or more partners (we will update you with instructions once your projects are released). You will also get a chance to interact with LLMs and use them for your projects! You are required to submit all your prompts and LLM responses. All the partners will receive the same score. 

## Late Submissions

The quarter moves quickly and all of the work in the course is cumulative. If work is late, you’ll fall behind and won’t receive the full benefit of the course. 


## Learning Cooperatively 

We encourage you to discuss course content with your friends and classmates as you are working on your assignments. No matter your academic background, you will learn more if you work alongside others than if you work alone. Ask questions, answer questions, and share ideas liberally.

If some emergency takes you away from the course for an extended period, or if you decide to drop the course for any reason, please don't just disappear silently! You should inform your discussion TA and your project partner (if you have one) immediately, so that nobody is expecting you to do something you can't finish.

## Academic Honesty

Cheating and Plagiarism often happens when students feel overwhelmed with completing assignments, meeting deadlines, and truly understanding the course material. When you need help, reach out to the course staff using Ed, in Tutoring hours, and/or during live Discussion sections and lectures. You are not alone in this class! The Teaching Staff is here to help you succeed. We expect that you will work with integrity and with respect for other members of the class, just as the course staff will work with integrity and with respect for you. 

Finally, know that it's normal to struggle. UC Santa Barbara has high standards, which is one of the reasons its degrees are valued. Everyone struggles even though many try not to show it. Even if you don't learn everything that's being covered, you'll be able to build on what you do learn, whereas if you cheat you'll have nothing to build on. You aren't expected to be perfect; it's ok not to get an A.

* Allowed: Discussion of lecture and reading materials		
* Allowed: Discussion of how to approach assignments, what techniques to consider, what textbook or lecture material is relevant
* Allowed: Using LLMs to understand code, concepts, perform helpful tasks related to  data analyses
* Not allowed: Sharing ideas in the form of code, pseudocode, or solutions if collaboration is not permitted.
* Not allowed: Turning in someone else's work as your own, even with that person's permission.
* Not allowed: Allowing someone else to turn in your work as his or her own.
* Not allowed: Turning in work without proper acknowledgment of the sources of the content (including ideas) contained within the work.	
* Not allowed: Blindly copying LLM responses 

If there is any suspicious activity, credit may be removed and a report will be made to the Office of Student Conduct. If there is more than one instance of academic integrity violations, the student will fail the course and another report will be made to the Office of Student Conduct.

Honesty and integrity in all academic work is essential for a valuable educational experience.  The Office of Judicial Affairs has policies, tips, and resources for proper citation use, recognizing actions considered to be cheating or other forms of academic theft, and students’ responsibilities, available on their website at: http://judicialaffairs.sa.ucsb.edu.  Students are responsible for educating themselves on the policies and to abide by them.


## Tentative Deadlines

Please refer to Canvas for our Tentative schedule of topics and deadlines.

## Schedule changes

As we review your coding assignments and projects and talk with you during Tutoring hours, we may find that we'd like to modify the pace of the course or change what we have included as the course progresses. If this does happen, we will let you know via lecture and Slack. Please check Slack, your UCSB email, and our Canvas page, regularly for updates to the assignments or any additional course updates. 

## Intellectual property - course materials

All course materials (class lectures and discussions, handouts, examinations, web materials) and the intellectual content of the course itself are protected by United States Federal Copyright Law and the California Civil Code. UC Policy 102.23 expressly prohibits students (and all other persons) from recording lectures or discussions and from distributing or selling course materials without the prior written permission of the instructor. (See http://policy.ucop.edu/doc/2710530/PACAOS-100). Students are permitted to make notes solely for their own private educational use. Exceptions to accommodate students with disabilities may be granted with appropriate documentation.

## Respectful Learning Environment

It is part of UCSB's mission to "foster an environment that promotes safety, inclusivity, and is free from discrimination". ([source](https://studentlife.sa.ucsb.edu/equity-inclusion/bias)). 

All students, faculty and staff are expected to follow both the letter and spirit of all of UCSB's policies that promote such an environment at all times, including in the context of this course. Please avoid any words or actions that would be inconsistent with this.

*UCSB non-discrimination policy*: UC Santa Barbara prohibits discrimination and harassment of any person on the basis of their protected class status, which is an identity protected by federal or state law, including the following: race, religion, color, citizenship, national or ethnic origin, ancestry, sex (including pregnancy, childbirth, lactation or related medical conditions), gender, gender identity, gender expression, gender transition, sexual orientation, physical or mental disability (including having a history of a disability or being regarded as being disabled), medical condition (cancer-related or genetic characteristics), predisposing genetic information (including family medical history), marital status, age (at least 40 years of age), or veteran or military status. ([source](https://titleix-dhp.ucsb.edu/discrimination-harassment-overview)).

UCSB does not tolerate sexual harassment/sexual violence, which is prohibited by University policy and state and federal law. The Title IX Compliance and Sexual Harassment Policy Compliance Office (TIX/SHPC) provides assistance in preventing and resolving and investigating complaints of sexual harassment/sexual violence and gender discrimination.

Please help me to cultivate a positive classroom environment by communicating any concerns that you have.	

## Mandatory Reporting 

As an instructor, one of my responsibilities is to help create a safe learning environment on our campus.  I want to ensure that students feel they can speak to me, but I also want students to be informed that I have a mandatory reporting responsibility related to my role as a professor. I am *required* to share information regarding sexual misconduct, information about a crime that may have occurred on UCSB’s campus or in the community, or incidents of bias directed against individuals or groups that violate university policy.   A result of my mandated report will be that students will receive outreach and resources from the campus Title IX office. Students may speak to someone confidentially by contacting CARE, Campus Advocacy, Resources & Education at the 24/7 advocacy line at (805) 893-4613 or visit them in person at the Student Resource Building.

## Accommodations for disabilities

Students with disabilities may request academic accommodations for exams online through the UCSB Disabled Students Program at <http://dsp.sa.ucsb.edu/>. Please make your requests for exam accommodations through the online system as early in the quarter as possible to ensure proper arrangement.

## Managing stress

Personal concerns such as stress, anxiety, relationships, depression, cultural differences, can interfere with the ability of students to succeed and thrive. For helpful resources, please contact UCSB Counseling & Psychological Services (CAPS) at 805-893-4411 or visit <https://caps.sa.ucsb.edu/> 

## Food Security and Calfresh

If you are facing any challenges securing food or housing, and believe this may affect your performance in the class, you are urged to reach out the resources available at <https://basicneeds.ucsb.edu>). 

## Standard Disclaimer

This syllabus is as accurate as possible, but is subject to change at
the instructor's discretion, within the bounds of UC policy.

(end of syllabus)
