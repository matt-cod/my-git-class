# Basic Version Control

## Version Control

**Version Control** is a system that records changes to a file or a set of files over time so that you can recall specific versions later. It is a critical component of collaborative software development, enabling multiple contributors to work on a project simultaneously without conflicts, tracking changes, and providing a history of modifications

## Difference Between Git and Github

**Git** is primarily a command-line tool, though various graphical user interfaces (GUIs) exist.
It provides features such as branching, merging, and tracking changes in the codebase.
Developers use Git to work collaboratively on projects, manage different versions of their code, and handle codebase history efficiently.

**GitHub**, on the other hand, is a web-based platform that provides hosting for software development using Git.
It is a platform where developers can store and manage their Git repositories, collaborate with others, and utilize various tools and features for project management.

## List 3 Other Github Alternatives

1. GitLab
2. Bitbucket
3. SourceForge

## The Difference Between Git Fetch and Git Pull

**Git Fetch** is primarily used to download changes from a remote repository to your local repository. It updates your remote-tracking branches. It does not automatically merge or apply the changes to your working directory or the branch you are on. Your local branches remain unchanged. It is a safe operation as it does not affect your working directory or introduce any changes to your local branches.
Syntax: `git fetch <remote>`


**Git Pull** is a combination of two actions: it fetches changes from the remote repository and automatically merges them into your current branch. It not only retrieves the changes but also applies them to your working directory and updates the branch you are currently on. If you have local changes that are not committed, git pull will try to merge the remote changes with your local changes. This could result in merge conflicts that need to be resolved manually.
Syntax: `git pull <remote> <branch>`

## Git Rebase and The Command for it

In simple terms, **Git Rebase** is a Git command used to rewrite the commit history by moving or combining commits. It's like taking your changes and putting them on top of the latest changes in the repository.

**Command:**

The basic syntax for `git rebase` is:

`git rebase <base-branch>`

This command takes the commits from your current branch and places them on top of the specified `<base-branch>`.

## Git Cherry-Pick and The Command for it

In simple terms, **Git Cherry-Pick** is a Git command that allows you to pick or copy specific commits from one branch and apply them to another branch. It's like selecting individual changes from one branch and applying them elsewhere.

**Command:**

The basic syntax for `git cherry-pick` is:

`git cherry-pick <commit-hash>`

This command takes the changes introduced by the specified `<commit-hash>` and applies them to your current branch.