# PAPER#3

**_Title: Measuring Software Testability Modulo Test Quality_**

# Authors:
**1: Valerio Terragni**

**2: Pasquale Salza**

**3: Mauro Pezze**

**_Conference Name:  International Conference on Program Comprehension (13-15 July 2020)._**

Published Date: Tue 14 Jul 2020 02:00 - 02:15 at ICPC - Session 4
 
Summary:
In this paper authors declares that follwing things:
Software testing is an essential, labor-intensive and time-consuming
activity of the software life cycle. Making testing easier is important
for many software companies, as it lowers development costs while
increasing the number of detected faults.
It is well understood that the effort of testing software systems
depends on the artifacts under test, meaning that some software
systems are easier to test than others . Comprehending
the relation between software artifacts and test effort is extremely
important to control the cost of testing and improve the accuracy of
test plans. Software Testability captures the impact of software
artifacts on testing by estimating the degree to which a software
system or component under test supports its own testing.
A software system with a high degree of testability results in a low test effort.
In their recent comprehensive literature review of 208 papers
on software testability, Garousi et al. observe that measuring
and predicting the testability is the topic that received the most
attention. The general idea is to measure (predict)
the test effort of software systems from structural metrics of the
software that are available before designing the test cases.
Early predicting the test effort can help developers to (i) early identify software components that require more test effort, on which
developers have to focus to ensure software quality, (ii) plan testing activities and optimally allocate resources, and (iii) recognize refactoring opportunities to reduce the test effort.
Comprehending the degree to which software components support testing is important to accurately schedule testing activities, train developers, and plan effective refactoring actions. Software
testability estimates such property by relating code characteristics
to the test effort. The main studies of testability reported in the
literature investigate the relation between class metrics and test
effort in terms of the size and complexity of the associated test
suites. They report a moderate correlation of some class metrics to
test-effort metrics, but suffer from two main limitations: (i) the results hardly generalize due to the small empirical evidence (datasets with no more than eight software projects); and (ii) mostly ignore the quality of the tests. The results confirm that some class metrics correlates with testeffort metrics, and indicate that normalizing test-effort metrics
with test-quality metrics drastically improves the correlation (up to
74 %). Better correlation leads to better prediction power, and thus
better prediction of test effort [51]. On the one hand, we use the
test-quality metrics to normalize the test effort for the correlation
analysis, allowing to fairly compare classes belonging to projects of
different test qualities. On the other hand, the test-quality metrics
can also be used as a target variable for prediction purposes. Indeed,
if the purpose is to predict the test effort before writing the tests,
a target value for test quality can be used in a preprocessing step
to normalize the dataset used for training a prediction model. For
instance, one might want to predict the test effort required to write
tests having a target mutation score of 80 %.

Research Methodology:
This paper investigates the relationships between the object-oriented
metrics of classes and the test effort of designing unit test cases
for such classes. We produced statistically significant and general
results for Java software systems, by conducting an experimental
study on a large set of heterogeneous Java software systems of
different size and category. Because heterogeneous projects are
likely to have different test-quality criteria, we introduce a novel
normalization procedure that homogenizes the values of test-effort
metrics according to the values of test-quality metrics.
This section contextualizes the scope of the study (Section 2.1),
presents the considered metrics of class, test effort and test quality  and introduces the new normalization procedure.

Results:
This paper proposes a new software testability approach that extends current practice with the novel idea of normalizing test effort
with respect to test quality. It also presented the results of an extensive study that involves 9,861 pairs of Java classes (with a total of 1,594,309 lines of code) and corresponding JUnit test cases taken
from 1,186 GitHub projects. Their results indicate that normalizing test effort with test quality
largely increases the correlation between class metric and test effort.
An improved correlation between class metric and test effort means
a better prediction of test effort. The normalization procedure that we presented in this paper enables the construction of large-scale prediction models from heterogeneous software systems implemented with different test adequacy criteria. Leveraging our normalization procedure we could train
different machine learning models considering different versions of
our data-set obtained by normalizing test effort by different target
test-quality values, such as 70 %, 80 %, 90 % line coverage. Given
in input a class, its class metrics values, and a target test-quality
value, we could predict the test effort using the prediction model
corresponding to the target test-quality value in input.

				      The End