# BirdOne

One-line layout for Thunderbird: tabs and unified toolbar share a single
row, global search hidden (use CTRL+K).

> Tested on Thunderbird 152 (Supernova UI, 115+ required) on Windows.

![preview](https://github.com/Firnschnee/BirdOne/blob/main/assets/preview.png)

### Features

>- Tab bar and unified toolbar merged into one row: tabs on the left, toolbar buttons on the right, next to the window controls
>- Responsive: below 850px window width the layout falls back to the default two-row interface
>- Square popup corners: no rounded inner corners in context menus and panels

### Installation
>
>1. Download [`userChrome.css`](https://github.com/Firnschnee/BirdOne/blob/main/userChrome.css)
>
>2. In Thunderbird go to **Settings → General**, scroll to the bottom and open **Config Editor**. Search for
   **`toolkit.legacyUserProfileCustomizations.stylesheets`** and set it to **`true`**.
>
>3. Recommended: in the same Config Editor set **`mail.tabs.autoHide`** to **`false`**, so the tab bar (and with it the one-line layout) is always visible, even with a single tab.
>
>4. Find your profile folder: **Help → Troubleshooting Information → Profile Folder → Open Folder**.
>
>5. Create a `chrome` folder inside the profile folder if it doesn't exist, then copy `userChrome.css` into it.
>
>6. Restart Thunderbird. The layout applies on restart.

The repository also contains [`userContent.css`](https://github.com/Firnschnee/BirdOne/blob/main/userContent.css) for the mail body, compose editor and settings page. It is work in progress and currently not recommended: it still applies the colour layer that `userChrome.css` no longer does. BirdOne works without it.

### Customisation
>BirdOne is configurable through CSS variables. See all options → [docs/customisation.md](docs/customisation.md)

### Firefox? 
> You are looking for [FoxOne!](https://github.com/Firnschnee/FoxOne)
---
Concept inspired by [@NeroWolfe75's](https://github.com/NeroWolfe75) [one-line experiment from 2023](https://www.reddit.com/r/Thunderbird/comments/15klzpr/oneliner_for_thunderbird/) | License: [MIT](LICENSE)
