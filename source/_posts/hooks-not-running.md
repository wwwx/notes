---
title: hooks-not-running
date: 2022-01-26 10:47:49
tags:
  - Git
---

- 1. Ensure that you don't have a typo in your filename. `precommit` or `pre-commit.sh` are invalid names. see Git hooks [documentation](https://git-scm.com/docs/githooks) for valid names.
- 2. Check that `git config core.hooksPath` returns `.husky`(or your custom hooks directory).
- 3. Verify that hook file are excutable. This is automatically set when using `husky add` command but you can run `chmod +x .husky/<hookname>` to fix that.
- 4. Check that your version of Git is greater than 2.9.
- 5. husky hooks: calling `package.json` scripts(**husky@4**), calling `.husky` files(**husky@7**)
