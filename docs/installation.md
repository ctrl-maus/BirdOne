---
layout: default
title: Installation
---

# Installation

### 1. Download

Download [`userChrome.css`](https://github.com/Firnschnee/BirdOne/blob/main/userChrome.css)

### 2. Enable custom stylesheets

In Thunderbird go to **Settings → General**, scroll to the bottom and open **Config Editor**, then set:

```
toolkit.legacyUserProfileCustomizations.stylesheets = true
```

### 3. Keep the tab bar visible (recommended)

In the same Config Editor set:

```
mail.tabs.autoHide = false
```

so the tab bar (and with it the one-line layout) is always visible, even with a single tab.

### 4. Find your profile folder

**Help → Troubleshooting Information → Profile Folder → Open Folder**

### 5. Copy the files

Create a `chrome` folder inside the profile folder if it doesn't exist, then copy
[`userChrome.css`](https://github.com/Firnschnee/BirdOne/blob/main/userChrome.css) into it.

### 6. Restart Thunderbird

The layout applies on restart.

---

The repository also contains [`userContent.css`](https://github.com/Firnschnee/BirdOne/blob/main/userContent.css)
for the mail body, compose editor and settings page. It is work in progress and
currently not recommended: it still applies the colour layer that `userChrome.css`
no longer does, so it pins those surfaces to a grey the rest of the interface no
longer uses. BirdOne works without it.
