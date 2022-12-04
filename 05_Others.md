# Update & Delete

Test delete untracked file:
```bash
$ git clean -n
```

Delete untracked file:
```bash
$ git clean -f
```

Unstage / undo adds:
```bash
$ git reset HEAD {file-name}
```

# Reflog

```bash
$ git reflog

$ git reset --hard {ssh-link}
```

# Using SSH

```bash
$ git remote -v
$ git remote set-url origin git@github.com:username/repo-name.git
```

No need to give password every time.

# Git Settings with GitHub

```bash
$ ssh-keygen -t rsa -b 4096 -C "githubMail"
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/id_rsa
$ vim .ssh/id_rsa.pub    # copy the value inside
$ ssh -T git@github.com
```

