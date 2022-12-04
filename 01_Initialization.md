Creates new repo in specified directory:
```bash
git init <directory>
```

Copies repo from specified URL:
```bash
git clone <url>
```

Set username for commit in current repo:
```bash
git config user.name "user_name"

# use --global to apply globally
git config --global user.name "username"
```

Set email for commit in current repo:
```bash
git config user.email "email"

# use --global to apply globally
git config --global user.email "email"
```

Enables helpful colorization of command line output
```bash
git config color.ui auto
```

Open the global configuration file in text editor for manual editing:
```bash
git config --global --edit
```

Connect local repo to the remote one:
```bash
git remote add <remote> <link>
```

> The default value for `<remote>` is `origin`.

`.gitignore` is used for a list of files that have to be excluded. This file should be in the root of the local repo.

Edit `.gitignore` file:
```bash
vim .gitignore
```

# Remote repository

Initializing remote repository:
```bash
$ git remote add origin {connection-string.git}
```

List remote repository:
```bash
$ git remote -v
```

Pushing repository:
```bash
$ git push origin master/main
```

Clone repository:
```bash
$ git clone {ssh-link}
```

Update the repository:
```bash
$ git fetch origin master
```

Fetch & merge remote changes:
```bash
$ git pull origin master
```
