---
layout: default
title: "Entry 7: Better Notifications with /hooks"
date: 2026-02-24
---

# Entry 7: Better Notifications with /hooks

**Date:** 2026-02-24

**TL;DR:** The `/hooks` command is an easier way to set up hooks than editing JSON files, and I added a second notification for when Claude is waiting on me for permission.

---

In [Entry 5](entry-005) I set up a notification sound for when Claude finishes executing by manually editing `.claude/settings.local.json`. It works, but I've since learned there's an easier way - the `/hooks` command.

Beyond that, I realized the Stop notification wasn't enough. If Claude is asking for permission to run a command or wants my input on an approach, it just sits there waiting silently. I'd tab away and not realize it was blocked on me.

So I ran `/hooks`, selected `PermissionRequest`, and for the command I used the same pattern as before but with a different sound so I can tell them apart:

```
afplay /System/Library/Sounds/Frog.aiff
```

Now I get a glass sound when Claude is done, and a frog sound when it needs my attention.

---

[Back to Index](../)
