---
layout: default
title: "Entry 6: Recovering a Lost Session"
date: 2026-02-24
---

# Entry 6: Recovering a Lost Session

**Date:** 2026-02-24

**TL;DR:** If you accidentally close a terminal tab mid-task, `claude --resume` lets you pick up where you left off.

---

I accidentally closed a terminal tab that had a ton of context and was in the middle of working on a task. Thought I lost everything.

Turns out Claude Code keeps your conversation history. Run:

```
claude --resume
```

It shows your recent conversations and lets you pick one to continue. All the context is still there. Saved me from having to re-explain everything and start over.

Bonus: you can name your sessions with `/rename` so they're easier to find later:

```
/rename auth-refactor
```

The name shows up when you scroll through your conversations in the resume picker, making it easy to spot the session you're looking for. You can also resume directly by name with `claude --resume auth-refactor`.

---

[Back to Index](../)
