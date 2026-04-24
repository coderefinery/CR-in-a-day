# Social coding

```{objectives}
- Get familiar with terminology around licensing.
- Practical advice for software licensing and citations
```

These materials are adopted from CodeRefinery lesson [Social Coding](https://coderefinery.github.io/social-coding/).
This is not legal advice! Please always consult your organizations legal team when in doubt.


## Relevance for data stewards

You may not be writing or releasing software yourself, but you are often asked to:

* Advise on licensing choices
* Interpret reuse conditions
* Assess whether software outputs can be shared
* Help make software citable and compliant with policy.

Social coding is as much about **people, rules, and expectations** as it is about tools.

## Comparing sharing papers and sharing code

```{figure} img/sharing-papers.jpg
:alt: Image shows that we are motivated sharing our published papers since we get rewarded with academic credit in form of citations

Citation as one form of academic credit to motivate sharing papers.
```

Sharing papers and academic credit:
- The goal is maximum visibility and maximum reuse.
- The more interesting science is done referencing my paper, the better for me.
- Nobody actively tries to limit the reach of their papers.

```{figure} img/sharing-code.jpg
:alt: Getting improvements back and also getting citations can motivate us to share code

Different ways we can benefit from sharing code.
```

Sharing code:
- "I did all the ground work and they get to do the interesting science?"
- Sharing code and encouraging *derivative work* may boost your academic impact.
- But will your work be visible if it is used two levels deep down?


## Journal policies as motivation for sharing

From [Science editorial policy](https://www.sciencemag.org/authors/science-journals-editorial-policies):
> "We require that **all computer code used for modeling and/or data analysis**
> that is not commercially available be deposited in a **publicly accessible repository**
> upon publication. In rare exceptional cases where security
> concerns or competing commercial interests pose a conflict, code-sharing
> arrangements that still facilitate reproduction of the work should be
> discussed with your Editor no later than the revision stage."

From [Nature editorial policy](https://www.nature.com/authors/policies/availability.html):
> "An inherent principle of publication is that others should be able to
> replicate and build upon the authors' published claims. A condition of
> publication in a Nature Research journal is that authors are required to make
> **materials, data, code, and associated protocols promptly available** to readers
> without undue qualifications. Any restrictions on the availability of
> materials or information must be disclosed to the editors at the time of
> submission. Any restrictions must also be disclosed in the submitted
> manuscript."

These policies may surface during data stewardship consultations, not just at submission time.

However [a study](https://www.pnas.org/content/115/11/2584) showed that despite
these policies, many people still do not share their code 😞.  This paper
includes samples of charming author responses such as:
> "When you approach a PI for the source codes and raw data, you better explain
> who you are, whom you work for, why you need the data and what you are going
> to do with it."


## Motivation for open source software


- Enable derivative work
- Do not lock yourself out of own code
- Attract developers who want to be able to show the coding work on their CVs
- Tightly regulated domains require open source
- Open-source software (OSS) can lead to more engagement from industry which may lead to more impact
- If it's not open, it is not likely to become standard


## Sharing software is also scary

- **Fear of being scooped**:
  A license can avoid it, and you can release when you are ready. Anyway, it is
  very unlikely that others will understand your code and publish before you
  without involving you in a collaboration. Sharing is a form of publishing.
- **Exposes possibly "ugly code"**:
  In practice almost nobody will judge the quality of your code.
  "Software, once written, is never really finished" (N. Asparouhova).
- **Others may find bugs and mistakes**:
  Isn't this good? Would you not like to use a code which gives people the chance to locate bugs?
  If you don't release, people will assume there are bugs anyway.
- **Others may require support and ask too many questions**:
  This can become a problem: use tools and community and protect your time.
  You aren't required to support anyone. You can also "archive" a repository to disable
  most forms of interaction (issues, PRs). Also a note in README on support level helps.
- **Fear of losing control over the direction of the project**:
  Open source does not mean everybody can change **your version**.
- **"Bad" derivative projects may appear**:
  It will be clear which is the official version.


## Code reusability: What contributes to reusability?

What contributes to you being able to reuse stuff that others make, and others
(or you) being able to reuse your stuff?  When you find a repository with code
you would like to reuse, you may look at the following things to determine its
reusability:


- **Date of last code change**: Is the project abandoned?
- **Release history**: How about stability and backwards-compatibility?
- **Versioning**: Will it be painful to upgrade?
- **Number of open pull requests and issues**: Are they followed-up?
- **Installation instructions**: Will it be difficult to get it running?
- **Example**: Will it be difficult to get started?
- **License**: Am I allowed to use it?
- **Contribution guide**: How to contribute and decision process?
- **Code of conduct**: How to make clear which behaviors are unacceptable and
  discouraged? How violations of Code of conduct will be handled?
- **Trust and community**: Somebody you trust recommended it?

... most of which you can learn in the [CodeRefinery](https://coderefinery.org) workshop!


## How our work connects to the work of others

```{figure} img/in-out.jpg
:alt: Our work depends on ideas, articles, data, and software

Whether and what we can share depends on how we obtained the components.
```

- Our work depends on outputs from others. Research of others depends on our outputs.
- Whether you can share your output depends on how you obtained your input.
- A repository that is private today might become public one day.
- Sometimes "OTHERS" are you yourself in the future in a different group/job.
- Our code often starts by changing other code: **derivative work**.
- **Software licenses** matter. And this is what we will discuss in the next episode.



## Copyright

```{figure} img/tate.jpg
:alt: Photo of somebody taking a photo of an artwork that contains the text "WHO OWNS WHAT?"
:width: 50%
```

- **Trademark**: Protects a name/brand from impersonation.
- **Patent**: Protects a novel, non-obvious, technical invention.
- **Copyright**: Protects **creative expression**: software, writing, graphics, photos, certain datasets, this presentation.
  Practically "forever" (lifetime of author + 70 years).

Copyright controls whether and how we can distribute the original work or the **derivative work**.

## Taxonomy of software licenses

["Software licensing
and open source explained with
cakes"](https://cicero.xyz/v3/remark/0.14.0/github.com/coderefinery/social-coding/main/licensing-and-cakes.md/).

```{figure} img/license-models.png
:alt: "European Union Public Licence (EUPL): guidelines July 2021"

European Commission, Directorate-General for Informatics, Schmitz, P., European Union Public Licence (EUPL): guidelines July 2021, Publications Office, 2021, <https://data.europa.eu/doi/10.2799/77160>
```

Comments:
- Arrows represent compatibility (A -> B: B can reuse A)
- Proprietary/custom: Derivative work typically not possible (no arrow goes from proprietary to open)
- Permissive: Derivative work does not have to be shared
- Copyleft/reciprocal: Derivative work must be made available under the same license terms
- NC (non-commercial) and ND (non-derivative) exist for data licenses but not really for software licenses 

**Great resource for comparing software licenses**: [Joinup Licensing Assistant](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-find-and-compare-software-licenses)
- Provides comments on licenses
- Easy to compare licenses ([example](https://joinup.ec.europa.eu/licence/compare/BSD-3-Clause;Apache-2.0))
- [Joinup Licensing Assistant - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker)
- Not biased by some company agenda

As we do here, data stewards should be careful not to give legal advice, but can:

* Explain common licenses
* Highlight compatibility issues
* Point researchers to institutional or legal support when needed.


## Software citation

```{questions}
- Is putting software on GitHub/GitLab/... publishing?
- Where to publish software?
- How can software be cited?
- How can I make my software citeable?
```


### Is putting software on GitHub/GitLab/... publishing?

```{figure} img/turing-way/8-fair-principles.jpg
:alt: FAIR principles
:width: 70%

FAIR principles. (c) [Scriberia](http://www.scriberia.co.uk) for [The Turing Way](https://the-turing-way.netlify.com), CC-BY.
```

Is it enough to make the code public for the code to remain **findable and accessible**?
- No. Because nothing prevents me from deleting my GitHub repository or
  rewriting the Git history and we have no guarantee that GitHub will still be around in 10 years.
- **Make your code citable and persistent**:
  Get a persistent identifier (PID) such as DOI in addition to sharing the
  code publicly, by using services like [Zenodo](https://zenodo.org) or
  similar services.


### How to make your software citable


**Checklist for making a release of your software citable**:

- Assigned an appropriate license
- Described the software using an appropriate metadata format
- Clear version number
- Authors credited
- Procured a persistent identifier
- Added a recommended citation to the software documentation

This checklist is adapted from: N. P. Chue Hong, A. Allen, A. Gonzalez-Beltran,
et al., Software Citation Checklist for Developers (Version 0.9.0). Zenodo.
2019b. ([DOI](https://doi.org/10.5281/zenodo.3482769))

**Our practical recommendations**:
- Add a file called [CITATION.cff](https://citation-file-format.github.io/) ([example](https://github.com/bast/runtest/blob/main/CITATION.cff)).
- Get a [digital object identifier
  (DOI)](https://en.wikipedia.org/wiki/Digital_object_identifier) for your code
  on [Zenodo](https://zenodo.org/) ([example](https://zenodo.org/record/8003695)).
- [Step-by-step recipe](https://coderefinery.github.io/github-without-command-line/doi/)
  for how to make your GitHub project citable using [Zenodo](https://zenodo.org/).
- Make it as easy as possible: clearly say what you want cited.

This is an example of a simple `CITATION.cff` file:
```yaml
cff-version: 1.2.0
message: "If you use this software, please cite it as below."
authors:
  - family-names: Doe
    given-names: Jane
    orcid: https://orcid.org/1234-5678-9101-1121
title: "My Research Software"
version: 2.0.4
doi: 10.5281/zenodo.1234
date-released: 2021-08-11
```

More about `CITATION.cff` files:
- [GitHub now supports CITATION.cff files](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files)
- [Web form to create, edit, and validate CITATION.cff files](https://citation-file-format.github.io/cff-initializer-javascript/)
- [Video: "How to create a CITATION.cff using cffinit"](https://www.youtube.com/watch?v=zcgLIT5Qd4M)


### Papers with focus on scientific software

Where can I publish papers which are primarily focused on my scientific
software?  Great list/summary is provided in this blog post: ["In which
journals should I publish my software?" (Neil P. Chue
Hong)](https://www.software.ac.uk/top-tip/which-journals-should-i-publish-my-software)


### How to cite software

```{admonition} Great resources
- A. M. Smith, D. S. Katz, K. E. Niemeyer, and FORCE11 Software Citation
  Working Group, "Software citation principles," PeerJ Comput. Sci., vol. 2,
  no. e86, 2016 ([DOI](https://doi.org/10.7717/peerj-cs.86))
- D. S. Katz, N. P. Chue Hong, T. Clark, et al., Recognizing the value of
  software: a software citation guide [version 2; peer review: 2 approved].
  F1000Research 2021, 9:1257 ([DOI](https://doi.org/10.12688/f1000research.26932.2))
- N. P. Chue Hong, A. Allen, A. Gonzalez-Beltran, et al., Software Citation
  Checklist for Authors (Version 0.9.0). Zenodo. 2019a. ([DOI](https://doi.org/10.5281/zenodo.3479199))
- N. P. Chue Hong, A. Allen, A. Gonzalez-Beltran, et al., Software Citation
  Checklist for Developers (Version 0.9.0). Zenodo. 2019b. ([DOI](https://doi.org/10.5281/zenodo.3482769))
```

Recommended format for software citation is to ensure the following information
is provided as part of the reference (from [Katz, Chue Hong, Clark,
2021](https://doi.org/10.12688/f1000research.26932.2) which also contains
software citation examples):
- Creator
- Title
- Publication venue
- Date
- Identifier
- Version
- Type


```{keypoints}
- **You cannot ignore licensing**: default is "no one can make copies or
  derivative works".
- Citation.cff files can make it easier for others to cite software and provide credit.
```