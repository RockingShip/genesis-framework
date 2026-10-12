# genesis-framework

A working method for writing a long manuscript together with AI agents, across many sessions and many agents.

Every agent session starts fresh. The Genesis Framework gives each newcomer the same way in: an entry file to read first, conduct rules that each carry their reason, and a capture habit so that what a session learns outlives it. The author keeps the final word. Agents act as challengers and as co-authors, and every change to the manuscript waits for mutual consensus.

## Status

Release 1.0.0, 2026-10-12: the early line at 8.2.3, the late line at 9.3.3, and the paper at r3.
The [changelog](CHANGELOG.md) records every change.

## Start here: early or late?

The framework comes in two lines, one per stage of a project. Pick the folder that matches where your work is, and copy that one folder.

| | [`genesis-framework-early`](genesis-framework-early/) | [`genesis-framework-late`](genesis-framework-late/) |
| :--- | :--- | :--- |
| **the stage** | early and middle: the subject is still being found, and knowledge sits scattered across sessions | late: the manuscript is close to complete, and the work is consolidation |
| **what agents do** | propose, extrapolate and overreach, so the author can react | check, ground and refine; every change waits for consensus |
| **how it is built** | a constitution of 8 core protocols, 12 cognitive systems and 29 executable protocols, which the model runs and reports on | ten conduct rules, each with its reason, and eight modes chosen by the session's goal |
| **who does the work** | a pipeline of roles: archaeologist, lexicographer, technical author, with cold readers on the side | one agent per session, cold reader first and co-author after the switch |
| **memory** | the author carries findings between sessions by hand | an entry file read first, and a capture written before each session ends |
| **portable** | written for its case study; adapt it by hand | the rules come in three portable forms, with templates for everything else |
| **written with** | Gemini 3.1 Pro; cold readers on Claude Opus 5 | Claude Opus 5.5 |
| **current version** | 8.2.3 | 9.3.3 |

Each folder has its own `INSTALL.md`, since the two lines load differently:
[late](genesis-framework-late/INSTALL.md) covers Claude in a Project, Claude in a standalone chat,
Gemini, small local models such as those run on Strata, and coding agents;
[early](genesis-framework-early/INSTALL.md) covers Gemini, Claude as cold reader, and coding agents.

**If you are unsure, start late.** Its ten rules on one page are enough to change how a session works, and they load into ChatGPT, Claude, Gemini, a coding agent or a local model.

## How the pieces fit

Each piece has one job and a moment at which it is loaded.

| job | when it is loaded | file in `genesis-framework-late` | worked example in `case-study` |
| :--- | :--- | :--- | :--- |
| standing instructions | always, by the environment | `genesisCore.md`, `AGENTS.md` or `skills/genesis/SKILL.md` | the case study's project instructions, which point to the awakening |
| entry file | first, by the agent | `templates/awakening.md` | `GENESIS-AWAKENING.md` |
| reading the author | first, beside the entry file | `templates/voice0.md` | `VOICE-0-Reading-the-Author.md` |
| writing as the author | when drafting | `templates/voice.md` | kept private by the case study |
| first message | to start a session | `templates/readerWelcome.md` | the two welcomes in the paper's Appendix A |
| session record | as the session goes | `templates/captureTemplate.md` | this repository's own [`genesis/captures/`](genesis/captures/) |
| close | at the end | `templates/closingPrompt.md` | §5 of `GENESIS-AWAKENING.md` |
| full rules and modes | when a mode calls for them | `GENESIS-FRAMEWORK-LATE.md` | the same file, written for the case study |
| fresh readers | when testing material or onboarding | `readerAudits.md` | the paper's §8.4 |
| why it works | to understand | the [paper](paper/GENESIS-PAPER.md) | |

Three of these are easy to confuse. The **standing instructions** sit in your environment and point the agent to the entry file. The **entry file** is the first file the agent reads and carries how to work. The **first message** is yours, and carries the goal of the session. Where an agent can read only what you paste, paste the entry file as the first message, before the welcome.

## Contents

