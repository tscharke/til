# Using sed

Bash allows you to perform pattern replacement using variable expansion with `sed`(**s**tream **ed**itor).

To replace a value means, we're searching for this value and replacing it with another one.

## Replace characters

To replace all `e`'s with a upercae `X`:

```bash
echo "replace all es in this line" | sed 's/e/X/g'

rXplacX all Xs in this linX
```

## Remove value

Removing is also a kind of replacement. We're searching for value and replacing it with _nothing_.

```bash
echo "remove all spaces of this line" | sed 's/ //g'

removeallspacesofthisline
```

## Using special characters

In my cases, special characters are characters like: `:`, `/` and so on.

To remove the scheme of an URI including `://`:

```bash
echo "https://www.example.com" | sed 's#https://##g'

www.example.com
```

Here I use `#` instead of `/` for _sed_ to avoid conflicts with the searching value: `https://`.
