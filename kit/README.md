# The Genesis kit

Ten rules and two templates for writing a long piece of work with AI agents across
many sessions. Each rule carries its reason, so an agent can judge it as well as follow it.

**Status:** 1.0.0, a first release. Its first outside test, on a small local model, is
under way.

## What is here

| file | use |
| :--- | :--- |
| [`genesis-core.md`](genesis-core.md) | the ten rules, one page; paste it wherever your AI takes standing instructions |
| [`AGENTS.md`](AGENTS.md) | the same rules as a section for agents that read rules files |
| [`skills/genesis/SKILL.md`](skills/genesis/SKILL.md) | the same rules as a skill, with steps for starting and finishing |
| [`templates/awakening.md`](templates/awakening.md) | the entry file every agent reads first |
| [`templates/capture-template.md`](templates/capture-template.md) | what a session leaves behind for the next one |

## Three layers

1. **The rules alone.** Put `genesis-core.md` in your AI's standing instructions.
   That is enough to change how a session works.
2. **The rules and two files.** Add an awakening file and keep captures. Each new
   session then starts from the same ground, and what one session learns reaches the next.
3. **The full framework.** Modes, stances and reader audits for a long project, in
   [`framework/`](../framework/), once published.

## Setting it up

Make a `genesis/` folder in your project with three things in it:

```
genesis/
  awakening.md          from templates/awakening.md, filled in
  capture-template.md   from templates/capture-template.md
  captures/             one file per session
```

Then give your AI the rules:

| where you work | what to do |
| :--- | :--- |
| ChatGPT (custom GPT or Project) | paste `genesis-core.md` into the instructions; upload `awakening.md` and the capture template as files |
| Claude (Project) | paste `genesis-core.md` into the project instructions; add `awakening.md` and the capture template to the project files |
| Gemini (Gem) | paste `genesis-core.md` into the Gem's instructions; attach `awakening.md` and the capture template |
| a coding agent that reads `AGENTS.md` | copy the section in `kit/AGENTS.md` into your project's `AGENTS.md`; it sits between its own markers alongside anything else there |
| a coding agent that reads `CLAUDE.md` | copy the section into `CLAUDE.md`, or point `CLAUDE.md` at your `AGENTS.md` |
| a coding agent that loads skills | copy `kit/skills/genesis/` into the agent's skills folder |
| a local model in a chat front end | paste `genesis-core.md` into the system prompt; paste the awakening at the start of each session |

In a session limited to chat, the agent gives its capture in its final reply.
You save it to `genesis/captures/` and paste the latest one into the next session.
Carrying it by hand has a benefit of its own: you read every capture before it travels on.

## Making it yours

Keep the ten rules as they are, and put everything particular to your project in the
awakening file: who decides, your house style, the words that mean something special
in your work. Then the rules stay the same across projects, and the awakening carries
what is different.

## Licence

The rules and templates are MIT licensed; see [`LICENSE.txt`](../LICENSE.txt).
