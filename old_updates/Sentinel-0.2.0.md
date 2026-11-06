# Sentinel 0.2.0

First Phase 2 release (V1 polish, D70, D71, D77): work packages 2.1 to 2.12.

- Review Rules: while you edit a rule, the editor shows how many open items it matches ("Matches 3 open items, 1 excluded"); excluded items are the ones you removed from the queue by hand (US-5.6).
- Review Rules: unsaved changes are no longer lost. Selecting another rule, Add Rule, Done, the close button and ⌘W ask whether to save, discard or cancel (US-5.7).
- Fixed: removing a criterion from a rule crashed Sentinel.
- Lists and queues say how many commits arrived since you last opened the Review tab ("2 new commits"); without a count yet they still say "New commits" (US-4.10).
- Menu bar: the Review Queue counts by state (To Review, In Review, Changes Available, Review Done), each opening the queue, and a sparkle next to the icon while an AI review runs (US-12.3).
- Fixed: with the inspector open in a window of the default size, the item header was drawn outside its column and Start Review or Add to Queue did nothing when clicked. The header, the queue and AI controls, the findings filter bar and finding rows now adapt to a narrow column.
- Notifications can be muted for an hour, until tomorrow morning or until you turn them back on, for everything (menu bar, Settings → Notifications) or for one repository (its menu in the sidebar, its Notifications settings). Muted notifications still appear in Notifications; the menu bar icon and the repository show a muted bell (US-11.5).
- Findings: Explain asks the AI to explain a finding in its conversation, without changing the finding (US-9.10).
- After new commits, Review Changes reviews only the commits since the last AI review, with the rest of the change as context; its menu still offers the whole change. The diff comes from your local clone when there is one, else from GitHub or GitLab. The session says "changes since session N" (US-8.9).
- Activity Log: filter by category (Connections, Sync, Rules and queue, Review, AI, Findings, Publishing) and search item titles, repository names and event details, across the whole log; Clear resets every filter (US-13.4).
- Menu bar: the Review Queue grouped by state (To Review, Changes Available, In Review), each item with Start Review or Mark Review Done, Run AI Review or Review Changes, Open in Browser and Remove from Queue (US-12.4).
- Notifications: banners have Open, Start Review, Run AI Review and Mark as Read where they apply; while an item's notification is unread, later ones update it ("3 updates on #42") instead of piling up; the events chosen in Settings → Notifications apply to every repository, and a repository can use its own choice (US-11.6 to US-11.8).
- Activity Log: group by day or by item; an item's history shows its AI sessions on the timeline, and clicking one opens it (US-13.5).
- Lists, queues and the item header show CI status, the review decision, merge conflicts and unresolved threads, with a filter for each (US-4.11).
- Findings: reply on a published finding's thread on GitHub or GitLab, resolve the thread, or both; Draft with AI writes the reply for you to edit and send (US-10.10).
- Published findings follow their code when lines are inserted above them or the branch is rebased; they go stale only when the lines under them change (US-9.11).
- AI sessions: ask about the whole review in the session's own conversation, where the AI can propose new findings; Compare shows a session against another one: new, fixed and still present (US-9.9).
