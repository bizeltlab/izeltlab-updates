# Ízeltláb updates

Update source for the izeltlab.hu shop: the Ízeltláb theme, the Codex plugin and the Ízeltláb Bolt plugin.
WordPress reads `updates.json` (Settings → Ízeltláb updates) and offers `update/` as an update; `backup/` holds the
version that was live before it (Roll back button).

Each deploy: the old backup is deleted, the previous update becomes the backup, the new build becomes the update.

Each zip in `updates.json` has a `sha256` fingerprint. From theme 2.11.0, Codex 1.71.0 and Bolt 1.7.0 on, the shop refuses a zip whose fingerprint is missing or does not match.
