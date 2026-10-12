# genesis-framework-late

The Genesis Framework for the **late stage**: consolidating a long manuscript that is close to
complete, with fresh AI agents joining session after session. Copy this one folder into your own
setup; everything in it is a working file.

Written with, and tuned to, Claude Opus 5.5. The full framework is at 9.3.3, and the portable
rules follow its version numbers. Its first outside test, on a small local model, is under way.

## What is here

| file | use |
| :--- | :--- |
| [`genesisCore.md`](genesisCore.md) | the ten rules on one page; paste it wherever your AI takes standing instructions |
| [`AGENTS.md`](AGENTS.md) | the same rules as a section for agents that read rules files |
| [`skills/genesis/SKILL.md`](skills/genesis/SKILL.md) | the same rules as a skill, with steps for starting and finishing |
| [`GENESIS-FRAMEWORK-LATE.md`](GENESIS-FRAMEWORK-LATE.md) | the full framework: every rule with its reason, eight modes, two stances, the capture system |
| [`templates/awakening.md`](templates/awakening.md) | the entry file every agent reads first |
| [`templates/voice0.md`](templates/voice0.md) | how to read the author's messages, read beside the awakening on waking |
| [`templates/voice.md`](templates/voice.md) | a model of the author's voice, for agents drafting in the author's name |
| [`templates/readerWelcome.md`](templates/readerWelcome.md) | the message that wakes a fresh reader, and why each phrase is there |
| [`templates/captureTemplate.md`](templates/captureTemplate.md) | what a session leaves behind for the next one |
| [`templates/closingPrompt.md`](templates/closingPrompt.md) | the questions every session answers before it ends |
| [`readerAudits.md`](readerAudits.md) | how to run fresh readers against your material or your onboarding, and fold their stumbles back |

Each template names its worked example in the [case study](../case-study/).

## Three layers

1. **The rules alone.** Put `genesisCore.md` in your AI's standing instructions. That is enough to
   change how a session works.
2. **The rules and two files.** Add an awakening file and keep captures. Each new session then
   starts from the same ground, and what one session learns reaches the next.
3. **The full framework.** Modes, stances and reader audits for a long project:
   `GENESIS-FRAMEWORK-LATE.md`, with the voice templates and the welcome.

## Setting it up

Make a `genesis/` folder in your project with three things in it:

```
genesis/
  awakening.md          from templates/awakening.md, filled in
  captureTemplate.md    from templates/captureTemplate.md
  captures/             one file per session
```

Then give your AI the rules:

| where you work | what to do |
| :--- | :--- |
| ChatGPT (custom GPT or Project) | paste `genesisCore.md` into the instructions; upload `awakening.md` and the capture template as files |
| Claude (Project) | paste `genesisCore.md` into the project instructions; add `awakening.md` and the capture template to the project files |
| Gemini (Gem) | paste `genesisCore.md` into the Gem's instructions; attach `awakening.md` and the capture template |
| a coding agent that reads `AGENTS.md` | copy the section in `AGENTS.md` into your project's `AGENTS.md`; it sits between its own markers alongside anything else there |
| a coding agent that reads `CLAUDE.md` | copy the section into `CLAUDE.md`, or point `CLAUDE.md` at your `AGENTS.md` |
| a coding agent that loads skills | copy `skills/genesis/` into the agent's skills folder |
| a local model in a chat front end | paste `genesisCore.md` into the system prompt; paste the awakening at the start of each session |

In a session limited to chat, the agent gives its capture in its final reply. You save it to
`genesis/captures/` and paste the latest one into the next session. Carrying it by hand has a
benefit of its own: you read every capture before it travels on.

## Making it yours

Keep the ten rules as they are, and put everything particular to your project in the awakening
file: who decides, your house style, the words that mean something special in your work. Then the
rules stay the same across projects, and the awakening carries what is different.

## Versions

`GENESIS-FRAMEWORK-LATE.md` holds 9.0.0 to 9.3.3 in its history, tagged `framework-late-<version>`.
The paper's [§8](../paper/GENESIS-PAPER.md) tells what each fresh reader found and which version it
produced.

| version | what it brought |
| :--- | :--- |
| 9.0.0 | the first late-stage framework: a small core of rules each with its reason, modes chosen by the session's goal, red and blue stances |
| 9.1.0 | a new first rule, *sessions are free; the record answers to evidence*, and corrections found in an earlier agent's review |
| 9.2.0 | the author's handle, the voice document as a companion, and consensus before any change to the manuscript |
| 9.3.0 | from reader 1: the airlock built from separate files, since a file is read whole; identification by generation and reader |
| 9.3.1 | from reader 2: the document listing varies by surface, and every reader reports what arrived |
| 9.3.2 | from reader 3, the baseline: a clearer capture rule, the exact identification format, the onboarding audit's scope, and the prior capture |
| 9.3.3 | from reader 4: identification after the reading and in the final message, and the airlock rules placed first |

`GENESIS-FRAMEWORK-LATE.md` was written for the case study and names its files and paths; the
portable rules and templates carry the same design without them. Passages marked `[redacted]`
remove the author's name, references to a retired framework, and personal detail.

## Licence

The rules (`genesisCore.md`, `AGENTS.md`, `skills/genesis/SKILL.md`), the full framework and
`readerAudits.md` are method, under CC BY 4.0; see [`LICENSE-CC-BY-4.0.txt`](../LICENSE-CC-BY-4.0.txt).
The templates are under MIT; see [`LICENSE.txt`](../LICENSE.txt).