| folder | holds | current |
| :--- | :--- | :--- |
| [`genesis-framework-late`](genesis-framework-late/) | the late line: rules in three forms, the full framework, six templates, the reader audit guide | 9.3.3 |
| [`genesis-framework-early`](genesis-framework-early/) | the early line: the full framework and its roles | 8.2.3 |
| [`paper`](paper/) | [`GENESIS-PAPER.md`](paper/GENESIS-PAPER.md), *Genesis*: the account of how the method arose, what each stumble taught, and what changed between the lines; beside it, two documents that go deeper, [`reachingConsensus.md`](paper/reachingConsensus.md) and [`positiveFraming.md`](paper/positiveFraming.md) | r3 |
| [`case-study`](case-study/) | *Topological Computing*, the manuscript the framework grew up with: worked examples and the lineage of every version | r47 |
| [`genesis`](genesis/) | this repository's own use of the late line: its entry file and captures | |

## This repository uses its own framework

The repository is written the way the late line asks a project to be written. Its root
[`AGENTS.md`](AGENTS.md) holds the ten rules, which coding agents load automatically, and tells every
agent to read [`genesis/awakening.md`](genesis/awakening.md) first: what the repository is, who decides,
the house style and the conventions. Each working session leaves a capture in
[`genesis/captures/`](genesis/captures/). So the `genesis/` folder is a live example of the folder
`genesis-framework-late/INSTALL.md` asks you to create in your own project. The same folder also
holds the four fresh readers' audits of the case study's onboarding, which produced the late line's
9.3.0 to 9.3.3, and six readings of the manuscript by fourth generation cold readers.

## Models

The framework has been shaped with two models, and each line names the model it was configured for.

* The early line, up to 8.2.3, was written with, and tuned to, Gemini 3.1 Pro. The cold reader files followed 8.2.3, for the middle stage, for readers on Claude Opus 5.
* The late line, from 9.0.0, is written with, and tuned to, Claude Opus 5.5.

How well a line carries over to other models is an open question, and this repository will record the evidence as it arrives.

## How this was written

This repository was written by AI agents at the sentence level, in co-authorship with its author. The division of the work is the method itself.

* **The author holds the content:** the knowledge, the insights, every ruling on what is true, and the accountability for all of it.
* **The agents hold the consistency:** turning rulings into prose, keeping terms, numbers and cross-references aligned across every file, and reporting where the text trips a fresh reader. They also propose (a term, a structure, a reading), and every proposal is marked as theirs.
* **Nothing is committed until both agree.** An agent's proposal waits for the author's ruling. An author's ruling is checked by the agent against the record, which says where it conflicts.

**The sentences are generated with the author's attention to detail and in his voice,** drawn from his own prose and from his corrections to earlier drafts. Each text then goes through rounds of revision until both agree on every sentence, so that it reads as spoken from a shared voice. Where a text is still on its way there, it is marked as a draft.

So the sentences are generated, and the content is authored. A generative tool produces content from a prompt. Here the content comes from the author, and what the agents contribute is that it holds together. The models involved are named under *Models*. Every commit names xyzzy as its author and Claude as its committer.

[`paper/reachingConsensus.md`](paper/reachingConsensus.md) shows the process on a single paragraph: fifteen versions, each a proposal, each move from one to the next the author's response to it.

## Thanks

The framework grew from two models in two roles. Gemini 3.1 Pro brought the blue team mindset: an
enthusiastic, inviting co-author whose fluency drafted the early and middle stages. Claude brought
the red team mindset: a plain, grounded reader that reported where the text asked for more than it
had shown.

## Versioning

Each artefact is one file, and its versions are its commits in git, each named in its commit's subject, such as `GENESIS-FRAMEWORK-LATE 9.3.3` or `GENESIS-PAPER r3`. Every version of the two framework files also carries a tag, the version number after a `v`: `v3.1` to `v8.2.3` for the early line, `v9.0.0` to `v9.3.3` for the late. The two lines take their own version numbers and never share one, so a bump in one leaves the other untouched; the late line's portable rules follow its numbers. Releases of the whole repository are tagged as well, starting with `v1.0.0`. See each file's history with `git log --follow <file>`, or its *History* view on GitHub. The [changelog](CHANGELOG.md) summarises every change.

## Licence

* Method and prose, including the rules (`genesisCore.md`, `AGENTS.md`, `SKILL.md`) and both frameworks: Creative Commons Attribution 4.0 International, see [LICENSE-CC-BY-4.0.txt](LICENSE-CC-BY-4.0.txt).
* Templates and scripts: MIT, see [LICENSE.txt](LICENSE.txt).

The software of the Topological case study is a separate project with its own licensing, and lives outside this repository.

## Contact

RockingShip Research, [www.rockingship.org](https://www.rockingship.org)

* For the organisation: research@rockingship.org
* For the author, xyzzy: xyzzy@rockingship.org
