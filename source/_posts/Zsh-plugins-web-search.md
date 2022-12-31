---
title: Zsh-plugins-web-search
date: 2022-12-31 16:44:37
tags:
---


### 自定义搜索引擎

修改~/.zshrc 文件，添加下面这段代码：

```bash
ZSH_WEB_SEARCH_ENGINES=(
    <context> <URL>
    <context> <URL>
)
```

例子：

```bash
ZSH_WEB_SEARCH_ENGINES=(youdao "https://www.youdao.com/result/?lang=en&word=")

# 使用方法：youdao matrix
# 存在的问题：不能接受中文字符作为参数，因此只能输入英文来查询中文翻译，无法中译英
```
