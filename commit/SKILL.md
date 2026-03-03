---
name: commit
description: Create a git commit with a well-structured conventional commit message. Use when user asks to commit changes.
disable-model-invocation: true
allowed-tools: Bash
---

Create a conventional commit for the current staged changes.

1. Run `git diff --staged` to review what's staged
2. Determine the type: feat/fix/docs/refactor/test/chore
3. Write a concise commit message in the format: `type(scope): description`
4. Run `git commit -m "<message>"`
5. Show the commit hash after success
