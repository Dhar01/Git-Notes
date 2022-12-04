Lists version history for the current branch:
```bash
git log
```

> Add `--pretty=oneline` to show commit hashes and messages only.

Difference between two commits:
```bash
git diff <commit1> <commit2>
```

> Also applied to comparing two branches. Add `--name-only` to show the file names only.

- Save current changes into stash stack:
(*usually used when current changes don't want to be committed*)
```bash
git stash
```

- Apply last changes stored in stash stack onto current working HEAD:
```bash
git stash pop
```

- Show stash stack:
```bash
git stash list
```

- Create new commit that undoes all of the changes in the `<commit>`:
```bash
git revert <commit>
```

- Undo the commit after `<commit>`:
```bash
git reset <commit>
# keep the changes locally
```

> Add `--hard` to discard the changes.

- Show revision in `<file>` line by line:
```bash
git blame -- <file>
```

# Stash

Save into stash:
```bash
$ git stash save "message"
$ git stash
```

Show list of the stash:
```bash
$ git stash list
```

View all stash:
```bash
$ git stash show
```

Show status of a specific stash:
```bash
$ git stash show {stash-ID}
```

Show changes on stash:
```bash
$ git stash show -p {stash-ID}
```

Bring all stash:
```bash
$ git stash pop
```

Bring/get back to specific stash:
```bash
$ git stash pop {stash-ID}
```

Use specific stash without dropping:
```bash
$ git stash apply {stash-ID}
```

Use custom stash and index:
```bash
$ git stash apply --index
```

Create new branch from stash:
```bash
$ git stash branch {new-branch}
```

Delete 1st item of stash list:
```bash
$ git stash drop
```

Delete specific stash from stash list:
```bash
$ git stash drop {stash-ID}
```

Delete the whole stash:
```bash
$ git stash clear
```

# Compare

Show difference:
```bash
$ git diff {commit-ID} {commit-ID}
```

Compare modified files and highlight changes:
```bash
$ git diff --color-words {file-name}
```

View the difference between last commit and staged version:
```bash
$ git diff --staged
```

Compare branches:
```bash
$ git diff main..{branch-name}
```
