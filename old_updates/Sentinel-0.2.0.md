# Sentinel 0.2.0

Released on 08/10/2026.

Faster daily reviews: quick actions in the menu bar and in notifications, AI reviews of only what changed, and the provider's status at a glance.

## New

- **Review only what changed.** After new commits, Review Changes asks the AI to review just the commits since its last review.
- **Menu bar.** The Review Queue by state, with Start Review, Run AI Review, Mark Done and more on each item, and a sparkle while an AI review runs.
- **Notifications.** Open, Start Review, Run AI Review or Mark as Read from the banner. Updates on one item are grouped instead of piling up, and you can mute notifications for an hour, until tomorrow or until you turn them back on.
- **Provider status** in lists and headers: CI, the review decision, merge conflicts and unresolved threads, each with a filter.
- **Reply to and resolve** a published finding's thread on GitHub or GitLab, with Draft with AI to write the reply.
- **Ask the AI** about a whole review session, Explain a single finding, or Compare two sessions.
- **Activity Log** filters, search, and grouping by day or by item.

## Improved

- Review Rules show how many open items they match while you edit, and ask before discarding unsaved changes.
- Lists say how many new commits arrived since you last looked.
- Published findings follow their code when lines move or the branch is rebased.

## Fixed

- Removing a criterion from a rule crashed Sentinel.
- With the inspector open in a small window, the item header was cut off and its buttons did not respond.
