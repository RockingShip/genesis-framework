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
| [`INSTALL.md`](INSTALL.md) | how to install it in each environment |
| [`readerAudits.md`](readerAudits.md) | how to run fresh readers against your material or your onboarding, and fold their stumbles back |

Each template names its worked example in the [case study](../case-study/).

## Three layers

1. **The rules alone.** Put `genesisCore.md` in your AI's standing instructions. That is enough to
   change how a session works.
2. **The rules and two files.** Add an awakening file and keep captures. Each new session then
   starts from the same ground, and what one session learns reaches the next.
3. **The full framework.** Modes, stances and reader audits for a long project:
   `GENESIS-FRAMEWORK-LATE.md`, with the voice templates and the welcome.

## Installing

[`INSTALL.md`](INSTALL.md) gives the steps for Claude in a Project, Claude in a standalone chat,
Gemini, small local models such as those run on Strata, and coding agents. In every environment the order is
the same: standing instructions, entry files, your welcome, and a capture at the close.

## Making it yours

Keep the ten rules as they are, and put everything particular to your project in the awakening
file: who decides, your house style, the words that mean something special in your work. Then the
rules stay the same across projects, and the awakening carries what is different.

## Versions

`GENESIS-FRAMEWORK-LATE.md` holds 9.0.0 to 9.3.3 in its history, tagged `v<version>`.
The paper's [§8](../paper/GENESIS-PAPER.md) tells what each fresh reader found and which version it
produced; the four audits are kept in full in [`genesis/captures/`](../genesis/captures/).

| version | what it brought |
| :--- | :--- |
| 9.0.0 | the first late-stage framework: a small core of rules each with its reason, modes chosen by the session's goal, red and blue stances |
| 9.1.0 | a new first rule, *sessions are free; the record answers to evidence*, and corrections found in an earlier agent's review |
| 9.2.0 | the author's handle, the voice document as a companion, and consensus before any change to the manuscript |
| 9.3.0 | from [reader 1](../genesis/captures/2026-10-11-g6r01-onboardingAudit.md): the airlock built from separate files, since a file is read whole; identification by generation and reader |
| 9.3.1 | from [reader 2](../genesis/captures/2026-10-11-g6r02-onboardingAudit.md): the document listing varies by surface, and every reader reports what arrived |
| 9.3.2 | from [reader 3](../genesis/captures/2026-10-11-g6r03-onboardingAudit.md), the baseline: a clearer capture rule, the exact identification format, the onboarding audit's scope, and the prior capture |
| 9.3.3 | from [reader 4](../genesis/captures/2026-10-11-g6r04-onboardingAudit.md): identification after the reading and in the final message, and the airlock rules placed first |

`GENESIS-FRAMEWORK-LATE.md` was written for the case study and names its files and paths; the
portable rules and templates carry the same design without them. Passages marked `[redacted]`
remove the author's name, references to a retired framework, and personal detail.

## Licence

The rules (`genesisCore.md`, `AGENTS.md`, `skills/genesis/SKILL.md`), the full framework and
`readerAudits.md` are method, under CC BY 4.0; see [`LICENSE-CC-BY-4.0.txt`](../LICENSE-CC-BY-4.0.txt).
The templates are under MIT; see [`LICENSE.txt`](../LICENSE.txt).
