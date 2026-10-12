# Installing the late line

Every environment needs the same four things, in the same order:

1. **Standing instructions:** the rules, loaded by the environment into every session.
2. **Entry files:** your filled-in `awakening.md` and `voice0.md`, read by the agent first.
3. **The first message:** your welcome, with the session's goal.
4. **The close:** the closing prompt, and a capture you save for the next session.

Prepare the files once, then follow the section for your environment.

## Prepare your files

```
genesis/
  awakening.md          from templates/awakening.md, filled in
  voice0.md             from templates/voice0.md, filled in (optional, recommended)
  captureTemplate.md    from templates/captureTemplate.md
  captures/             one file per session, saved by you or written by the agent
```

Keep `templates/readerWelcome.md` and `templates/closingPrompt.md` at hand for steps 3 and 4.

**Which rules file:** `genesisCore.md` is one page and fits every environment.
`GENESIS-FRAMEWORK-LATE.md` is the full framework, about 8,000 words; add it as a file where your
environment holds files and has room for it, so the agent can open it when a mode calls for it.

---

## Claude, in a Project

The closest fit: the case study runs this way.

1. **Project instructions:** paste `genesisCore.md`. Then add one line naming the entry files, for
   example: *On waking, read `awakening.md` and `voice0.md` before anything else.*
2. **Project knowledge:** upload `awakening.md`, `voice0.md`, `captureTemplate.md`, and optionally
   `GENESIS-FRAMEWORK-LATE.md`.
3. **Each session:** start a new chat in the project and send your welcome.
4. **At the end:** send the closing prompt. Save the capture the agent gives you, and upload it to
   the project knowledge so the next session can read it.

## Claude, standalone chat

A single chat outside any project: everything travels in the first message.

1. **First message:** attach `genesisCore.md`, `awakening.md` and `voice0.md`, and write: *Read the
   attached rules and both entry files before anything else.* Then paste your welcome below it.
2. **During the session:** attach any further file by hand when a mode calls for it.
3. **At the end:** send the closing prompt and save the capture. Attach the latest capture to the
   first message of your next chat.

## Claude, other ways in

Claude runs in several places, and each takes the four steps in its own way.

| where | standing instructions | entry files | notes |
| :--- | :--- | :--- | :--- |
| Claude Code, in a terminal, the desktop app or the web | the `AGENTS.md` section or `CLAUDE.md` in the repository, or the skill | `genesis/` in the repository | see *Coding agents* below; Claude Code reads `CLAUDE.md` and skills by itself |
| the Claude API | `genesisCore.md` as the system prompt | the awakening and voice0 in the first user message | your own code saves each capture from the final reply |
| claude.ai personal preferences | your house style, which then applies to every chat | | keep the ten rules in the project or the first message, so they apply to this work alone |

## Gemini

**In a Gem**, the reusable form:

1. **Gem instructions:** paste `genesisCore.md`, with the line naming the entry files.
2. **Gem knowledge:** add `awakening.md`, `voice0.md`, `captureTemplate.md`, and optionally
   `GENESIS-FRAMEWORK-LATE.md`.
3. **Each session:** open a new chat with the Gem and send your welcome.
4. **At the end:** send the closing prompt, save the capture, and add the latest capture to the
   Gem's knowledge.

**In a standalone chat**, follow *Claude, standalone chat* above: the same files in the first
message.

## Small local models, for example on Strata

[Strata](https://stratallm.org/) is an open-source engine for running language models on your own
hardware, such as a heavily quantised Qwen3.8-Flash-Next. A model that small has a short attention
span and little room, so keep the load small.

1. **System prompt:** paste `genesisCore.md` only.
2. **First message:** paste a short `awakening.md` (a page at most), then your welcome. Leave
   `voice0.md` and the full framework out until the model shows it holds the rules.
3. **If it runs inside a coding agent** that reads rules files, use the *Coding agents* section
   instead; the agent then loads the rules and reads the entry file by itself.
4. **At the end:** send the closing prompt and save the capture yourself.
5. **Record the result:** the model, its quantisation and its settings, with what held and what
   slipped. A rule set that holds on the smallest model it meets will hold anywhere.

## Coding agents

For agents that work in a repository (Claude Code, Codex, OpenCode and others):

1. **Rules:** copy the section in `AGENTS.md` into your repository's `AGENTS.md`; it sits between its
   own markers alongside anything else there. For an agent that reads `CLAUDE.md`, copy the section
   there, or point `CLAUDE.md` at `AGENTS.md`. For an agent that loads skills, copy
   `skills/genesis/` into its skills folder.
2. **Entry files:** put your `genesis/` folder at the repository root.
3. **Each session:** give the goal as your first message. The agent reads `genesis/awakening.md`
   and writes its capture to `genesis/captures/` by itself.

This repository runs this way: see its own [`AGENTS.md`](../AGENTS.md) and [`genesis/`](../genesis/).

## Other chat assistants

Any assistant with a place for standing instructions works like *Gemini, in a Gem*: rules in the
instructions, entry files as attached knowledge. Any assistant without one works like *Claude,
standalone chat*.
