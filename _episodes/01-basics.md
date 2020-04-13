---
layout: episode
title: Basics and motivation
teaching: 20
exercises: 0
questions:
  - What is version control and why?
  - What are commits and branches?
  - What are forks and clones?
objectives:
  - Get a mental representation for commits and branches.
  - Understand the difference between forks and clones.
  - Understand the difference between Git and GitHub.
---

> ## Goal of this tutorial
>
> - Get a grasp of Git and GitHub without the command line
>
> ### What we will not cover
>
> - Command line interface
> - Cloning using SSH protocol and SSH keys
> - Rebasing and squashing
> - Many Git tricks which can be explored later
{: .discussion}

## Version control

### What are version control tools?

- Version control is a tool that can **record snapshots of a project**.
- You can think of version control like regularly taking a photo of your work
  (movie sets take regular polaroids to be able to recreate a scene the next day).


### What we typically like to snapshot

- Software (this is how it started but Git/GitHub can track a lot more)
- Scripts
- Documents (plain text file much better suitable than Word documents)
- Manuscripts
- Configuration files
- Website sources
- Data


### Why are snapshots valuable? Reproducibility!

- We have the means to refer to a well-defined version of a project when sharing, collaborating, and publishing.
- If we discover a problem, we can find out when it was introduced.

---

## Difference between [Git](https://git-scm.com) and [GitHub](https://github.com)

**Git**
- Tool that can record and synchronize snapshots.
- Not the only tool that can record snapshots (other popular tools are
[Subversion](https://subversion.apache.org) and [Mercurial](https://www.mercurial-scm.org)).

**GitHub**
- Service that provides hosting for Git repositories with a nice web interface.
- Not the only service that provides this (other popular services are
[GitLab](https://about.gitlab.com/) and [Bitbucket](https://bitbucket.org)).

---

## Commits, branches, repositories, forks, clones

- Commit: snapshot of the project, gets a unique identifier (e.g. `c7f0e8bfc718be04525847fc7ac237f470add76e`)
- Branch: independent development line, often we call the main development line `master`
- Tag: like a sticky note that you attach to a particular commit
- Repository: the project, contains all commits, all branches, all tags
- Cloning: copying the whole repository to your laptop
- Forking: taking a copy of a repository (which is typically not yours) - they
  copy stays on GitHub and you can make changes to the copy


### Interesting repositories to explore these concepts

- Event Horizon Telescope imaging software
  - Repository: [https://github.com/achael/eht-imaging](https://github.com/achael/eht-imaging)
  - Commits, branches, forks: [https://github.com/achael/eht-imaging/network](https://github.com/achael/eht-imaging/network)
- [Activity inequality study](http://activityinequality.stanford.edu/)
  - Data: [https://github.com/timalthoff/activityinequality/tree/master/data](https://github.com/timalthoff/activityinequality/tree/master/data)
- FiveThirtyEight story [Why We’re Sharing 3 Million Russian Troll Tweets](https://fivethirtyeight.com/features/why-were-sharing-3-million-russian-troll-tweets/)
  - Data: [https://github.com/fivethirtyeight/russian-troll-tweets](https://github.com/fivethirtyeight/russian-troll-tweets)
- The NY Times Coronavirus (Covid-19) Data in the United States
  - Data: [https://github.com/nytimes/covid-19-data](https://github.com/nytimes/covid-19-data)
  - Website: [https://www.nytimes.com/interactive/2020/us/coronavirus-us-cases.html](https://www.nytimes.com/interactive/2020/us/coronavirus-us-cases.html)
- CSV exports of the Getty Provenance Index
  - Data: [https://github.com/thegetty/provenance-index-csv](https://github.com/thegetty/provenance-index-csv)


### [Example](https://github.com/achael/eht-imaging/network)

<img src="{{ site.baseurl }}/img/commits-and-branches.svg" width="800px">

---

> ## Why using repositories?
>
> - All changes are recorded.
> - We do not have to send changes via email.
> - We can experiment with several ideas which might not work out (using branches).
> - Several people can work on the same project at the same time (using branches).
> - We do not have to wait for others to send us "the latest version" over email.
> - We do not have to merge parallel developments by hand.
> - It is possible to serve websites directly from a repository.
{: .discussion}