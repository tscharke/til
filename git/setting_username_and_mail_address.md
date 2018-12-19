# Setting username and mail-address

After initialize a new Git-Repository you wanna set your or a different username and mail-address.
You can implement this with the following commands inside your new repository (folder):

## For a single repository

```bash
$ git config user.name "John Doe"
$ git config user.email "John.Doe@example.com"
```

## For every repository (globally)

You need the same data as [for a single repository](#For a single repository) only in addition with the git-option `--global` 

```bash
$ git config --global user.name "John Doe"
$ git config --global user.email "John.Doe@example.com"
```

[Source](https://help.github.com/articles/setting-your-username-in-git/)
