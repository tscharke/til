# Add/set a tag

To add a new tag (e.g. `v1.0.0`) use the following command:

```bash
git tag v1.0.0
```

If the tag already exists and you wanna _override_ it, use the option `force` like this:

```bash
git tag v1.0.0 --force
```

## Tag a specific/older commit

Sometimes you want to tag a specific/an older commit (e.g. hash `2dae1750`).
This is a easy as adding a new tag. 😉

The syntax is: `git tag {TAG_NAME} {HASH OF COMMIT} [--force]`

If you want to tag the commit `2dae1750` with the new tag `new-tag` you can do it like this:

```bash
git tag new-tag 2dae1750
```

And if you want to tag the commit `2dae1750` with an existing commit:

```bash
git tag v1.0.0 2dae1750 --force
```

**NOTE**: Please keep in mind, that _force_'ing a tag means it removes the existing one and set it to the new HEAD.
