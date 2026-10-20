# Title
Self-reaction block, touch long-press popup, per-emoji merged notifications, notification cleanup, responsive layout

# Description
Hi, thanks for the plugin! I use it on my forum and added a few things. All new settings are optional and the defaults keep the existing behaviour, except the first item (see below).

- **Block self-reactions** (ACP switch "Allow users to react to their own posts", off by default). The add-button is hidden on the author's own posts, the server rejects it, and it never gives reputation.
- **Touch devices:** long-press on a reaction opens a popup listing who reacted (same look as the desktop tooltip). It stays open until you tap elsewhere, so it survives the browser's "image options" dialog.
- **Full reactors list** (right-click / "Show everyone").
- **Notifications:** same-emoji reactions on one post/message are merged into one notification (different emojis stay separate); the emoji is rendered as an image instead of `:name:` text.
- **Cleanup:** removing a reaction deletes the author's notification (ACP switch, on by default); removing a built-in upvote deletes its notification (switch on the core Reputation & Flags page, on by default).
- **Layout:** the reactions row wraps and never makes the page wider than the screen.
- Hebrew translation of the ACP.

Tested with unit tests against mocked NodeBB modules and in a browser for the layout and touch events. I'm happy to split this into smaller PRs if you prefer.
