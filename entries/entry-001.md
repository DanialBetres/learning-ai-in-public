---
layout: default
title: "Entry 1: Setting Up Claude Code"
date: 2026-02-06
---

# Entry 1: Setting Up Claude Code

**Date:** 2026-02-06
**TL;DR:** I installed Claude Code in a new terminal, ran my first session, and learned what a CLAUDE.md file is for.

---

## Wait, How Do I Even Use This Thing?

Before writing a single line of code, I got stuck on something embarrassingly basic: how am I supposed to interface with Claude Code?

In the terminal? If so, which terminal? Within an IDE? A standalone app? Do people have the IDE and the terminal side by side? Separate windows? Should I be using the VS Code extension instead? The web browser version? The macOS desktop app? There are a lot of options and I had no idea which one was "right."

I didn't figure out the best answer yet - and honestly I'm not sure there is one single best answer. But I had to start somewhere, so I decided to go with the terminal.

## Picking a Terminal

I had been using Kitty as my terminal and wasn't loving it. Around the same time, I saw that the creator of Claude Code mentioned his team loved using the [Ghostty](https://ghostty.org/) terminal. That was enough for me - I downloaded it and decided to start fresh there.

## Installing Claude Code

Once I had Ghostty set up, I followed the [official install instructions](https://code.claude.com/docs/en/overview#native-install-recommended). It's a one-liner:

```bash
curl -fsSL https://claude.ai/install.sh | bash
```

After that, I went into the project I was working on and ran:

```bash
cd my-project
claude
```

That dropped me right into the Claude Code agent. Cool! Now what?

## The First Thing To Do: /init

The docs recommend running `/init` as your first step. What this does is analyze your codebase and generate a `CLAUDE.md` file for you.

So what's a CLAUDE.md file? It's a special file that Claude reads at the start of every conversation. Think of it as persistent instructions - things like your code style preferences, how to run tests, workflow rules, or anything else Claude can't figure out just by reading your code. The [docs go into more detail](https://code.claude.com/docs/en/best-practices#write-an-effective-claude-md) on what to include and what to leave out.

The key insight: CLAUDE.md is how you give Claude context it can't infer on its own. You don't need to write a novel - just the stuff that matters. If Claude already does something correctly without being told, you don't need a rule for it.

After running `/init`, I had a basic CLAUDE.md file and the agent had a better understanding of my codebase.

## Asking It Questions

I decided to start simple - just asked a few questions about the codebase. Things like how certain parts of the code worked, what certain files were responsible for, that kind of thing. I was pleasantly surprised with the answers. They were thoughtful and actually accurate.

If you're just getting started, I'd recommend doing the same thing. Don't try to build something right away. Just ask questions about your codebase and see how it responds. Get a feel for it.

## What About IDE Integration and Everything Else?

I haven't experimented with the VS Code extension, the desktop app, the web version, or any of the other ways to use Claude Code. For now, I'm sticking to the terminal until I run into a scenario where I'd need something different.

I'm trying not to overdo things or do everything at once. Taking it step by step.

---

[Follow me on LinkedIn](https://www.linkedin.com/in/danbet/) | [Back to Index](../)
