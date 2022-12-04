Add path into staging (*file or directory*):
```bash
git add <path>
```

Removes path from staging back to unstaged area:
```bash
git restore --staged <path>
```

Removes path and adds that change into staging:
```bash
git rm -r <path>
```

Commits the stage with specified message:
```bash
git commit -m <message>
```

Repair last commit with specified new message:
```bash
git commit --amend -m <message>
```

> Change `-m <message>` to `--no-edit` to repair without editing commit message.

Check the list of which files are staged, unstaged, or untracked:
```bash
git status
```

Upload a branch to same branch in remote: 
```bash
git push <remote> <branch>
```

Update local branch with all new commits from remote branch with rebasing, avoiding the conflict with changes from remote:
```bash
git pull -r
```

# Log

List of git log:
```bash
$ git log
```

View logs in one line (*awesome!*):
```bash
$ git log --oneline
```

List of changed files:
```bash
$ git log --name-only
```

View commit log in one line with full SHA-1 format:
```bash
$ git log --format=oneline
```

View changes:
```bash
$ git log -p
```

View commits of a specific file:
```bash
$ git log {file-name}
```

View all commits of a specific file:
```bash
$ git log -p {file-name}
```

View status & summary of commits:
```bash
$ git log --stat
$ git log --stat --summary
```

View commit history in graph:
```bash
$ git log --graph
```

View summary of commit history in graph:
```bash
$ git log --oneline --graph --all --decorate
```

View previous commit history:
```bash
$ git log --graph --decorate
```
