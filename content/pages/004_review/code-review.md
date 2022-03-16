Title: Code Review
Lang: en
Category: review
Slug: code-review
Summary: It's review time
Status: published

## Create a Pull Request

On the web, in your repository you can click on the “Pull Requests” tab and create a new pull request. You will pick your branch on the right and choose to merge it back into main.

Alternatively, you can use the github cli to create a pull request (PR).
Write a good description of what you’re trying to achieve in your code change so that reviewers have context. It’s a great idea to link to an existing JIRA or Github issue as well, where the problem may be more fully described and the reviewer will also have the benefit of the comments thread. 

If you have CODEOWNERS added to your repository, a reviewer will automatically be added to your repository. The speed of review turnaround definitely varies, but at Sage we like to review with one or two business days. In addition to any reviewers who were added automatically, you can add additional reviewer(s) who may be subject matter experts or interestsed in a particular fix.

## How do you do a code review?
Google publishes [guidelines](https://google.github.io/eng-practices/review/) for the respective responsibilities of reviewers and code authors. If you have never participated in a code review, it is recommended that you read these.

Some highlights include:

> In general, reviewers should favor approving a CL once it is in a state where it definitely improves the overall code health of the system being worked on, even if the CL isn’t perfect.

> ...if a CL adds a feature that the reviewer doesn’t want in their system, then the reviewer can certainly deny approval even if the code is well-designed.

> Reviewers should always feel free to leave comments expressing that something could be better, but if it’s not very important, prefix it with something like "Nit:"  to let the author know that it’s just a point of polish that they could choose to ignore.

Sage Bionetworks has an open door meeting where code reviews are sometimes discussed, and a Code Review Github team. Lastly, code reviews MUST adhere to the Sage code of conduct linked above.
