Title: Github Repository Creation
Lang: en
Category: Setup
Slug: github-repository-creation
Summary: Suggestions on how to set up a new Github repository.
Status: published

At Sage Bionetworks, git is RECOMMENDED for version control and Github RECOMMENDED for storing and sharing code.

## Naming Conventions
There’s a wide variety of styles in naming repositories, but our RECOMMENDED convention is [kebab-case](https://wiki.c2.com/?KebabCase).

## GitHub Repository Templates
*Status: ok – maybe some links to examples?*

* Language-agnostic template
    * Readme
    * Gitignore (hidden OS files)
    * Code of Conduct
    * Contribution Guidelines
    * Dockerfile (with base alpine/ubuntu?)
* Language-specific templates
    * Gitignore (language-specific rules from [gitignore.io](https://www.toptal.com/developers/gitignore))
    * Package management files (e.g., Pipfile, renv)
    * Language-specific Dockerfile (e.g., python/rocker base image)

## Repository Structure

Specific structure will depend on language and purpose, but there are some general guidelines you SHOULD follow:

1. Create a README.md file at the project root.
1. Create a .gitignore file indicating which files to skip when committing (for example, IDE-specific files and folders).
1. Create a CODEOWNERS file, typically placed under a .github directory. This is a file you use to indicate who owns code. This will allow those people to be notified when a pull request is created (see team and branch protection below).
1. A CODE_OF_CONDUCT.md file that prescribes what is considered acceptable behavior for participation in open source code. Sage follows the Contributor Covenant code of conduct. You SHOULD link to Sage’s page on this rather than copying content that may change over time.


Additionally, some practices are RECOMMENDED:

1. A CONTRIBUTING.md file that indicates how source code in the repository is developed, how to create a pull request, etc. For advice on developing this, see Github’s [guidelines](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors), or some examples from Sage include [challenge-registry](https://github.com/Sage-Bionetworks/challenge-registry/blob/main/.github/CONTRIBUTING.md), [synapsemonitor](https://github.com/Sage-Bionetworks/synapsemonitor/blob/develop/CONTRIBUTING.md), and [nextflow-infra](https://github.com/Sage-Bionetworks-Workflows/nextflow-infra/blob/main/CONTRIBUTING.md).
1. A LICENSE.md file that indicates how the code is permitted to be used. The most common license used at Sage Bionetworks is [Apache 2.0](https://choosealicense.com/licenses/apache-2.0/). 
1. A commit/PR template document to default to. It ensures that every commit/PR has the necessary information to whoever looks at it. This is particularly important for PRs as it informs the reviewers what they’re looking at, the context of the work, etc.
