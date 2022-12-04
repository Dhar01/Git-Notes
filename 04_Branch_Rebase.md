Create a new branch:
```bash
$ git branch {branch-name}
```

Switch to an existing branch:
```bash
$ git checkout {branch-name}
$ git switch {branch-name}    # new
```

Switch to previous branch:
```bash
git checkout -
```

Create a new branch and switch to it:
```bash
$ git checkout -b {branch-name}
```

Rename branch:
```bash
$ git branch -m {branch-name} {new-branch-name}
$ git branch --move {old-branch-name} {new-branch-name}
```

Show all branches that are merged into current branch:
```bash
$ git branch --merged
```

Delete a branch:
```bash
$ git branch -d {branch-name}
```

List all branches:
```bash
$ git branch
```

View all branches - *local & remote*:
```bash
$ git branch -a
```

Remove remote branch:
```bash
$ git push --delete origin {branch-name}
```

Delete unmerged branch:
```bash
$ git branch -D {branch-name-to-delete}
```

> **HEAD** is where we right now in the repository. The **HEAD** points to the last commit in the branch we  are currently on.

# Merge

There are two types of merging:
1. **Fast-forward-merge**: It happens when current branch has no extra commits compared to the branch we're merging.
2. **No-fast-forward-merge**: If the master branch has new changes which other branch doesn't have, git will commit no-fast-forward merge.
- - -
First checkout to master branch:
```bash
$ git checkout master
```

Merging:
```bash
$ git merge {branch-name}
```

Merge on master branch (*only if fast forward*):
```bash
$ git merge --ff-only {branch-name}
```

Merging on master branch (*forcing a new commit*):
```bash
$ git merge --no-ff {branch-name}
```

Stop merge (*in case of conflicts*):
```bash
$ git merge --abort
$ git reset --merge        # prior to v1.7.4
```

Undo local merge:
```bash
$ git reset  --hard {branch-name}
```

Merge a specific commit:
```bash
$ git cherry-pick {commit-ID}
```

Rebase:
```bash
$ git checkout {branch-name} >> git rebase main
```

Cancel rebase:
```bash
$ git rebase --abort
```

Squash multiple commit to one commit:
```bash
$ git rebase -i HEAD~3
```

Squash merge in one commit:
```bash
$ git merge --squash {branch-name}  # (and commit afterwards)
```
