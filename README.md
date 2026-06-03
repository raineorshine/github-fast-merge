# github-fast-merge

A Chrome extension that merges GitHub PRs with a single keyboard shortcut.

## What it does

Press **Cmd+Shift+M** (Mac) or **Ctrl+Shift+M** (Windows/Linux) on any GitHub PR page to:

1. Verify all checks have passed
2. Tick the bypass rules checkbox (if present)
3. Click the merge button
4. Confirm the merge

A toast notification reports success or the reason it stopped.

## Local Development

```sh
npm run dev
```

Load the `dist/` folder as an unpacked extension in `chrome://extensions`. Do not run `npm run build` or it will overwrite the dev manifest.

## Build & Release

This _will_ overwrite the `dist/` manifest, so you'll need to restart the dev server after building.

```sh
npm run build
```
