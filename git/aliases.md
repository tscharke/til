# Git aliases

You can create git **aliases** for commands you're using in your daily work by using `git config`.

Instead of typing `git commit`, you can use`git ci` (the alias **ci**) by setting a name (**ci**) and the git-command (**commit**) for an alias:

```bash
git config alias.ci commit

# or
git config alias.amend 'commit --amend --reuse-message HEAD'
```

## For every repository (globally)

With the git-option `global` you set aliases for every repository - **globally**:

```bash
git config --global alias.ci commit

# or
git config --global alias.amend 'commit --amend --reuse-message HEAD'
```

[Source](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases)

[Amend commit](amend.md)
