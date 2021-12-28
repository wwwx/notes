---
title: test markdown snippets
date: 2021-12-28 14:43:13
tags: 
- vim
- hexo
categories:
- vim 
---


```bash
snippet head "Hexo post header" b
---
title: ${1:title}
date: `!v strftime("%Y-%m-%d %H:%M:%S")`
tags:
- ${4}
---

${0}
endsnippet
```

