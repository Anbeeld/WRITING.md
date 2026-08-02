# Anbeeld's WRITING.md — AI Writing Rules

A prose ruleset that makes AI-assisted text sharper, not as generic, and less like default model output. It targets the patterns that make generated prose feel recognizable without breaking grammar, faking typos, or gutting useful structure. The result reads better than unguided output and avoids the most common tells.

The rules combine writing standards, web readability research, documentation guidance, detector-limit research, and direct observation of what LLMs produce when left to defaults.

[![Support my work!](https://anbeeld.com/images/support.jpg)](https://anbeeld.com/support)

## What it does

- Starts with context: medium, audience, reader need, and the job of the text.
- Calibrates voice to genre. Opinion pieces can sound like a person; summaries and docs stay neutral.
- Calibrates a personal or brand voice only when explicitly requested, without importing biography or caricaturing surface quirks.
- Keeps the format appropriate. Docs stay scannable; casual replies do not get over-structured. Does not remove useful structure just to look less templated.
- Replaces polished generality with concrete anchors. If a paragraph has no checkable detail, it gets revised.
- Guards against fake specificity. Quotes, numbers, dates, causal claims, and named claims need support.
- Preserves meaning during edits: scope, uncertainty, attribution, conditions, exact terms, links, and redactions do not drift just because a sentence gets smoother.
- Breaks the patterns that make model prose look templated: repeated cadence, hidden lists, generic signposts, and too-neat paragraph shapes.
- Prefers ordinary words over inflated phrasing. Allows repetition when the ordinary word is the right one.
- Cuts the staged parts: keynote cadence, service-desk tone, ceremonial openings, and filler closings.
- Does not fake humanity with some specific tricks. No invented typos, no forced slang, no programmatic sentence-length variation, no staged messiness. You can add it yourself, if needed.
- Revises by reading and cutting. Collapses restatements, drops announcement sentences, and replaces the most generic clause with something specific.

## How to use it

### 1. Manually as direct instructions

Give [the ruleset](WRITING.md) to an AI and tell it to apply the rules with their stated precedence and medium routing. The high-density instructions (~5400 words) counter regular sentence structure, generic phrasing, parallel enumeration, overly neat conclusions, meaning drift during editing, and other model defaults.

One pattern that works well: ask for a first draft with the rules applied, then request an audit of that draft against the required checks, and have the model rewrite based on what the audit caught. Repeat one or two more times if the text is on a larger side. Further rewrites after that usually circulate around the same model-level limitations.

This is meant for legitimate uses, like iterating on a human draft or turning loosely organized thinking into something you would actually publish. The output avoids the most common LLM tells and will read better than unguided model text, but it will not pass an experienced eye test or an advanced detector. Prompt-level instructions have a ceiling and can't overcome model-level defaults.

### 2. As a skill in an agent harness

Use the packaged skill in [/skills/writing](skills/writing) with tools that support skills: Claude Code, Codex, OpenCode, Cursor, and others. The skill loads on demand when the agent is doing writing, so it costs almost no context until needed.

**Installation:** copy the [/skills/writing](skills/writing) directory to your global skills folder:

- **Claude Code:** `~/.claude/skills/`
- **Codex:** `~/.codex/skills/`
- **Cursor:** `~/.cursor/skills/`
- **OpenCode:** `~/.config/opencode/skills/`

The skill description is scoped to reader-facing prose, including articles, blogs, documentation, criticism, long-form, email, marketing and SEO copy, summaries, scripts, applications, and UI text. It explicitly excludes code comments, commit messages, and private notes.

### 3. Compact as agent/chat instructions

[WRITING-compact.md](WRITING-compact.md) is the same rules at ~1500 words. Use as AGENTS.md or CLAUDE.md for writing agents, or as instructions in custom chats like GPTs and Gemini Gems. It keeps the core behavior, required checks, and a compressed watchlist while omitting full examples and diagnostics.

### 4. Mini as a section in AGENTS.md

[WRITING-mini.md](WRITING-mini.md) is ~330 words and fits on one screen. The highest-impact behavior is compressed into eight imperative bullets. It is designed for a persistent section in global AGENTS.md or CLAUDE.md, where the rules stay present without dominating context.

## See also

- [Anbeeld's Global AGENTS.md / CLAUDE.md](https://github.com/Anbeeld/AGENTS.md)
- [Anbeeld's RESUME.md: AI Resume/CV Rules](https://github.com/Anbeeld/RESUME.md)
- [Anbeeld's PROMPTING.md: AI Instruction Designer](https://github.com/Anbeeld/PROMPTING.md)

[![Support my work!](https://anbeeld.com/images/support.jpg)](https://anbeeld.com/support)
