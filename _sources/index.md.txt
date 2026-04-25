# CodeRefinery in a day

```{figure} img/coderefinery-logo.png
:alt: CodeRefinery logo
:width: 200px
:align: right
```

This course provides an introduction to essential practices in research software engineering, with a strong focus on collaboration, reproducibility, and sustainability. Participants will learn the fundamentals of version control and how to effectively collaborate on texts in GitHub. The course also explores key concepts in reproducible research, including organizing projects, a brief overview of environments and containers. In addition, it covers the social aspects of coding, such as software licensing, citation, and open collaboration. By the end, learners will know about best practices for developing and sharing research software more efficiently and transparently.

This course is a condensed version of the [CodeRefinery workshop](https://coderefinery.org/lessons/#lessons-that-we-teach-in-our-tools-workshops)



:::{prereq}

To follow the course, you will need a GitHub account: [Instructions](./getting-ready.md)

:::

## Why is this important?

When in doubt if what you are doing is important in research, always reflect using the [Allea European Code of Conduct for Research Integrity (2023)](https://allea.org/code-of-conduct/)

```{figure} img/allea-coc-cover.png
:alt: Allea European Code of Conduct for Research Integrity 2023 cover
:width: 130px
:align: right
```

The four Allea principles are:

- **Reliability** in ensuring the quality of research, reflected in the design, methodology, analysis, and use of resources.
- **Honesty** in developing, undertaking, reviewing, reporting, and communicating research in a ***transparent***, fair, full, and unbiased way.
- **Respect** for colleagues, research participants, research subjects, society, ecosystems, cultural heritage, and the environment.
- **Accountability** for the research ***from idea to publication***, for its management and organisation, for training, supervision, and mentoring, and for its wider societal impacts.

Transparency and accountability from idea to publication are fundamental requirements of reproducible research. What we will cover in this course are all the necessary steps needed so that the *computational/methodological/digital* part of the research work is done transparently and allows others to verify and reproduce it.  

**However**, we are not *just* doing this to follow research integrity principles, we are also doing this to improve how we work with other collaborators, and especially **we do this to help our future self** so that it can always be possible to travel back in time and see what was done at a certain part of the research process.

![Final.doc from PhDComics](http://www.phdcomics.com/comics/archive/phd101212s.gif) 

([Source](https://phdcomics.com/comics/archive.php?comicid=1531))



## Schedule

```{csv-table}
:delim: ;
:widths: auto

9:15-09:25 ; [Welcome, notes, icebreaker and setup](getting-ready.md)
9:25-9:30 ; Intro (this page)
9:30-9:40 ; [Motivation for version control, terminology](git-intro.md)
9:40-10:20 ; [Exercise type along](git-intro.md#exercise-our-first-repository)
9:55-10:05 ; Break
10:05-10:20 ; [Sharing](git-intro.md#working-with-my-own-github-repository)
10:20-10:25 ; [History and summary](git-intro.md)
10:25-11:00 ; [Collaborate on git](git-collaborative.md)
11:00-12:15 ; Lunch break
12:15-12:30 ; [Exercise in breakoutrooms](git-collaborative.md#exercise---suggesting-a-change-on-a-repository-you-do-not-own)
12:30-13:00 ; [Demo - How PRs look, code review and merge, issue linking, history, branch naming](git-collaborative.md#how-to-approach-other-peoples-repositories-with-ideas-changes-and-requests)
13:00-13:10 ; Break
13:20-13:25 ; [Reproducible research, motivation](reproducible_research.md#motivation)
13:25-13:45 ; [Discuss reading assignment in breakoutrooms](reproducible_research.md#discussion-reading-assignment)
13:45-14:00 ; [Other topics in reproducible research](reproducible_research.md)
14:00-14:10 ; Break
14:10-14:20 ; [Motivation on social coding](social_coding.md)
14:20-14:35 ; [Licensing](social_coding.md#taxonomy-of-software-licenses)
14:35-14:45 ; [Software citations](social_coding.md#software-citation)
14:45-14:55 ; [Connecting to other topics](wrapup.md#connection-to-data-steward-work)
14:55-15:00 ; [Wrap-up](wrapup.md)
```




```{toctree}
:caption: The lesson
:maxdepth: 1

getting-ready.md
git-intro.md
git-collaborative.md
reproducible_research.md
social_coding.md
wrapup.md
```

```{toctree}
:caption: Reference
:maxdepth: 1

quick-reference
guide
```

(learner-personas)=

## Who is the course for?

This course is for you, if you are in a position where you might want to support researchers with programming and its reproducibility. 

This course is not designed for "professional software engineers" or to make you one.

## About the course

In this course, you will get a quick overview of tools and best practices for research software development. This course will not teach a programming language, but we aim to show you some tools and techniques to be able to guide researchers to do programming well and avoid common inefficiency traps. The tools we teach are practically a requirement for any researcher who needs to write code. The main focus is on using Git for efficiently writing and maintaining research software or other content.

## See also

[All lessons of a full CodeRefinery workshop](https://coderefinery.org/lessons/#lessons-that-we-teach-in-our-tools-workshops)

You can also find recordings of the full lessons on Youtube:
- Version Control: [Intro pt 1](https://www.youtube.com/watch?v=0u2K7KJBL-U&list=PLpLblYHCzJACpOmIzO8TywjtfYD7_d93H&index=2) , [intro pt 2](https://www.youtube.com/watch?v=8uay_XoNRck&list=PLpLblYHCzJACpOmIzO8TywjtfYD7_d93H&index=4), [collaborative version control](https://www.youtube.com/watch?v=4Uf7eVSCZeU&list=PLpLblYHCzJACpOmIzO8TywjtfYD7_d93H&index=6)
- [Reproducible research](https://www.youtube.com/watch?v=dWemSikTR3A&list=PLpLblYHCzJACpOmIzO8TywjtfYD7_d93H&index=7)
- [Social coding](https://www.youtube.com/watch?v=qUc7PN0NNvk&list=PLpLblYHCzJACpOmIzO8TywjtfYD7_d93H&index=8)

[Full playlist on youtube](https://www.youtube.com/playlist?list=PLpLblYHCzJACpOmIzO8TywjtfYD7_d93H>), inlcuding also Documentation, Jupyter, modular code develeopment and automated testing.

## Credits

The CodeRefinery contributors for lessons introduction to version control, collaborative git, reproducible research and social coding. 