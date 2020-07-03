# Git add a tag

To add a new tag (e.g. `v1.0.0`) use the following command:

```bash
git tag v1.0.0
```

If the tag already exists and you wanna _override_ it, use the option `force` like this:

```bash
git tag v1.0.0 --force
```

**NOTE**: Please keep in mind, that _force_'ing a tag means it removes the existing one and set it to the new HEAD.
