# Sentinel 0.3.0

Released on 12/10/2026.

A new design for the whole app, in dark and light, with a new sidebar, list and item detail.

## New

- **A new look** in dark and light. Settings → General → Appearance follows the system or keeps one.
- **Sidebar** with one row per repository, grouped by connection, that collapses to a compact rail (⌃⌥⌘S).
- **Item header** with three cards: your review, the provider's checks and the AI review, including why an AI review failed.
- **The Review tab** shows the whole conversation in order: comments, threads, commits and pipelines, with the AI's findings as drafts in place.
- **Approve or request changes** from Sentinel, with Draft with AI for the text (request changes needs GitLab 18.9 or later). Reply on, resolve and unresolve any thread.
- **Chat** about a whole pull request or merge request: what to test, the riskiest change, a summary.
- **Focus the next AI review** on what matters to you, such as "check the token storage".
- **More filters**: review requested from me, assigned to me, several authors or labels, GitLab approvals left, and the severity of open findings, with quick chips for the common ones.
- **Notifications** when CI fails or passes again on a queued item, when the review decision changes, or when merge conflicts appear.

## Improved

- Compact or Regular list density, and columns that adapt to the window.
- Add Repository finds a repository by any part of its path.
- Continue a completed AI session by hand in Terminal.

## Fixed

- Cancel did not always stop a running AI review.
- A long line of code in a comment could freeze the item detail.
