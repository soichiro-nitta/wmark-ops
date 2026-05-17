# Timeline

## 2026-05-17

- Decided to create `wmark` as a public macOS window target picker.
- Chose `wmark` as the lowercase name, meaning "window mark".
- Decided to pair the implementation repository with `wmark-ops`.
- Split the MVP plan into `wmark-ops` Issue #1 through Issue #7.
- Added the first Swift CLI experiment on implementation branch `issue-1-window-metadata`.
- Confirmed `CGWindowListCopyWindowInfo` can return visible window metadata, Chrome front tab title/URL can be read through AppleScript, and `CGWindowListCreateImage` can create a local thumbnail. `CGWindowListCreateImage` is deprecated on macOS 14, so ScreenCaptureKit should be evaluated before the production thumbnail path is finalized.
- Recorded the macOS 14 thumbnail deprecation note in `gotchas.md` before continuing MVP implementation.
