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



GitHub is one place to **find the source** of software, webpages, presentations, books, games, and a **place to collaborate** and share. Hosting service for Git repositories with web interface -> Share and collaborate; Others: GitLab, Codeberg, ...

Git is a tool/format for version control ; Command line or inbuilt (VSCode etc); Others: [Subversion](https://subversion.apache.org),[Mercurial](https://www.mercurial-scm.org), [Pijul](https://pijul.org/)...



## What we typically like to snapshot

- Software (this is how it started but Git/GitHub can track a lot more)
- Scripts
- Documents (plain text files much better suitable than Word documents)
- Manuscripts (Git is great for collaborating/sharing LaTeX or [Quarto](https://quarto.org/) manuscripts)
- Configuration files
- Website sources
- Data (better options available!)

Do not use this for:

- Secrets
- Passwords
- Binaries; files that are difficult to diff
- Files generated from builds


## Difficulties of version control

Despite the benefits, let's be honest, there are some difficulties:

- One more thing to learn (it's probably worth it and will save you more time in the long run; basic career skill).
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

  **In-house GitLab**: Host your own repositories safely within the walls of your organisation.

Collaboration in the Nordics: [Nordic GitLab hosted by DeIC](https://coderefinery.org/repository/)

Why do we teach GitHub? ➡ Most used, beyond borders



## Terms

### Repositories - a place to store

<br>
<br>

.quote[A repository is the most basic element of GitHub. It's a place where you can **store your code**, your files, and each file's **revision history**. Repositories can be **owned by persons or organisations**, have **multiple collaborators** and can be either **public or private**]

.cite[Adapted from <https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories>]

???

Store everything, with history of changes
Ownership
Collborators
Open/closed

## Commit - a snapshot

.left-column50[
.center[
<img src="img/slides/camera.svg"
     alt="camera icon"
     style="height: 100px;"/>
]
<br>

.quote[Snapshot of current state of your repository
... like taking a picture with metadata]
]


.right-column40[

<br>
<br>
<br>

- Who?
- What?
- Why? -> Commit message!
- When?

]

???

Commit messages make the history

# (Optional) Clone - download

<br>

.center[
<img src="img/slides/github.svg"
     alt="GitHub logo"
     style="height: 150px;"/>


<br>

.quote[...get the latest (working) version on your computer]
]

???

Not only the files but also the history.


## Is sharing your work on GitHub making it reproducible?

.center[
<img src="img/slides/version_control_reproducibility.png"
alt=""
style="height: 350px;"/>
]


➡ Only in combination with other steps! **Computing environment**: Conda, Pip, Poetry, ...; **Persistent identifier**: Zenodo, ...

.footnote[Barker, M., Chue Hong, N.P., Katz, D.S. et al. Introducing the FAIR Principles for research software. Sci Data 9, 622 (2022). https://doi.org/10.1038/s41597-022-01710-x]'

???

You share your work, that is one of the steps!

----


# My own GitHub repository

<br>

## ... continue work on GitHub

1. Work on it, make updates on GitHub, ...
2. Commit when done (per file): take snapshots of units of work (one)

---


# Quick demo (please just watch):

<br>
<br>

.center[

All materials for this session are on GitHub too!

<https://github.com/samumantha/github-jupyter-4-ds>

.quote[Finding a typo in my own repository...]

]

???

Typo is in the README!





---

# (Optional) My own GitHub repository

## ... continue work locally

1. Clone: get a copy to my computer
2. Work on it, make updates, ...
3. Add, Commit: take snapshots of units of work (one or many)
4. Push: submit snapshots to GitHub

.quote[Pull: Get latest version from GitHub]

---


class: center, middle

<img src="https://raw.githubusercontent.com/hendrixroa/in-case-of-fire-1/master/in_case_of_fire.png"
     alt=""
     style="height: 450px;"/>

.cite[from <https://raw.githubusercontent.com/hendrixroa/in-case-of-fire-1/master/in_case_of_fire.png>]

---

# Demo: Starting new 

Just watch for now. 

.center[
### <https://github.com/>
.cite[See also: <https://samumantha.github.io/github-jupyter-4-ds/creating-repo-using-web/>]
]


.left-column50[
Create a new repository

- Namespace
- Name
- Description
- README
- LICENSE
- `.gitignore`
]

.right-column50[
Add new file

- Edit
- (Special: license/citation.cff)
- Commit
- `main`

History

Annotate
]

???

New file: type license or citation.cff into filename and check options
Annotate: File -> Preview - Code - Blame


---

# Making a suggestion 

<br>

Full workflow **GitHub**:

1. Suggest idea: issue
2. Discussion -> OK
3. Separate your work: branch / fork
4. Work: work - commit (one or more) 
6. Suggest work: pull request 
7. Accept: merge

➡ You made it to history!

???

This is the workflow for any repo you find on GitHub

---

# (Optional) Making a suggestion 

<br>

Full workflow **local**:

1. Suggest idea: issue
2. Discussion -> OK
3. Get the work: (fork) - clone - pull 
4. Work: work - add - commit (one or more) 
5. Put it on GitHub: push 
6. Suggest work: pull request 
7. Accept: merge

➡ You made it to history!

---

# (Optional) Demo - exploring an existing repo 

Just watch :)

<br>
<br>

- History
- Branches
- Forks
- Issues
- Pull requests

<br>

➡ <https://github.com/the-turing-way/the-turing-way/>

---

# Demo - contribute

You may suggest your own recipes!

<br>

- History
- Issue
- Fork / Branch
- Work
- Pull request

New file vs changing file

<br>

➡ <https://github.com/samumantha/data_support_recipe_book>

???

Commit history: 
- Who?
- What?
- Why? -> Commit message!
- When?


```{keypoints}
- TODO
``` 