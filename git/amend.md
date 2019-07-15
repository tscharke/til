# Amend commit

Sometimes we forget to commit files, leave `console.log`'s in or whatever.

To avoiding commits like _removed console.log_ you can add your changes to the last commit (`amend`) and reuse the old commit message (`reuse-message`).

```bash
git commit --amend --reuse-message HEAD
```

[Source](https://dev.to/antjanus/my-personal-git-tricks-cheatsheet-23j1)
