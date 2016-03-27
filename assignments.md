---
layout: page
title: Assignments
---

### List of assignments

{% for assign in site.assignments %}
- {% include link.html target=assign %}
{% endfor %}

### Frequently asked questions about assignments

*Written by Pat Hanrahan*

**What is the expected assignment workload?**

There are 7 assignments over the quarter, one per week.
Assignments involve writing approximately 100 lines of code,
and should be doable in 10 hours.
The assignments generally build on each other,
so it is hard to skip an assignment.
The last assignment will be a project, 
and you will have two weeks to do the project. 
The final project is more open-ended than the assignments,
and most students will spend more than 20 hours on their final project.

Starting early and making steady progress has been a generally more successful tactic than cramming the work into a last-minute all-nighter.

**What programming environment and tools are used?**

Students will use their own laptop for the assignments.
If you use a Mac laptop,
you will be using the Terminal program and unix command line tools.
If you own a Windows laptop,
you will install a virtual machine running Ubuntu linux 
and you will use the virtual machine for your assignments.

When developing on the Raspberry Pi,
you will compile programs on your laptop and download them to the Raspberry Pi.
We use a suite of open-source cross-development tools for arm processors.
These include the `binutil` packages of tools,
as well as `gcc` and `gdb`.
Other tools such as `make` and `git` will also be used for development.
You will also be expected to become proficient using 
a unix text editor such as `emacs` or `vi`,
and become proficient using the unix shell.

Assignments are distributed to students as `git` repositories.
Students edit, compile, and debug their assignments on their laptop.
When they are finished, 
they hand in the assignment by commiting their files 
into their personal git repository 
and creating a pull-request.

When the pull-request is created, code is run through a sanity check 
to ensure the code compiles. Students should ensure their code aligns with 
cs107e required [assignment directory structure](dir_structure) so it 
passes sanity check and may be evaluated by the graders.

**What is the policy on late assignments?**

Students are given a few self-granted grace days, a penalty is applied for
further late work, and there is a hard deadline after which no further late
work will be accepted. Read our detailed [late policy](/policies/#late-policy)
for the nitty-gritty mechanics.

**What is the assignment collaboration policy?**

The programming assignments are to be done individually and should represent
independent, original work. We adhere to the Stanford and CS department Honor
Code policies, and offer specific examples of its application to CS107E
coursework in our [course collaboration
policy](/policies/#collaboration-policy).

**How do I submit an assignment?**

Assignments are submitted online using `git`. 
Consult assignment 0 for information about how to use `git`.

**How are assignments graded?**

Each assignment will have a clear specification of what the program should do.
If there are multiple features, 
it will be clear how much of your grade depends on each feature.

We will also look at your code and assess the code quality.
Code quality will be graded on a bucket system where code that needs 
improvement falls in the [-] bucket, code that meets our expectations is in the 
[ok] bucket, and exceptional code falls in the [+] bucket.
In rare cases when the assignment was not sufficiently attempted, 
we will use a [- -] bucket. We will also provide comments throughout your code 
to help you improve your code quality.
Please incorporate our feedback into future assignments;
it will improve your grade and more importantly your coding style.

Assignments will have a basic part and various extensions. 
You are expected to do the basic part of each assignment.

Grades will be assigned using the following criteria:

**A.** All laboratories and basic part of assignments must be completed.
Your code quality grades should average somewhere 
between the [ok] and [+] buckets.
In addition, you must do at least 3 extensions and your final 
project must be outstanding.

**B.** All laboratories and basic part of assignments must be completed.
Your final project should be excellent.
Your code quality grades should average in the [ok] bucket.

**C and below.** All work is not completed satisfactorily.


**What about extra credit?**

This is still a new course, so we are always trying to improve it.
We will give extra credit for any work that we deem will make the next version
of the course better. This could include a creative variation of
an assignment that might be usable in the future; or written documentation,
guides, or FAQs on the hardware and software used in the course.

**What is the final project?**

See the [Final Project](project) page.

