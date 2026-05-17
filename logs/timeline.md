# Timeline

## 2026-05-17

- Decided to create `wmark` as a public macOS window target picker.
- Chose `wmark` as the lowercase name, meaning "window mark".
- Decided to pair the implementation repository with `wmark-ops`.
- Split the MVP plan into `wmark-ops` Issue #1 through Issue #7.
- Added the first Swift CLI experiment on implementation branch `issue-1-window-metadata`.
- Confirmed `CGWindowListCopyWindowInfo` can return visible window metadata, Chrome front tab title/URL can be read through AppleScript, and `CGWindowListCreateImage` can create a local thumbnail. `CGWindowListCreateImage` is deprecated on macOS 14, so ScreenCaptureKit should be evaluated before the production thumbnail path is finalized.
- Recorded the macOS 14 thumbnail deprecation note in `gotchas.md` before continuing MVP implementation.
- Decided the MVP should target macOS windows first. Chrome tab title and URL can remain optional context and do not need to be required for target identity.
- Decided target records should keep one uniform top-level window schema. App-specific fields should be optional context rather than different per-app record shapes.
- Added an early SwiftUI app experiment with scan list, hover preview, click-to-copy, local selection mode, global shortcut registration, cursor-window highlight, and click-to-mark flow.
- Added public-facing privacy and safety documentation to the implementation repository.
