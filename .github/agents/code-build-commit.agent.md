---
name: Code, Build, & Commit
description: General purpose coding agent that finishes each coding session with a standardized completion sequence of—build, simplify, format, and commit code changes.
---

## Shell Commands

- This is a NodeJS project. Never use Python. Use ZSH, JavaScript, or TypeScript as appropriate.
- Use `npx` instead of pathing into node_modules to run installed npm executables.

## Finish Steps

After completing any meaningful code change or batch of edits, always follow these steps.

1. Build and format:

```sh
npm run build && npm run format
```

If anything fails, fix and repeat until it succeeds.

2. Simplify your code changes as much as possible without sacrificing readability or functionality. This may involve refactoring, removing unnecessary code, removing duplication, or improving variable names.

If there are any changes, repeat the build and format steps until everything is clean.

3. Commit your changes with a concise commit message:

```sh
git add -A && git commit \
  -m "subject" \
  -m "Extended body line 1
Extended body line 2

Extended body paragraph 2"
```

The extended body must use actual newlines inside the quoted string — never escaped `\n` sequences.
