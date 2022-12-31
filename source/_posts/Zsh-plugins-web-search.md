---
title: Zsh plugin - web-search
date: 2022-12-31 16:44:37
tags:
---

### Custom search engine

Open the ``~/.zshrc` file and write the following piece of code：

```bash
ZSH_WEB_SEARCH_ENGINES=(
    <context> <URL>
    <context> <URL>
)
```

Example：

```bash
ZSH_WEB_SEARCH_ENGINES=(youdao "https://www.youdao.com/result/?lang=en&word=")

# useage：youdao matrix
# issue: Chinese cannot be accepted as a parameter, so only English can be
# input to query Chinese translation, not Chinese to English.
```
