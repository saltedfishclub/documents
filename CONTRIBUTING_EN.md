# Some Tips on Contributing


## Description

If a project is not specifically not required to follow the code contribution specification or has separate rules, then use the specification described in this document.  
This document is advisory, but that does not mean you can ignore everything.  

# Communication

See [code terms](CODE_OF_CONDUCT.md) for details

# Submitting code

Committing code is a common occurrence, but irregular commits can be difficult to review and maintain.  
Therefore, for the purpose of project maintainability, we recommend that you do the following:

1. The code should be simple and easy to understand, and consistent with the general coding style of the project. This requires you to look at the general structure of the project and the libraries used before committing (e.g. don't write Getter by hand if you can use `@Getter`, etc.)
2. don't introduce new dependencies unless necessary, and look carefully to see if what you want is already there. Do communicate with Maintainer or other Collaborator before introducing dependencies.
3. standard commit information and commit size. (One Commit for one small thing, one PR for one large thing)  
  * For new features (e.g. new code modules, components), open a new branch and a Pull Request with `[WIP]` in front of the title.

4. Do not change the version number without permission. 
5. When opening a PR, consider naming it `issue-xx` if it is related to an issue and mention `This resolves/closes #xx` in the body of the PR (so GitHub can automatically relate it to the issue).
6. Before merging PRs **you must wait for all workflows to finish** and resolve all Requested Changes and reply to all Comments from Assignee or Maintainer.
7. The Assignee of each PR must read the submitted code carefully before it is ready to be merged. Merging PRs without an Assignee is not allowed.

## Submission Information Specifications
If not specified, we use [Angular Submission Specification](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#-commit-message-format) to specify the commit message format.  

The commit message requires that it must contain what was done in a clear and concise manner.

## Other considerations

1. **Avoid premature optimization** Spend your time on more meaningful things (think of your pile of issues?). If there are real problems with this part, we'll come back to it later.
2. When submitting a large PR, please briefly describe what changes you have made. 
3. Remember to thank the contributor.

# End
