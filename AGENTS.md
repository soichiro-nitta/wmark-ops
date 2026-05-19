# wmark Ops Guidance

## Scope

- This repository is the operations source of truth for `wmark`.
- `wmark` is the macOS window target picker for safely passing local window targets to Codex.
- Execution tasks, planning, release notes, and implementation tracking should use GitHub Issues.

## Source Of Truth

- Product code and user-facing docs live in `soichiro-nitta/wmark`.
- This repository stores operating rules, planning notes, issue structure, and release/checklist context.

## Safety

- Do not store credentials, cookies, browser profiles, raw screenshots with sensitive information, or private user data in this repository.
- Window thumbnails and target queues belong only in local Git-ignored paths such as `~/.codex/window-targets/`.
- Do not design flows that move existing user windows between macOS Spaces automatically.
- External posts, releases, destructive operations, or repository setting changes require user confirmation before execution.

## Files

- `context.md`: product background and operating assumptions.
- `workflows.md`: repeated project workflows.
- `gotchas.md`: risks and design constraints.
- `logs/timeline.md`: timeline index. Monthly entries live under `logs/timeline/YYYY-MM.md`.
- `issue-templates/`: issue body templates.

## Issue Usage

- Use Issues for MVP tasks, research tasks, design decisions, and release tracking.
- Issues should include purpose, completion conditions, constraints, and verification notes.
- When a task is completed, leave a short result and close the issue.
