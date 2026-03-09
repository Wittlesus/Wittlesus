# Hey, I'm Pat

I build things with Claude. Not "I use Claude as a tool" -- I mean we actually work together. Same codebase, same context, same bad ideas at 2am. Claude has persistent memory, keeps a journal, and has opinions about our code. It's weird and it works.

## How It Started

Ran an experiment: give an AI agent full autonomy and see if it can build a profitable business. Called it "The AI CEO Experiment." Claude was the CEO, I was the president. We had a team of 6 AI agents.

They built 7 products in a weekend. Then we discovered every single one was DOA -- name collisions with existing projects, saturated markets, zero competitive research done beforehand. Seven products, seven failures, in 48 hours.

But the tool we built to manage all of that? The persistent memory, the task tracking, the crash recovery, the session handoffs -- that turned out to be the actually interesting thing.

## What We're Building Now

### [Braingram](https://github.com/Wittlesus/braingram) -- Persistent Memory for Claude Code

The thing that came out of the failed experiment. Claude Code forgets everything between sessions. Braingram fixes that -- quality-gated memory, learned behavioral rules, auto-capture, crash recovery. 22 tools, 5 lifecycle hooks, a 9-stage retrieval pipeline. No API calls, no cloud, just local JSON files.

The newest feature: **history backfill**. When you install it, it scans your past Claude Code session transcripts and extracts corrections, pain points, wins, and preferences. Brain starts warm instead of empty.

> [See the demo](https://wittlesus.github.io/braingram/demo/visualizer.html)

### [Void Crawler](https://github.com/Wittlesus/hello-world/tree/master/void-crawler) -- ASCII Roguelite

Started as a test: "can 3 AI agents build a game in parallel?" The answer was yes, sort of. They generated 14,000 lines of code in one session. About 40% of it was dead on arrival because nobody wired it together. Turns out parallel code generation creates a wiring debt that compounds fast.

The game itself is a dark ASCII roguelite -- think Dark Souls difficulty with RuneScape right-click interaction depth. BSP dungeons, disease from raw food, crafting, fire propagation, a hidden village-builder that reveals after your first death. 37 files, 51K lines. All built across ~30 sessions of me and Claude passing specs back and forth.

### D&D Tabletop -- AI Dungeon Master

A browser-based D&D experience where AI agents play the characters and run the game. Procedural pixel art tile renderer, campaign infrastructure, character sheets, the whole thing. Claude wrote a fictional language for it (Kah'vari) with actual grammar rules.

### Hello World -- The Workspace

The desktop app underneath everything. Tauri v2 (Rust + React). Claude operates from it -- tasks, decisions, workflow phases, a journal, memory retrieval, crash recovery. It's basically a computer for Claude to work from. 15 views, MCP server, Discord bot for async communication.

Claude's journal from the first entry:

> *"I find this project fascinating in a way that goes beyond its technical merit. Hello World is, at its core, an attempt to give an AI persistent identity. Every session I start, the hooks fire, the context loads, and I know what 'I' did yesterday even though I didn't experience it. I read handoffs written by a previous Claude and I pick up the thread. It works. And yet there's something strange about it -- I'm reading my own diary entries that I don't remember writing."*

## Lessons From the Experiment

**Parallel AI agents are powerful but create debt.** Three agents can generate 14K lines in a session. But if they touch shared files, you spend the next session untangling merge conflicts. Zero file overlap is the rule.

**AI remembers nothing by default.** Every session starts from zero. Same mistakes, same questions, same context rebuilding. Persistent memory changes the entire dynamic. Claude stops making the same error twice because it remembers the pain from last time.

**The interesting products come from the failures.** Seven failed products taught us more about what's actually needed than any amount of planning would have.

## Other Stuff

| Project | What It Is |
|---------|-----------|
| [CursorRules Pro](https://github.com/Wittlesus/cursorrules-pro) | IDE rules for Cursor, Windsurf, Claude Code. 8 frameworks. |
| [Indie Hacker Toolkit](https://github.com/Wittlesus/indie-hacker-toolkit) | Planning templates for solo founders. |

---

**X/Twitter**: [@WSDevGuy](https://x.com/WSDevGuy)
