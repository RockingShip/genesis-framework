# Installing the early line

The early line works differently from the late one. Its framework is a long constitution the model
assimilates at the start of a session, with **one role** loaded beside it, and its cold readers run
in a **separate** session with their own pair of files. So each session type gets its own setup.

| session type | load | purpose |
| :--- | :--- | :--- |
| co-authoring | `GENESIS-FRAMEWORK-EARLY.md`, then one file from `roles/` | recovering, structuring and drafting |
| cold reading | `roles/CLAUDE-REDTEAM-standing-instructions.md` and `roles/CLAUDE-COLDSTART-orientation.md` | reporting where a fresh reader trips |

The roles follow the pipeline in `roles/GENESIS-PIPELINE.md`: the Digital Archaeologist recovers,
the Lexicographer structures, the Technical Author drafts. One role per session.

**Size.** The framework is about 7,000 words, written for a large model with a long context. For a
small local model, use the [late line](../genesis-framework-late/) instead.

**Adapt before use.** These files were written for the case study and name its concepts. Replace
the project-specific passages with your own, and fill in the bracketed status fields of the cold
reader's orientation for each pass.

---

## Gemini, the line's home

Written with, and tuned to, Gemini 3.1 Pro.

**In a Gem**, for co-authoring:

1. **Gem instructions:** *Assimilate the attached Genesis Framework as your operating framework,
   then adopt the attached role.*
2. **Gem knowledge:** `GENESIS-FRAMEWORK-EARLY.md` and the one role for this Gem. Make one Gem per
   role.
3. **Each session:** open a new chat with the Gem and state the goal. The framework opens with its
   own handshake; let it run.
4. **Carrying work on:** findings move between sessions by hand. Paste what the previous stage
   produced into the next stage's session.

**In a standalone chat:** attach the framework and the role to the first message, with the same
instruction, then state the goal.

## Claude, for cold reading

The cold reader files were written for readers on Claude.

**In a Project:**

1. **Project instructions:** paste `roles/CLAUDE-REDTEAM-standing-instructions.md`. It stays the
   same for every pass.
2. **Project knowledge:** upload the manuscript files to be read.
3. **Each pass:** start a new chat and paste `roles/CLAUDE-COLDSTART-orientation.md` as the first
   message, with its status fields filled in for this pass.
4. **At the end:** save the report and carry it, by hand, to the co-authoring sessions.

**Standalone chat:** attach both red team files and the manuscript files to the first message.

**For co-authoring in Claude**, follow the Gemini instructions with a Project in place of a Gem: the
framework and one role as project knowledge, the instruction to assimilate them as project
instructions. Expect differences: the line was tuned to another model.

## Small local models

The early line is too large for a small model to hold. Use the
[late line](../genesis-framework-late/INSTALL.md), whose rules fit on one page.

## Coding agents

The early line predates rules files. To use it in a repository, put the framework and the chosen
role in the repository and point the agent at both in its `AGENTS.md` or `CLAUDE.md`, with the
instruction to assimilate them before starting.
