# Quick Reference


- **Git**: A distributed version control system that tracks changes in files and lets many people collaborate on the same project while preserving full history.

- **GitHub / GitLab / ...** : Web-based platforms that host git repositories and add collaboration features such as issue tracking, pull requests, code review, and CI.

- **Repository**: The project, contains all data and history (commits, branches, tags).

- **Commit**: Snapshot of the project, gets a unique identifier (e.g. c7f0e8bfc718be04525847fc7ac237f470add76e).

- **Branch**: Independent development line for testing, developing, separation from "working version" which is often called `main`.

- **Tag**: A pointer to one commit, to be able to refer to it later. Like a commemorative plaque that you attach to a particular commit (e.g. `phd-printed` or `paper-submitted`).

- **Cloning <clone>**: Copying the whole repository to your laptop – the first time. It is not necessary to download each file one by one.

- **Forking <fork>**: Taking a copy of a repository (which is typically not yours) – your copy (fork) stays on GitHub/GitLab and you can make changes to your copy.

- **Upstream**: The original repository that a fork was created from; often used to pull in updates from the main project.

- **Issue**: A way to report a bug, suggest a change, ask for a change, or discuss an idea.

- **Pull Request (PR)**: Making a contribution; suggesting a change to be incorporated into another branch, a request to merge.

- **Dependency**: External software, library, or tool that your project needs in order to run or be built.

- **Container**: An isolated, lightweight runtime environment that packages software together with its dependencies.

- **Container image**: A static blueprint containing everything needed to run a container (software, dependencies, configuration).

- **Container recipe**: A text file describing how to build a container image (e.g. `Dockerfile`, `Singularity.def`).

- **Reproducibility**: The ability to rerun the same steps and obtain the same results, even at a different time or by a different person.

- **Workflow tool**: Software that automates multi-step processes (e.g. data analysis pipelines), handling dependencies and execution order.
