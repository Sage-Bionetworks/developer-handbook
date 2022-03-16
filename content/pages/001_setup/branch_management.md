Title: Branch Protection
Lang: en
Category: Setup
Slug: branch-protection
Summary: Suggestions on how to set up Github teams.
Status: published

Branch protection is a tool for encouraging the desired behavior from contributors. This is accomplished by setting up a rule requiring a pull request before merging. The default setting will allow admins to override this requirement, which is useful if you need to perform an emergency merge to fix a problem.

To set up branch protection, go to Settings > Branches and create a branch protection rule for your default branch (usually “main” or “master”). For example, a common pattern is to set up a branch protection rule for main that:

1. Requires a pull request before merging
1. Requires at least one approval
1. Requires an approved review by Code Owners
