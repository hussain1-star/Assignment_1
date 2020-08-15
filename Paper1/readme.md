# An Empirical Study of Quick Remedy Commits.

# Authors
1: Fengcai Wen

2: Csaba Nagy

3: Michele Lanza

4: Gabriele Bavota

# Conference Name:  

International Conference on Program Comprehension (13-15 July 2020).

Published Date: Tue 14 Jul 2020 02:00 - 02:15 at ICPC - Session 4

Summary:
In this research paper authors declares that In the software life-cycle, change is the rule rather than the exception. Changes are generally performed through commit activities
aimed at adding new functionalities, repairing faults, and refactoring code [49]. Some of these commits can involve a substantial part
of the source code, with dozens of artifacts impacted [39]. This is
often the result of what Herzig and Zeller [41] defined as tangled
commits: commits grouping together several unrelated activities,
such as fixing a bug and adding a new feature.
In other cases, a single cohesive change (e.g., a bug fix) is instead split across several commits. This can be due to omitted code
changes and/or the need for fixing a mistake done in the first attempt to implement the change. Park et al. [54] showed that 22% to
33% of bugs require more than one fix attempt (i.e., supplementary
patches). 
Thus,there is no study broadly investigating the types of changes that
developers tend to omit during implementation activities.
We present a qualitative study focusing on “quick remedy commits” performed by developers. We define as quick remedy commits
those commits that (i) quickly succeed a commit performed by the
same developer in the same repository; and (ii) aim at remedying
to issues introduced as the result of code changes omitted in the
previous commit (e.g., fix references to code components that have
been broken as a consequence of a rename refactoring) and/or of
introduced errors. In other words, we identified pairs of commits
(ci , ci+1) that are temporally close (i.e., ci+1 succeeds ci by a few
minutes), are performed by the same developer, and include in the
commit note of ci+1 a reference to fixing issues introduced in ci.
Software systems are continuously modified to implement new
features, to fix bugs, and to improve quality attributes. Most of these
activities are not atomic changes, but rather the result of several
related changes affecting different parts of the code. For this reason,
it may happen that developers omit some of the needed changes
and, as a consequence, leave a task partially unfinished, introduce
technical debt or, in the worst case scenario, inject bugs. Knowing
the changes that are mistakenly omitted by developers can help
in designing recommender systems able to automatically identify
risky situations in which, for example, the developer is likely to be
pushing an incomplete change to the software repository.
In Section 2 they present the design of
our empirical study, and discuss its results in Section 3. In Section 4
we discuss the threats that could affect the validity of our study. In
Section 5 we discuss the related literature, while in Section 6 we
draw our conclusions and outline our future work.

Research Methodology:
This category groups the pairs of commits (ci , ci+1) in which the
remedy commit (i.e., ci+1) implements a refactoring/cleanup of the
code changed in ci
(see Fig. 4). In these commits developers are
either not satisfied of the code they implemented or are trying to
address warnings received by static analyzers.

Results:
They presented a qualitative empirical study aimed at investigating
quick remedy commits performed by developers in GitHub projects.
We defined quick remedy commits as commits performed by developers to remedy to changes omitted or errors introduced in a
previous commit, performed just a few minutes before.
Our study is based on the manual analysis of 500 commits, that
we classified by looking at the objective of the remedy commit (i.e.,
why the remedy commit was performed). The output of our study
is represented by the taxonomy depicted in Fig. 4. We used several
qualitative findings to distill lessons learned resulting in actionable
items for both researchers and practitioners (Section 3).
Our future work will target two directions. First, we plan to
enlarge the set of commits manually analyzed to test the generalizability and completeness of the defined taxonomy. Second, we will
work on some of the research directions discussed in our results
section, and summarized in the following:
Automatic bug fixing. Developing approaches able to learn how to
automatically fix the “simple” bugs that, as shown in our study, are
fixed by developers within a few minutes from their introduction.
We believe that approaches based on deep learning (see e.g., [65])
can be particularly performant in this specific context.
Automatic identification of omitted changes. Integrating approaches
to identify locations for missed code changes in a continuous integration pipeline, to alert developers when changes they are committing are likely to be incomplete.
Learning coding conventions. Investigating novel techniques to
learn coding conventions, enlarging the set of conventions that
are currently supported by state-of-the-art techniques [25]. Once
learned, the coding conventions can be automatically checked on
the code to commit, raising a warning in case violations are detected.
On the impact of reverted commits on MSR studies. Studying the
impact that reverted commits have on the findings of MSR studies
using the change history of software systems as basic information
to compute a variety of proxies (e.g., developers’ experience, changeproneness of code) is also part of our research agenda.

				   The End

