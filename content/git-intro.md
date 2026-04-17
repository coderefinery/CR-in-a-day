# Introduction to version control

:::{objectives}
- Understand the basic principles of version control and interactive computing platforms to support computational reproducibility.
- Utilize the basic features of Git(-Hub) and Jupyter notebooks.
- Know where those tools can be run and found.
:::

:::{info}
This materials is adoopted from CodeRefinery lesson XX
:::

It is normal that it may be overwhelming. Take it as a starting point and come back when you want to try something new. You may not have use for these tools yourself, but good to know anyway to potentially forward researchers.

- Version control is the practice of **tracking and managing changes over time**.
- You can think of version control like regularly taking a photo ("snapshot") of your work.


## Why do we need to keep track of versions?

**Problem: If you have to identify and find your code from 17 days
ago, can you?**

Version control is an answer to the following questions (do you recognize some
of them?):

- "It broke ... hopefully I have a working version somewhere?"
- "Can you please send me the latest version?"
- "Where is the latest version?"
- "Which version are you using?"
- "Which version have the authors used in the paper I am trying to reproduce?"
- "Found a bug! Since when was it there?"
- "I am sure it used to work. When did it change?"
- "My laptop is gone. Is my thesis now gone?"


## Features: roll-back, branching, merging, collaboration

**Problem: Your code worked two days ago, but is giving an error now.
You don't know what you changed.**

**Problem: You and your colleague want to work on the same code at the
same time.**


- **Roll-back**: you can always go back to a previous version and compare

- **Branching and merging**:
  - Work on different ideas at the same time
  - Different people can work on the same code/project without interfering
  - You can experiment with an idea and discard it if it turns out to be a bad idea

:::{figure} img/gopher/gophers.png
:alt: Branching explained with a gopher
:width: 100%

Image created using <https://gopherize.me/>
([inspiration](https://twitter.com/jay_gee/status/703360688618536960)).
:::

- **Collaboration**: review, compare, share, discuss

- [Example network graph](https://github.com/coderefinery/git-intro/network)

- With version control we can **annotate** code
([browse this example online](https://github.com/networkx/networkx/blame/main/networkx/algorithms/boundary.py)):

:::{figure} img/git-annotate.png
:alt: Example of a git-annotated code with code and history side-by-side
:width: 100%
:class: with-border

Example of a git-annotated code with code and history side-by-side.
:::

- Talking about code, showing someone your code
     - "Clone the code, go to the file 'src/util.rs', and search for 'time_iso8601'".
  Oh! But make sure you use the version from August 2023."
     - Or I can send you a [permalink](https://github.com/NordicHPC/sonar/blob/75daafc86582feb06299d6a47c82112f39888152/src/util.rs#L40-L44):

:::{figure} img/code-portion.png
:alt: Screen-shot of a code portion
:width: 100%
:class: with-border

Permalink that points to a code portion.
:::

### Git repositories - a place to store

.quote[A repository is the most basic element of GitHub. It's a place where you can **store your code**, your files, and each file's **revision history**. Repositories can be **owned by persons or organisations**, have **multiple collaborators** and can be either **public or private**]

.cite[Adapted from <https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories>]

Locally, a Git repository is the .git/ folder inside a project. This repository tracks all changes made to files in your project, building a history over time. Meaning, if you delete the .git/ folder, then you delete your project’s history.

.cite[Adapted from <https://www.gitkraken.com/learn/git/tutorials/what-is-a-git-repository>]

## Demo - exploring a repository online

:::{exercise}

Let's browse the [numpy repository on GitHub](xx).

Numpy is a popular Python package used in almost all research code. It has a large community of contributors.

1. Check out the main page: Source code, README, LICENSE
2. Contributors
3. Branches
4. History
5. Commits
6. Clone

:::

## Terminology: Commit

.quote[Snapshot of current state of your repository
... like taking a picture with metadata]

- Who?
- What?
- Why? -> Commit message!
- When?

-> Commit messages make the history!

## Terminology: Clone - download

.quote[...get the latest (working) version on your computer]

Download not only the files, but also the history.

## Git vs GitHub

Git is a tool/format for version control. It can be used via the terminal or be inbuilt to integrated development environments (IDE) like VSCode, RStudio, Jupyter. Alternative tools are for example [Subversion](https://subversion.apache.org),[Mercurial](https://www.mercurial-scm.org), or [Pijul](https://pijul.org/).

GitHub is a osting service for Git repositories with web interface. It is one place to **find the source** of software, webpages, presentations, books, games, and a **place to collaborate** and share.  Alternative services for example [GitLab](xx) and [Codeberg](xx).

## What we typically like to snapshot

- Software (this is how it started but Git/GitHub can track a lot more)
- Scripts
- Documents (plain text files much better suitable than Word documents)
- Manuscripts (Git is great for collaborating/sharing LaTeX or [Quarto](https://quarto.org/) manuscripts)
- Configuration files
- Website sources
- Data (better options available!)

Do not use git for:

- Secrets
- Passwords
- Binaries; files that are difficult to diff
- Files generated from builds


## Difficulties of version control

Despite the benefits, let's be honest, there are some difficulties:

- One more thing to learn (it's probably worth it and as a researcher will save you more time in the long run; basic career skill).
- Difficult if your collaborators don't want to use it (in the worst case, you
  can version control **on your side** and email them versions).
- Advanced things can be difficult, but basics are often enough (ask others for help when needed).


## Why Git and GitHub

Why git?
- **Easy to set up**: no server needed.
- **Very popular**: chances are high you will need to contribute to somebody else's code which is tracked with Git.
- **Distributed**: good backup, no single point of failure, you can track and
  clean-up changes offline, simplifies collaboration model for open-source
  projects.
- Important **platforms** such as [GitHub](https://github.com), [GitLab](https://gitlab.com), and [Bitbucket](https://bitbucket.org)
  build on top of Git.

Note that many organisations have their own **In-house GitLab**: This lets you host your own repositories safely within the walls of your organisation.

For collaboration in the Nordics, data kept in Denmark: [Nordic GitLab hosted by DeIC](https://coderefinery.org/repository/)


## Scenarios for working with GitHub

:::[discussion]


# My own GitHub repository

## ... continue work on GitHub

1. Work on it, make updates on GitHub, ...
2. Commit when done (per file): take snapshots of units of work (one)


# My own GitHub repository

## ... continue work locally

1. Clone: get a copy to my computer
2. Work on it, make updates, ...
3. Add, Commit: take snapshots of units of work (one or many)
4. Push: submit snapshots to GitHub

.quote[Pull: Get latest version from GitHub]



# Starting a new repository


Create a new repository

- Namespace
- Name
- Description
- README
- LICENSE
- `.gitignore`

Add new file

- Edit
- (Special: license/citation.cff)
- Commit
- `main`

History

Annotate

New file: type license or citation.cff into filename and check options
Annotate: File -> Preview - Code - Blame






```{keypoints}
- TODO
``` 