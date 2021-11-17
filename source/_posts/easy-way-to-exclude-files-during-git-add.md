---
title: Easy way to exclude files during git add
date: 2021-11-17 17:00:16
tags:
	- Git
---

Every day we use the "git add" command a lot to add our changes to the index for new commits, but have you ever wondered how we can add all the changed files with some files excluded during the execution of this command (not with .gitignore)? If the answer is yes, then this article will help you to understand how certain files can be excluded during the git add command.

## TLDR; command to exclude specific file

```bash
git add -A ':!<file_path>'
```

<!-- more -->
## Problem
One day I was put in a situation where I need to add some files for my new commit but I also need to exclude a few files during that execution and those files will get added later on once my work is done on those.

### One way to do this is to hit the below command

```bash
git add <file_path> <file_path> ... <file_path>
```

Basically, If I have done changes to under 13 files and wanted to exclude only 3 files from those, that means 10 files need to be added with the git add command, then I have to copy all those 10 files path and paste it to the terminal manually and it will have become little bit tedious task. Let’s look at the example.

```bash
git add Dockerfile \
README.md \
nest-cli.json \
package-lock.json \
package.json \
src/app.controller.spec.ts \
src/app.controller.ts \
src/app.module.ts \
src/app.service.ts \
src/main.ts
```

After this command, you can now check for the staged files by hitting.

```bash
git status
```

## Solution

But what if this process can be done inversely🤔? Like instead of passing 10 files paths I could just pass 3 files path, 👀 yes you heard it right this can be possible with git add with the below example.

```bash
git add -A ':!.eslintrc.js' ':!.gitignore' ':!.prettierrc'
```

And now when you hit git status it will show all 10 files added to the index apart from the 3 excluded files. It's like a NOT (!) operator under the git add path option.
