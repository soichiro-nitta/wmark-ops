# Context

`wmark` exists to solve target ambiguity when asking Codex to operate a local Chrome tab or macOS window.

The intended model is explicit user selection. The user marks a window or tab, `wmark` stores short-lived local metadata, and Codex resolves a short target id such as `WTG-A7F3` against current window state.

This replaces the previous Space-based approach. `wmark` should not infer or manipulate macOS Spaces as its primary safety mechanism.
