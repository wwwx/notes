---
title: Ranger cheat sheet
tags:
  - shell
  - vim
categories:
  - shell
---

### General

| Shortcut | Description                 |
| -------- | --------------------------- |
| `ranger` | Start Ranger                |
| `Q`      | Quit Ranger                 |
| `R`      | Reload current directory    |
| `?`      | Ranger Manpages / Shortcuts |

<!-- more -->

### Movement

| Shortcut | Description          |
| -------- | -------------------- |
| `k`      | up                   |
| `j`      | down                 |
| `h`      | parent directory     |
| `l`      | subdirectory         |
| `gg`     | go to top of list    |
| `G`      | go to bottom of list |
| `J`      | half page down       |
| `K`      | half page up         |
| `H`      | History Back         |
| `L`      | History Forward      |
| `~`      | Switch the view      |

### File Operations

| Shortcut  | Description                |
| --------- | -------------------------- |
| \<Enter>  | Open                       |
| `r`       | open file with             |
| `z`       | toggle settings            |
| `o`       | change sort order          |
| `zh`      | view hidden files          |
| `cw`      | rename current file        |
| `yy`      | yank / copy                |
| `dd`      | cut                        |
| `pp`      | paste                      |
| `/`       | search for files `:search` |
| `n`       | next match                 |
| `N`       | prev match                 |
| \<Delete> | Delete                     |

### Commands

| Shortcut | Description                                                                |
| -------- | -------------------------------------------------------------------------- |
| `:`      | Excute Range Command                                                       |
| `!`      | Excute Shell Command                                                       |
| `chmod`  | Change file Permissions                                                    |
| `du`     | Disk Usage Curren Directory                                                |
| `s`      | Run the terminal in your current ranger window (exit to go back to ranger) |

### Tabs

| Shortcut    | Description           |
| ----------- | --------------------- |
| `<C-n>`     | Create new tab        |
| `<C-w>`     | Close current tab     |
| tab         | Next tab              |
| Shift + tab | Previous tab          |
| Alt + [n]   | goto / create [n] tab |

### File substituting

| Shortcut | Description                         |
| -------- | ----------------------------------- |
| `%f`     | substitute highlighted file         |
| `%d`     | substitute current directory        |
| `%s`     | substitute currently selected files |
| `%t`     | substitute currently tagged files   |

Example for substitution
`bulkrename %s`

### Marker

| Shortcut        | Description                       |
| --------------- | --------------------------------- |
| `m + <letter>`  | Create Marker                     |
| `um + <letter>` | Delete Marker                     |
| `' + <letter>`  | Go to Marker                      |
| `t`             | tag a file with an \*             |
| `t"<any>`       | tag a file with your desired mark |
