---
layout: default
title: Installation
---

# Installation

### 1. Download

Download [`userChrome.css`](https://github.com/Firnschnee/BirdOne/blob/main/userChrome.css) and [`userContent.css`](https://github.com/Firnschnee/BirdOne/blob/main/userContent.css)

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

Create a `chrome` folder inside the profile folder if it doesn't exist, then copy these files into it:

- [`userChrome.css`](https://github.com/Firnschnee/BirdOne/blob/main/userChrome.css) — Thunderbird UI styling
- [`userContent.css`](https://github.com/Firnschnee/BirdOne/blob/main/userContent.css) — mail body and compose editor in dark mode

### 6. Restart Thunderbird

The layout applies on restart.
