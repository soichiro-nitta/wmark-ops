# Gotchas

- `CGWindow ID` is useful but not permanent. It can change when a window is closed, recreated, or the app restarts.
- Chrome tab identity is not the same as macOS window identity. Store URL and tab title when available.
- Window thumbnails may contain sensitive data. Store them only in local Git-ignored paths and expire them quickly.
- Hovering a list item should show a preview, not foreground or move another Space by default.
