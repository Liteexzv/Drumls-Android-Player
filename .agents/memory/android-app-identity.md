---
name: Android app identity
description: Compatibility rule for display-name changes in the Android player.
---

For a display-name-only rename from Wave to Drumls, keep the Android application ID and browser storage keys unchanged. Update only user-facing labels and build artifact names.

**Why:** Changing the application ID can prevent an installed app from receiving updates, and changing storage keys can make existing playlists and settings appear lost.

**How to apply:** Preserve `com.liteex.wave`, `wave`, and `wave4` for compatibility unless the user explicitly requests a new app identity or a storage migration.
