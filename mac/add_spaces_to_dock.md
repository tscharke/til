# Add Spaces to the Dock

To add spaces to your Dock, execute the following code (in your `terminal`) so many times, so many spaces you want to insert to your Dock:

```bash
defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'
```

To see the spaces inside your Dock, do a:

```bash
killall Dock
```

**Note**:You only need to `killall` when you have entered in as many spaces as you want.

Seen by [Wes Bos](https://wesbos.com) & [Codes](https://www.youtube.com/watch?v=U46AULbRg4w) by [Jesse Showalter](https://www.youtube.com/channel/UCvBGFeXbBrq3W9_0oNLJREQ)
