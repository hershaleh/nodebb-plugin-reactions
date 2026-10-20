# How to send these changes to the original author (when ready)

1. On https://github.com/ClickAndGoScript/nodebb-plugin-reactions click **Fork** > **Create fork** (not on your own repo).
2. Ask Claude to push `upstream.patch` to a new branch of your fork, or do it yourself:

       git clone https://github.com/<you>/<fork-name>
       cd <fork-name>
       git checkout -b my-improvements
       git apply /path/to/upstream.patch
       git add -A && git commit -m "Self-reaction block, touch popup, merged notifications, ..."
       git push origin my-improvements

3. Open your fork on GitHub, click **Contribute** > **Open pull request**, paste `PR-description.md` and send.

`upstream.patch` applies to the original's master (commit ba30d8b, "fix: block reactions on deleted posts").
