 # PAPER#2

**Title: UI Screens Identification and Exraction from Mobile Programming Screencasts.**

# Authors:

1: Mohmmad Alahmadi

2: Abdulkarim Khormi

3: Sonia Haiduc

# Conference Name:  International Conference on Program Comprehension (13-15 July 2020).

Published Date: Tue 14 Jul 2020 02:00 - 02:15 at ICPC - Session 4

Summary:
In this paper authors declares that follwing things in their research:
Smartphones are some of the most widely used devices today, with
more than 2.5 billion users worldwide. The two most popular
app stores, the Apple App Store1
and Google Play Store2 host
millions of smartphone applications that people use for a variety
of tasks in their daily lives. The increasing demand for
these applications has spurred growth in mobile app development
with more and more programmers learning to develop new mobile
applications or having to maintain and evolve existing ones.
When learning about new concepts and technologies, debugging,
or looking for answers to programming questions, online resources
are developers’ preferred documentation sources. Screencasts
are particularly on the rise , with tens of millions of
videos available on many programming topics, hosted on platforms
like YouTube3
Mobile applications demand is on the rise, leading to more programmers learning to develop or having to maintain this kind of
programs. Developers often refer to online resources to find inspiration or answers to questions they have about mobile programming
topics and screencasts are a popular resource. However, given the
multitude of screencasts available, it can be difficult to quickly
comprehend which of the many videos is relevant to one’s needs.
We propose a novel approach, called UIScreens, which detects,
extracts, and presents the most representative user interface (UI)
screens embedded in mobile development screencasts. This could
help developers quickly comprehend what an app displayed in a
video is about, therefore saving time searching for useful videos.
UIScreens has been evaluated in two empirical studies on iOS
and Android programming screencasts. The first study investigates
the accuracy of our UI extraction and shows that our approach is
able to detect and extract UI screens with an accuracy of 94%. The
second is a user study with mobile app developers, who evaluated
both the accuracy and the usefulness of UIScreens. They agreed that
UIScreens is accurate and extracts representative UI screens from
videos. They considered that the extracted UI screens are useful for
understanding what a video is about and if it is relevant to a search.
Our approach has been implemented as a free online tool.

Research Methodology:
The study was conducted through an online survey
composed of two main sections. The first section was designed to
capture demographic data, such as the main occupation (professional developer, academic, student) and the mobile programming
experience (iOS and/or Android and number of years) of our participants. Each participant was required to have at least 6 months
experience in at least one of the two mobile programming platforms
to be qualified for participating in our survey. The study participants were recruited through announcements on professional social
media channels.
For this study, we collected a brand new set of 50 programming
screencasts (25 iOS and 25 Android), on which we applied our approach. This was done in order to avoid any bias that could be
caused by applying UIScreens on a video from which frames were
used during the training of our model. This is important for ensuring that our model is generalizable and that our evaluation is
unbiased. The average length of the videos in this study was ~ 10
minutes. Each participant was assigned one iOS and one Android
video. For each of the two videos, they were asked to first watch
the video in its entirety and then evaluate the extracted UI screens
by indicating their agreement level with two statements. The first
statement referred to the sufficiency of the extracted UI screens
(“The list of UI screens extracted is sufficient to understand what
are the main concepts discussed in the video”) and the second one
referred to their uniqueness (“The list of UI screens extracted does
not present duplicate information, i.e., all UI screens presented are
unique”).

Results:
In this paper, they proposed a novel approach, called UIScreens, to
locate and extract UI screens embedded in mobile programming
screencasts, with the purpose of offering developers a UI-focused
overview of a video. Our approach extracts the deep features from
video frames using a CNN and these features are then fed into an
object detector to identify the exact location of UI screens within the
video frames. UIScreens was also implemented as a freely available
tool. We conducted two evaluation studies to assess our approach
in terms of its accuracy, and the quality and usefulness of its results.
The evaluation showed that UIScreens was able to accurately classify and locate UIs in video frames. Additionally, UIScreens received positive feedback from mobile developers, showing potential for
our approach to help developers in navigating and understanding
the contents of mobile programming screencasts. To our knowledge,
UIScreens is the first approach to perform UI screen extraction from
mobile development screencasts.
In their future work, we plan to explore and identify in more detail
the particular GUI elements present in the extracted UI screens and
to allow indexing and searching based on UI element types (e.g.,
drop-down list). Furthermore, we plan to conduct more user studies
where professional developers and computer science students get to
evaluate our tool in the context of specific program comprehension
and UI programming tasks. We also plan to explore UI extraction
from other types of programming videos besides those focused on
mobile applications.


				  The End