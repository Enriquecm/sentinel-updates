# Sentinel 0.5.0

Released on 06/11/2026.

Sentinel now gathers the context around a pull request or merge request, groups related work into Topics, and has a new Settings window.

## New

- **Context.** A pull request's Context tab gathers what relates to it from Slack, Jira, Bitrise, Confluence and your Claude Code sessions into a summary that links every source. Sentinel reads them through your own Claude Code's MCP servers, read-only. Turn it on in Settings → Context; Sentinel keeps it current and shows what changed since you last looked.
- **Topics.** Group pull requests, merge requests and links about one subject. Sentinel suggests a Topic when items share a ticket, a thread or a build. Add an item with ⌥⌘T, and follow a Topic to hear when it changes.
- **AI spending.** Settings → AI → Usage and budget shows what AI runs cost by day, module and model. Set a daily or monthly budget: Sentinel warns at 80% and pauses automatic runs when you reach it. The runs you start yourself keep working.
- **Follow any repository.** Paste the URL of a repository you are not a member of, such as a public project, in Add Repository. Sentinel never publishes there by itself.
- **Undo and Redo** (⌘Z, ⇧⌘Z) for your actions in Sentinel, such as Start Review, Mark Done or accepting a finding. Comments on GitHub or GitLab are not undone.
- **Back and forward** between the places you visited, with ⌘[ and ⌘] or the arrows in the toolbar.

## Improved

- Settings is rebuilt like System Settings, with search and a page for each account, repository and source.
- Search finds a pull request or merge request by its number: 57, !57 or #57.
- The repository bar shows when its list was last updated.
- Sentinel no longer checks the context of closed or merged items.
