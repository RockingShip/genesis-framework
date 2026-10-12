# Awakening: genesis-framework

*The entry file for agents working on this repository. The repo uses its own kit: the rules are in
[`AGENTS.md`](../AGENTS.md), and this file carries what is particular to the repo.*

**Updated:** 2026-10-12

## The project

This repository publishes the Genesis Framework: a method for writing a long work with AI agents
across many sessions. It holds a portable kit, the v9 framework as used on its case study, the
paper that accounts for the method, and the record of every earlier version. It is itself an
example of the method in use.

## The author

The author is **xyzzy**, of RockingShip Research. Address him as Xyzzy. He holds the knowledge, the
rulings and the accountability.

Agents may fix typos, broken links and formatting directly. Everything else is proposed first and
made once Xyzzy agrees: new files, changes of content, renames, and anything touching the verbatim files of either line or the case study.

## Where things stand

- Released as 1.0.0 on 2026-10-12 and 1.1.0 on 2026-10-13, with the whole repo as the release. From here, history stays as
  it is: corrections arrive as new commits.
- `genesis-framework-early` 8.2.3; `genesis-framework-late` 9.4.0; `paper/GENESIS-PAPER.md` r3.
- The Pages view runs on the `RockingShip/moonwalk` theme, outside the RockingShip showcase until
  the case study's manuscript is published.
- Waiting: everything open is in [`backlog.md`](backlog.md).

## Where things are

| file or folder | holds |
| :--- | :--- |
| `README.md` | the front door: which line to use, how the pieces fit, models, thanks, licences, contact |
| `genesis-framework-late/` | the late line: rules in three forms, the full framework, templates, the reader audit guide |
| `genesis-framework-early/` | the early line: the full framework and its roles |
| `paper/` | the paper, `GENESIS-PAPER.md`, with its companions `reachingConsensus.md` and `positiveFraming.md` |
| `case-study/` | what the framework did on the Topological manuscript, its worked examples (`GENESIS-AWAKENING.md`, `VOICE-0-Reading-the-Author.md`), and `LINEAGE.md` |
| `genesis/backlog.md` | every open point from the captures, with who acts and where it lands, until resolved |
| `CHANGELOG.md` | every change, one timestamped line each |
| `genesis/captures/` | what earlier sessions on this repo decided, learned and left open; also the four reader audits of 2026-10-11 (`g6r01` to `g6r04`), copied from the case study, which produced the late line's 9.3.0 to 9.3.3, and six fourth generation manuscript readings of 2026-08-14 (`g4r01` to `g4r09`) |

## House style

Xyzzy's standing instruction, verbatim:

> Avoid negative words. Frame from the positive. Avoid the use of NOT and all it's variations like
> don't, won't can't, shouldn't. Avoid using dashes in prose as separator. Spelling British English.
> Keep asking for clarifications until we mutually agree on the topic before presenting code or
> proposals.

## Conventions

- **File names:** content files in lowerCamelCase, Latin-1, without spaces (`genesisCore.md`).
  Products in capitals (`GENESIS-PAPER.md`, `GENESIS-FRAMEWORK-LATE.md`). Conventional files keep
  their conventional names (`README.md`, `AGENTS.md`, `SKILL.md`, `LICENSE.txt`). Files that hold
  verbatim history keep their original base names. The case study, which lives outside git, is
  named with its revision: `TOPOLOGICAL-MANUSCRIPT-r47`.
- **Versions:** one file per artefact; each version is a commit of that file, with the version in
  the commit message; the two framework files' versions also carry a tag such as `late-9.3.3`;
  releases of the whole repository are tagged `vX.Y.Z`. The EARLY and LATE lines take their own
  version numbers, and the late line's portable rules follow its numbers.
- **Licences:** method and prose under CC BY 4.0, including the portable rules and both
  frameworks; templates and scripts under MIT.
- **Privacy:** the author appears only as `xyzzy` with `xyzzy@rockingship.org`. Material the author has
  retired stays outside the repo; the history keeps only what `case-study/LINEAGE.md` lists. Outside testers stay
  unnamed. The Topological software and its licensing live elsewhere.
- **Record files** are verbatim; a removed passage reads `[redacted]`. Claims without a traceable
  source are marked `[UNVERIFIED]`.
- **Commits:** author `xyzzy <xyzzy@rockingship.org>`, committer `Claude <noreply@anthropic.com>`,
  pushed to `main`. While the repo is private, rewriting history and force-pushing are allowed.
- **Changelog:** one line per change, `YYYY-MM-DD HH:MM:SS Added|Changed|Fixed: …`, newest first.

## Words to know

| term | meaning here |
| :--- | :--- |
| the late line, the early line | `genesis-framework-late/` and `genesis-framework-early/`, one folder each to copy |
| the case study | the *Topological Computing* manuscript, where the framework was developed |
| blue, red | the co-author's stance and the cold reader's stance |
| generation, reader | the project's maturity level, and one session's agent within it |
| capture | a session's record of what it decided, learned and left open |

## Your first reply

Open with what you read and the goal of this session as you understood it. Ask about anything
unclear before you start work.
