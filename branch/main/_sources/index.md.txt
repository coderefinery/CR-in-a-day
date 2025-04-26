# CodeRefinery in a day

This course provides an introduction to essential practices in research software engineering, with a strong focus on collaboration, reproducibility, and sustainability. Participants will learn the fundamentals of version control and how to effectively collaborate on texts in GitHub. The course also explores key concepts in reproducible research, including organizing projects, a brief overview of environments and containers. In addition, it covers the social aspects of coding, such as software licensing, citation, and open collaboration. By the end, learners will know about best practices for developing and sharing research software more efficiently and transparently.

This course is a condensed version of the [CodeRefinery workshop](https://coderefinery.org/lessons/#lessons-that-we-teach-in-our-tools-workshops)



:::{prereq}

To follow the course, you will need a GitHub account: [Instructions](./getting-ready.md)

:::

## Why is this important?

When in doubt if what you are doing is important in research, always reflect using the Allea European Code of Conduct for Research Integrity (2023)

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

Please note that some of the materials are hosted in other repositories. Make sure to always come back here to find the next link.

```{csv-table}
:delim: ;
:widths: auto

9:15-10:00 ; Introduction to Version Control [motivation](https://coderefinery.github.io/git-intro/motivation/) and [sharing](https://coderefinery.github.io/git-intro/sharing/) 
10:00-10:10 ; Break 
10:10-11:00 ; [Collaborating with git](./collaborativegit.md) 
11:00-12:00 ; *Lunchbreak*
12:00-12:50 ; Collaborating with git exercise
12:50-13:00; Break
13:00-14:00 ; **[Reproducibility and code](https://coderefinery.github.io/reproducible-research)**: 
5 min; Reproducible research intro
10 min; Reproducible research motivation
15 min; Organizing projects
15 min; Environments and containers
14:00-14:10 ; Break
14:10-14:45; **Social coding**: 
10 min;  [Social coding](https://coderefinery.github.io/social-coding/)
10 min;  [Software licensing with cake](https://cicero.xyz/v3/remark/0.14.0/github.com/coderefinery/social-coding/main/licensing-and-cakes.md/#1)
5 min;  [Software licensing](https://coderefinery.github.io/social-coding/software-licensing/)
10 min;  [Software citation](https://coderefinery.github.io/social-coding/software-citation/)
14:45-15:00; [Wrapup](./wrapup.md) 
```

```{toctree}
:caption: The lesson
:maxdepth: 1

getting-ready.md
Motivation for version control <https://coderefinery.github.io/git-intro/motivation/>
Sharing your work <https://coderefinery.github.io/git-intro/sharing/>
collaborativegit.md
Reproducible research intro <https://coderefinery.github.io/reproducible-research/intro/>
Reproducible research motivation <https://coderefinery.github.io/reproducible-research/motivation/>
Project organization <https://coderefinery.github.io/reproducible-research/organizing-projects/>
Social coding <https://coderefinery.github.io/social-coding/>
Software licensing with cake <https://cicero.xyz/v3/remark/0.14.0/github.com/coderefinery/social-coding/main/licensing-and-cakes.md/#1>
Software licensing <https://coderefinery.github.io/social-coding/software-licensing/>
Software citation <https://coderefinery.github.io/social-coding/software-citation/>
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
