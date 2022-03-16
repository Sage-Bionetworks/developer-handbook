Title: Development Workflow
Lang: en
Category: development
Slug: development-workflow
Summary: Discussion of various workflow options
Status: published

## Forking versus Providing Write Access
Depending on the nature of the project and the team composition, it may be more preferable to fork (clone) repositories, or to work on the same repository using feature branches. ~The convention at Sage is to favor forking.~

*TODO: insert a discussion of when it’s preferable to promote forking vs. providing write access to repositories.* 

*TODO: insert Thomas’s forking workflow here*

## Version Control Development Style
There are two development styles commonly used at Sage: gitflow and trunk-based development.

This [article](https://www.toptal.com/software/trunk-based-development-git-flow#development-styles) provides a heuristic for deciding when to use gitflow vs. trunk-based development, though their reasoning is a bit flawed, in that they take an all-or-nothing approach on trunk-based development, requiring that all the developers on a project have the ability to merge to the default branch. If you remove that assumption, trunk-based development fits far more use cases.

Learn more about these two development styles:

|Gitflow|Trunk-based|
|-|-|
|[Atlassian: Gitflow Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)|[Atlassian: Trunk-based Development](https://www.atlassian.com/continuous-delivery/continuous-integration/trunk-based-development)|
|?|[Trunk-based Development: Five Minute Overview](https://trunkbaseddevelopment.com/5-min-overview/)|
