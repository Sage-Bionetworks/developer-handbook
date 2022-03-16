Title: Feature Branches
Lang: en
Category: development
Slug: feature-branches
Summary: All about feature branches, huzzah
Status: published

## What's a Feature Branch?
Developers branch from the default branch (hereafter called “main”). The branch created is a feature branch. The best feature branches are created to make a discrete, well-defined change.

## Optimal 
An optimal feature branch:

* Adds one feature or
* Fixes one bug or
* Makes administrative corrections, such as correcting indentation, whitespace, general linting, or adding documentation
* Has a branch name that conveys information about the changes in that branch. A good branch name could include some or all of the following (ideally separated by hyphens or underscores for readability), depending on the team/project:
    * `<author>`
    * `<branch-type>` e.g. ‘bug’, ‘wip’, ‘feature’
    * `<branch-name-or-unique-identifier>` e.g. a JIRA ticket ID 
* Includes a small number of commits with informative and useful commit messages. Note that you can combine a bunch of ‘working commits’ together into a single, focused commit by performing an interactive rebase before pushing your branch. Rewriting commit history after pushing a branch is not recommended.

A sub-optimal feature branch:

* Adds multiple features or
* Fixes lots of bugs or
* Mixes up adding features, fixing bugs, and making administrative corrections.
* Lacks a meaningful name that helps understand what changes it contains
* Includes many commits with messages that aren’t meaningful or helpful

That is, don't do this:

<img src="https://imgs.xkcd.com/comics/git_commit.png" alt="As a project drags on, my git commit messages get less and less informative.">[^1]


[^1]: xkcd is [licensed](https://xkcd.com/license.html) under a Creative Commons Attribution-NonCommercial 2.5 License.