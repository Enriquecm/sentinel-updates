# Sentinel 0.3.0

Released on 12/10/2026 (build 199).

A new design for the whole app, in a dark and a light appearance, and work packages 2.14 to 2.33 of Phase 2 (D85–D100).

- A new look in the dark and the light appearance; Settings → General → Appearance follows the system or keeps one of them (US-14.5).
- Sidebar: one row per repository, grouped by connection, with Claude Code's status pinned at the bottom; each repository and connection has a popover with its details and actions, and a repository can have its own icon (US-4.13, US-1.6, US-2.8).
- Mini sidebar: collapse the sidebar to an 84pt rail of tiles with ⇤, View › Compact Sidebar (⌃⌥⌘S) or by dragging its edge; letting go snaps it to the rail or the full sidebar. Hovering a repository shows its destinations (US-4.14).
- The list has a new header: the repository, the Pull Requests or Merge Requests and Queue tabs with badges for new activity, and the filters with their chips. Each row splits its status into three capsules: Sentinel's review state, the AI review and the provider's checks, each with a tooltip (US-4.13, US-4.16).
- Filters: Quick chips for the common ones, and a page per group in the filters popover. New filters: review requested from me, assigned to me, several authors, reviewers or labels, GitLab approvals left, and the severity of open findings (US-4.17, US-4.12).
- View › List Density: Compact or Regular. The list shows the one that fits its width, and dragging the list's edge chooses it; the width is remembered (US-4.15).
- The four columns adapt together: each keeps a minimum width, the window cannot be made smaller than they need, and opening the right bar or expanding the sidebar makes the window wider when the detail has no room left.
- The item header comes in three sizes with three cards: Sentinel (the review steps and the queue), the provider (checks, your review, threads) and the AI review (its state, findings and actions). It says how many commits arrived since your review and why an AI review failed, in a few words (US-4.18).
- Approve, request changes and undo your approval from the item header, with Draft with AI for the text. On GitLab, request changes needs GitLab 18.9 or later (US-10.11).
- The item detail has two tabs. Overview shows the description and the history. Review shows the conversation in order: comments, threads, commits, reviews, pipeline results with their failed jobs, force pushes and state changes from GitHub or GitLab, with the AI sessions and their findings as drafts in place (US-4.19, US-4.20, US-9.12).
- Reply on, resolve and unresolve any thread, people's and Sentinel's; Draft reply writes the reply for you to edit and send (US-10.12).
- The right bar has three tabs: Details, Chat and Sessions. It opens without a selected item too, and keeps its width when you select one (US-4.21).
- Chat: ask about the whole pull request or merge request (what to test, the riskiest change, a summary); the answers can point to drafts and checks, and the conversation is kept. Chat never changes a finding (US-9.13).
- Focus the next AI review on what matters to you, in up to 500 characters ("check the token storage") (US-8.10).
- Open a completed AI session in Terminal and continue it by hand with Claude Code; completed sessions are kept for 7 days (US-8.11).
- Add Repository: the search finds a repository by any part of its full path, its owner or group included, among the repositories the connection can access (US-2.1).
- Items are named the way their provider names them, #42 on GitHub and !42 on GitLab, and item notifications say the item's review state (US-11.9).
- Notifications when, on a queued item, CI fails or passes again (on by default), the review decision changes, or merge conflicts appear (both off by default) (US-11.10).
- Menu bar: queued items show their checks, how long they have been in the queue and what is new; the icon marks an AI review that failed while you were away, and the menu shows unread notifications (US-12.5).
- Fixed: Cancel did not always stop a running AI review, which then stayed Running; it now stops it and records it as cancelled.
- Fixed: a long line of code in a comment or a draft could freeze the item detail.
- Fixed: emptying a connection's name now gives it back its username, and a repository's icon follows its nickname.
- Fixed: Draft reply shows that the AI is writing, and the focus field waits while a review runs.
