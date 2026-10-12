# genesis-framework-early

The Genesis Framework for the **early and middle stages**: when the corpus is mostly silence,
knowledge sits scattered across sessions, and agents are expected to propose, extrapolate and
overreach so that the author can react. Copy this one folder into your own setup.

Written with, and tuned to, Gemini 3.1 Pro. The full framework is at 8.2.3. The cold reader files
followed it, for the middle stage, written for readers on Claude Opus 5.

## What is here

| file | use |
| :--- | :--- |
| [`GENESIS-FRAMEWORK-EARLY.md`](GENESIS-FRAMEWORK-EARLY.md) | the full framework: a constitution of core protocols, cognitive systems and executable protocols, loaded at the start of a co-authoring session |
| [`roles/GENESIS-PIPELINE.md`](roles/GENESIS-PIPELINE.md) | the Mine, Refinery and Forge pipeline: how the stages hand work to one another |
| [`roles/GENESIS-ROLE-Digital-Archaeologist.md`](roles/GENESIS-ROLE-Digital-Archaeologist.md) | the Mine: recovering knowledge from raw session transcripts |
| [`roles/GENESIS-ROLE-Lexicographer.md`](roles/GENESIS-ROLE-Lexicographer.md) | the Refinery: turning the recovered narrative into a lexicon |
| [`roles/GENESIS-ROLE-Technical-Author.md`](roles/GENESIS-ROLE-Technical-Author.md) | the Forge: turning the lexicon into chapters |
| [`roles/CLAUDE-REDTEAM-standing-instructions.md`](roles/CLAUDE-REDTEAM-standing-instructions.md) | the cold reader's invariant stance, sent with every red team session |
| [`roles/CLAUDE-COLDSTART-orientation.md`](roles/CLAUDE-COLDSTART-orientation.md) | the cold reader's welcome, which carries what goes stale |

## Installing

[`INSTALL.md`](INSTALL.md) gives the steps for Gemini, the line's home, for Claude as cold reader,
and for coding agents. Each session type gets its own setup.

## How it runs

1. **Co-authoring sessions** load `GENESIS-FRAMEWORK-EARLY.md`, then one role from the pipeline.
   Load one role at a time.
2. **Cold readers** load the red team pair: the standing instructions, which stay the same, and the
   orientation, which changes with the project. They report where the text tripped them, and the
   author carries the findings back to the co-authoring sessions.
3. **When the manuscript nears completion**, move to [`genesis-framework-late`](../genesis-framework-late/).

## Versions

Every file holds its recovered versions in its history, each tagged:

| file | versions | tags |
| :--- | :--- | :--- |
| `GENESIS-FRAMEWORK-EARLY.md` | sixteen, 3.1 to 8.2.3 | `framework-early-<version>` |
| `roles/GENESIS-ROLE-Digital-Archaeologist.md` | ten, 2.1.3 to 5.3.0 | `archaeologist-<version>` |
| `roles/CLAUDE-COLDSTART-orientation.md` | 1.0.0, 1.1.0 and 2.0.0; 1.1.0 is the one in use | `coldstart-<version>` |
| `roles/CLAUDE-REDTEAM-standing-instructions.md` | 1.0.0 | `redteam-1.0.0` |
| `roles/GENESIS-PIPELINE.md` | 1.3.0 | `pipeline-1.3.0` |
| `roles/GENESIS-ROLE-Lexicographer.md`<br>`roles/GENESIS-ROLE-Technical-Author.md` | 1.0.0 each | `lexicographer-1.0.0`<br>`technical-author-1.0.0` |

```sh
git log --follow genesis-framework-early/GENESIS-FRAMEWORK-EARLY.md
git show framework-early-7.2:genesis-framework-early/GENESIS-FRAMEWORK-EARLY.md
```

Where each version came from, and what reads across them, is in the case study's
[`LINEAGE.md`](../case-study/LINEAGE.md).

## Notes

* These files were written for the case study, the *Topological Computing* manuscript, and name its
  concepts. They are verbatim apart from passages marked `[redacted]`.
* The early line asks the model to run and report on internal systems. The late line keeps the
  purposes those systems served and replaces their readouts with practical conduct; the paper's
  [§8.2](../paper/GENESIS-PAPER.md) explains the change.

## Licence

Method and prose, under CC BY 4.0; see [`LICENSE-CC-BY-4.0.txt`](../LICENSE-CC-BY-4.0.txt).
