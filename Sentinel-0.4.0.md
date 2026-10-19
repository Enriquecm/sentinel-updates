# Sentinel 0.4.0

Released on 19/10/2026 (build 227).

The right bar beside the detail, over it or in a window of its own, and the conversations with the AI rebuilt around one chat per item, with a terminal in the item's window: work packages 2.34 to 2.47 of Phase 2 (D101–D110).

- The right bar can sit beside the detail or over it. Switch with the control in its header or View › Right Bar › Beside / Over (⌃⌥⌘0); the choice is remembered, and switching keeps the tab, the scroll position and what you were typing. Over leaves the columns as they are and closes with Escape (US-4.22).
- Open in New Window gives an item a window of its own, one per item, from the bar's header, the row's context menu, a double-click on a row, the detail header's ⋯ menu or Item › Open in New Window (⌘O). It has Details, Chat, Sessions and Terminal, keeps its size and position, and comes back at the next launch (US-4.23, US-4.25).
- An item open in the main window and in its own window is the same in both: a message sent or a session cancelled in one shows in the other at once (US-4.24).
- ⌘R refreshes the item in front, ⇧⌘R refreshes everything, and ⌥⌘1 to ⌥⌘4 pick the bar's tabs (US-4.25).
- One chat per item: the conversation about the whole pull request or merge request, each session's and each finding's read as one list, each run of messages tagged with its scope. Type @ to ask about a session or a finding; the filter shows one scope at a time (US-9.14).
- Replies appear as they are written, after the files the AI opens; Stop (⌘.) keeps what arrived (US-9.15).
- Copy a message as Markdown or plain text, a code block on its own, or a path; Quote the message or the part you selected; ⇧⌘C copies the last answer; Export… saves the conversation, or the scope you filtered, as Markdown (US-9.16).
- Use an answer as a new draft, a revision of a finding, a reply on a thread, the body of an approval or a request for changes, or the focus of the next review. Findings and revisions the AI proposes arrive as cards you add, edit or discard; nothing joins Review until you add it (US-9.17, US-9.18).
- Revise a draft or a comment Sentinel published from a conversation: the card shows the change word by word, and a published comment changes on GitHub or GitLab only after Update Comment (US-9.18).
- Drafts from a conversation are marked Proposed in Chat in Review, with Show in Chat, and appear at the time you added them. Drafts about the whole pull request or merge request are kept in a Chat session (D105, D110).
- Sessions shows the runs: Ask in Chat, Open Terminal, Compare…, and Open in your terminal app (US-4.21).
- A Terminal tab in the item's window runs Claude Code, or a command you choose, in Sentinel's copy of the item, never in your clone; it continues the chat or a session. Sentinel offers the agent its tools, which can only propose findings and revisions for you to add (US-8.12, US-8.13).
- Settings → AI Backend → Terminal: the app sessions open in outside Sentinel (Terminal, iTerm or another), and the custom command for the Terminal tab (US-8.14).
