# Sentinel 0.5.0

Released on 06/11/2026 (build 449).

The first modules: the context of a pull request or merge request, kept current, and Topics that group the work around one subject; the Settings window rebuilt as System Settings; following repositories you are not a member of; Undo and Redo; back and forward. Work packages 3.1 to 3.34 of Phase 3 (D115–D201).

**Context**

- Settings → Context turns the Context module on. It reads your own Claude Code's MCP servers, read-only: Settings → Sources lists them, signs you in where a server asks, and lets you mark the read tools of a server Sentinel does not know (US-15.1, US-16.1 to US-16.4).
- A pull request's or merge request's Context tab gathers what it relates to, from its sources (Slack, Jira, Bitrise, Confluence, Claude Code sessions and others), into a summary whose every statement names its records. You follow a gather as it runs, stop it, read what the AI found and confirm or dismiss it, open each record, and go back to an earlier update (US-17.1 to US-17.8).
- A context is checked when its tab shows and it is older than the age you choose, under a daily limit of automatic reads. The tab and the rows say when it was last checked, what changed since you last looked, and when an update is not seen yet (US-17.9 to US-17.12).
- The repository bar says when its list was last updated, and the item's header when the item was last read (D147, D148).

**AI usage and the spending guard**

- Every AI run is recorded, whatever started it. Settings → AI › Usage and budget shows today, 7 and 30 days, split by module, feature and model; Home shows today's use (US-18.1, US-18.2).
- A daily budget ($10 to start) and an optional monthly one: Sentinel warns at 80% and, at the budget, stops automatic runs until the next day, saying where it stopped one; the runs you ask for keep running (US-18.3, US-18.4).

**Topics**

- Topics in the sidebar group pull requests, merge requests and links about one subject, with a state, a History and a context of their own gathered from their items' contexts and their own links (US-20.1 to US-20.5).
- Sentinel suggests a Topic when items share a ticket, a thread or a build, or when the AI proposes one; you accept, edit or dismiss it, and a dismissed one comes back only when what it rested on changed, or when you restore it (US-20.6).
- A merge request's Topics tab, Add to Topic (⌥⌘T), and a popover on each of a Topic's pull requests or merge requests with how it stands, with Open in New Window (US-20.7, US-20.4).
- Follow a Topic to have it read at an interval and to be told when it changes; Topics is a module that can be turned off, keeping or deleting its data (US-20.8 to US-20.12).

**Settings**

- One window as System Settings: a sidebar with search, ‹ › between the pages, changes that apply at once and Apply for the ones that cost (US-19.1, US-19.2).
- Accounts holds each connection and repository as a page, and the Defaults every repository follows until it has its own value; Review, Context and Topics have panes of their own, and each source a page (US-19.3 to US-19.6).

**Review**

- Follow a repository you are not a member of, such as a public project, by pasting its URL in Add Repository. Sentinel never publishes there by itself, keeps AI Review at Manual to start, and shows each write your access does not allow disabled with why; the repository carries a NOT A MEMBER tag, and if you stop being a member, automatic publishing turns off and Sentinel tells you (US-21.1 to US-21.3).
- The list's search, New Topic's and the Topics list's find a pull request or merge request by its number: 57, !57 or #57 (D198).
- Edit › Undo and Redo (⌘Z, ⇧⌘Z) undo your own actions on Sentinel's data, per window: Start Review and Mark Done, the queue, a finding's Accept or Ignore, Mark All Read, a Topic's state, links, title and follow, and a mute. A step is undone only while it is as you left it, and Sentinel says why when it is not; writes on GitHub or GitLab are not undone (US-22.1, US-22.2).
- ‹ › in the main window's toolbar, ⌘[ ⌘], and ⌘← ⌘→ outside a text field go back and forward between the places you visited (US-23.1).
- The context of a closed or merged pull request or merge request is no longer checked by itself (D197), and Refresh Items in a Topic shows that it is working.
