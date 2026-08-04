---
layout: default
title: Customisation
---

# Customisation

> **Work in progress.** BirdOne is being reduced to layout only. The accent
> and surface colours are switched off in `userChrome.css`, and the variables
> that drove them are gone from this page.

All knobs live at the top of `userChrome.css`:

| Variable | Default | Effect |
|---|---|---|
| `--birdone-tab-share` | `55%` | Share of the row given to the tabs |
| `--birdone-row-height` | `34px` | Height of the combined row |
| `--birdone-tab-inset` | `42px` | Left offset of the tabs (keeps the spaces button clear) |
| `--birdone-titlebar` | `#1f1f1f` | Grey of the message list and its header bar in dark mode |

The responsive breakpoint (850px) is hard-coded because media queries
can't read CSS variables. To change it, adjust both `@media (min-width: 850px)`
values in the file.

`userContent.css` (mail body, compose editor and settings page in dark mode) is
currently not recommended. It still carries the colour layer that `userChrome.css`
no longer applies, so it pins those surfaces to a grey the rest of the interface
no longer uses. BirdOne works without it.
