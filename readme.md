# qwik-bun-build-issue

Reproduction for Qwik City App build issue when using Bun

## Reproduction

1. Clone this repository via `git clone git@github.com:octet-stream/qwik-bun-build-issue.git`
2. Install dependencis via `bun i`
3. Run `bun run build` and the build process with fail with the following error:

```
$ bun run --bun tsc --incremental --noEmit --pretty
$ bun run --bun vite build
vite v5.1.4 building for production...
✓ 0 modules transformed.
x Build failed in 4ms
error during build:
Error: [vite-plugin-qwik] Not implemented
    at <anonymous> (/Users/octetstream/projects/qwik-bun-build-issue/node_modules/@builder.io/qwik/optimizer.mjs:1435:35)
    at processTicksAndRejections (:12:39)
error: "vite" exited with code 1
error: script "build.client" exited with code 1
error: "qwik" exited with code 1
error: script "build" exited with code 1
```
