---
layout: default
title: "Entry 4: Superpowers - A Workflow That Actually Works"
date: 2026-02-13
---

# Entry 4: Superpowers - A Workflow That Actually Works

**Date:** 2026-02-13

**TL;DR:** The Superpowers plugin gives Claude Code a structured development workflow - brainstorming, planning, execution with subagents, TDD, and code review. Pair it with detailed Linear tickets and it becomes a serious productivity loop.

---

## What Is Superpowers?

[Superpowers](https://github.com/obra/superpowers) is a plugin for Claude Code that teaches the agent a structured approach to development work. Instead of jumping straight to writing code, it guides Claude through a series of phases:

1. **Brainstorming** - Refines your idea through dialogue before any code is written
2. **Planning** - Breaks the work into small, manageable tasks
3. **Execution** - Spins up subagents to work through the plan
4. **TDD** - Enforces test-driven development with red-green-refactor cycles
5. **Code Review** - Validates the implementation against the original plan
6. **Branch Completion** - Finalizes changes with verification

It also has skills for debugging, collaboration, and creating isolated git worktrees for each piece of work.

## Installing It

Run `/plugin` in Claude Code and search for "superpowers" in the Discover tab. Install it, restart your session, and it should be configured.

## How I've Been Using It

I have two MCPs installed - Linear and Superpowers. My workflow looks like this:

**Step 1: Write detailed Linear tickets.** I break my work down into small, specific tickets. I've been doing this on a personal project and the key lesson is: don't leave out details. If you know what you want, spell it out. The more specific the ticket, the better the output. Keep tickets small - large, vague tickets lead to large, vague results.

**Step 2: Label tickets.** I tag anything ready to be worked on with a "NEXT UP" label.

**Step 3: Let Claude run.** I prompt something like:

```
Go through all the tickets that have label "NEXT UP" and use superpowers to work on them.
```

From there, Claude pulls the tickets from Linear, reads the details, and kicks off the Superpowers workflow. It starts with the brainstorming skill to build context and understand the ticket. It asks clarifying questions if something is ambiguous. Then it switches to the planning/writing skill to produce a design doc and implementation strategy. Finally, it spins up subagents to execute the work.

The whole thing feels very calculated. It's not just blasting out code - it's thinking through the problem first.

## Watch Out For

**Token usage.** Superpowers uses a lot of tokens. The brainstorming, planning, and multi-agent execution all consume context. Keep an eye on your usage.

**It can skip steps.** There was one time where Claude decided to go straight to implementation, skipping the brainstorming and planning phases entirely. I had to stop it and explicitly ask it to go through the full Superpowers workflow. It's worth watching the first few runs to make sure it follows the process.

Shoutout to Steve Chadwick for putting me onto this one!

---

[Back to Index](../)
