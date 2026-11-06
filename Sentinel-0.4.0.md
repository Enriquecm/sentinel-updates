# Sentinel 0.4.0

Released on 19/10/2026.

One chat per pull request or merge request, a window of its own for each item, and a terminal that runs Claude Code on Sentinel's copy of the code.

## New

- **Open in New Window** (⌘O) gives an item a window of its own, with Details, Chat, Sessions and Terminal. It comes back at the next launch.
- **One chat per item** about the whole pull request or merge request, its sessions and its findings. Type @ to ask about a session or a finding. Replies appear as they are written, and Stop (⌘.) keeps what arrived.
- **Turn answers into work**: a new draft, a revised finding, a reply on a thread or the text of an approval. What the AI proposes arrives as a card you add, edit or discard, and a published comment changes only after Update Comment.
- **Terminal tab** that runs Claude Code, or a command you choose, on Sentinel's copy of the item, never in your clone.
- **Right bar beside or over the detail** (⌃⌥⌘0).

## Improved

- Copy a message as Markdown or plain text, quote it, or export the conversation. ⇧⌘C copies the last answer.
- ⌘R refreshes the item in front, ⇧⌘R refreshes everything, and ⌥⌘1 to ⌥⌘4 pick the right bar's tabs.
- Settings → AI Backend → Terminal chooses the terminal app sessions open in.
