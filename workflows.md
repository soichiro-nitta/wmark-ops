# Workflows

## MVP Planning

1. Keep product plans in the implementation repository under `docs/`.
2. Track actionable tasks in GitHub Issues in this repository or the implementation repository depending on scope.
3. Keep sensitive screenshots and local target queues out of Git.
4. Verify macOS APIs with small experiments before committing to UI design.

## Target Safety

1. Treat saved target metadata as a candidate, not truth.
2. Revalidate against current window state before operating.
3. Stop when a target is stale, missing, or ambiguous.
4. Do not move existing windows between Spaces automatically.
5. For the MVP, target macOS windows first. Chrome tab title and URL are optional context, not required identity.
6. Keep target records structurally uniform. App-specific details belong in optional context, not top-level identity fields.
7. Public-facing documentation must explain local target data, thumbnails, and permission needs before app distribution.
