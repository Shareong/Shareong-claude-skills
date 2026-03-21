---
name: commit
description: Create a git commit with a well-structured conventional commit message. Use after completing each logical unit of work.
disable-model-invocation: true
allowed-tools: Bash
---

Create a conventional commit for ALL current changes (staged and unstaged).

1. Run `git add -A` to stage everything
2. Run `git diff --staged --stat` to see what files changed
3. Run `git diff --staged` to review the actual changes (if too long, use `--stat` summary only)
4. Determine the type: feat / fix / docs / refactor / test / chore
5. Determine scope from the files changed (e.g., "card", "api", "homepage")
6. Write a concise commit message: `type(scope): description`
7. Run `git commit -m "type(scope): description"`
8. Show the commit result
