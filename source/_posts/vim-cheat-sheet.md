---
title: Vim Cheat Sheet
date: 2021-12-28 15:57:34
tags:
- vim
categories:
- cheatsheet
---

# Fold (by indent) #

```bash
set foldmethod=indent   
set foldnestmax=10
set nofoldenable
set foldlevel=2
```

<!-- more -->

| Shortcut                                     | Description                                           |
|----------------------------------------------|-------------------------------------------------------|
| <kbd>z</kbd> <kbd>o</kbd>                    | opens a fold at the cursor                            |
| <kbd>z</kbd> <kbd>shift</kbd> + <kbd>o</kbd> | opens all fold at the cursor                          |
| <kbd>z</kbd> <kbd>c</kbd>                    | closes a fold at the cursor                           |
| <kbd>z</kbd> <kbd>m</kbd>                    | increases the foldlevel by one                        |
| <kbd>z</kbd> <kbd>shift</kbd> + <kbd>m</kbd> | closes all open folds                                 |
| <kbd>z</kbd> <kbd>r</kbd>                    | decreases the foldlevel by one                        |
| <kbd>z</kbd> <kbd>shift</kbd> + <kbd>r</kbd> | decreases the foldlevel to zero (all folds will open) |
