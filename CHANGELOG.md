# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
Each artefact keeps its own versions as commits and tags; this file summarises them.

## [Unreleased]

```
2026-10-13 01:50:06 Added: a convention for release notes, naming each versioned artefact by its path with the version in brackets; the backlog updated after release 1.1.0.
2026-10-13 12:25:00 Fixed: the README contents table and tag range brought to the late line 9.4.0; `LICENSE.txt` renamed `LICENSE-MIT.txt`, so GitHub shows both licences rather than MIT alone. Both found by an outside reading of the repository.
2026-10-13 18:00:00 Fixed: `LICENSE-CC-BY-4.0.txt` replaced by the canonical plain-text legal code, so GitHub recognises it; the earlier copy was a reflowed web version.
2026-10-13 18:20:00 Fixed: `LICENSE-CC-BY-4.0.txt` renamed `LICENSE-CC-BY.txt`; the dots in "4.0" put the name outside the patterns GitHub uses to find licence files.
```

## [1.1.0] - 2026-10-13

The backlog, and a cleaner repository.

- `genesis-framework-late/` at 9.4.0: open points from every capture are carried to one backlog and
  struck as resolved only on the author's ruling. Rule 10 in its three forms, a new
  `templates/backlog.md`, and the capture and closing templates follow.
- `genesis/backlog.md`: this repository's own backlog, paired with the case study's.
- Tags: `vX.Y.Z` for releases, `early-<version>` and `late-<version>` for the framework.
- Every commit signed, and every commit message free of session links.
- The Pages view's tables fitted to their content.

```
2026-10-13 01:36:00 Changed: every commit signed; session links removed from every commit message.
2026-10-13 01:32:01 Changed: `GENESIS-FRAMEWORK-LATE` 9.4.0, amended in place: one backlog per layer in the case study, its layout recorded in `claude/STANDING-Project-Layout.md`; `genesis/backlog.md` paired with the case study's `claude/GENESIS-BACKLOG.md`.
2026-10-13 01:21:22 Added: `GENESIS-FRAMEWORK-LATE` 9.4.0, the backlog: open points from every capture carried to one list; rule 10 in its three forms, the capture and closing templates, a new `templates/backlog.md`, the install guide, and this repository's own `genesis/backlog.md`.
2026-10-13 01:15:44 Changed: the fifth generation named as deprecated, its contributions carried into the sixth, in the paper §2.1, the late framework and the case study's awakening.
2026-10-13 01:11:11 Fixed: rule 10 in `AGENTS.md` now asks for the [VERIFIED], [AUTHOR] or [READER] mark, as `genesisCore.md` and `SKILL.md` do.
2026-10-13 00:58:26 Changed: `GENESIS-FRAMEWORK-LATE` 9.3.3, amended in place: M7 kept, for preparing any volume or paper for the author's read.
2026-10-13 00:19:01 Changed: framework tags are `early-<version>` and `late-<version>`, leaving `vX.Y.Z` to releases.
2026-10-13 00:15:45 Changed: tags only on the framework versions, as `v<version>`; every other version is named in its commit subject.
2026-10-12 23:55:39 Fixed: Pages tables: the first column fits its content and the others share the width (`assets/genesis.css`, with the theme's head include extended to load it).
2026-10-12 23:55:39 Fixed: 8.2.3 carries eight core protocols, in the README and the lineage, as in the paper.
```

## [1.0.0] - 2026-10-12

The first release: the Genesis Framework as a method for writing a long work with AI agents across
many sessions, with its own history and its case study.

- `genesis-framework-late/` at 9.3.3: the portable rules in three forms, the full framework, six
  templates, the reader audit guide and an install guide per environment.
- `genesis-framework-early/` at 8.2.3: the full framework and its roles, every recovered version
  tagged.
- `paper/GENESIS-PAPER.md` at r3, with its two companions, `reachingConsensus.md` and
  `positiveFraming.md`.
- `case-study/`: the worked examples and the lineage.
- `genesis/`: the repository's own use of the late line, with the reader audits and readings that
  shaped it.

```
2026-10-12 23:26:32 Changed: release state: README status, paper r3 out of draft, awakening updated.
2026-10-12 23:25:48 Fixed: Strata named correctly, as the engine that runs a small local model rather than the model itself.
2026-10-12 23:15:37 Added: the GitHub Pages view on the `RockingShip/moonwalk` theme (`_config.yml`, `_data/home.yml`, favicons); the README serves as the home page.
2026-10-12 23:07:17 Changed: history rewritten so that no version carries the retracted subject; the version tags are re-pointed to match.
2026-10-12 23:06:05 Removed: from the paper, the corpus index and the reverse sweep as outstanding work, both belonging to the case study; Appendix B becomes *The corpus*.
2026-10-12 23:03:19 Fixed: paper §8.1, Claude as cold reader from May and June 2026, as co-author from r19.
2026-10-12 22:02:45 Added: paper §5.4, erosion at the scale of the book: the split between storage and solution, and the wounds it left.
2026-10-12 21:55:10 Removed: a retracted subject from the paper §2.1 and, as `[redacted]`, from the late framework and the case study's awakening. Fixed: the lineage's two dated notes verified by the author.
2026-10-12 21:51:39 Fixed: every `[UNVERIFIED]` mark in the paper settled; the author verified each claim, and the mark leaves the reader contract. The fourth generation's welcome dated to the middle stage.
2026-10-12 21:50:08 Changed: paper §8.1, Gemini co-authored the early stage; from r19 the author set Gemini and Claude against each other.
2026-10-12 21:47:12 Changed: paper §8.1 records r19 as Claude's first involvement, with every earlier book draft written with Gemini.
2026-10-12 21:41:39 Changed: paper §8.1 dates the early stage from June 2025 and the middle stage from the tenth book draft, late May 2026, through r19.
2026-10-12 21:38:50 Added: paper §8.1 describes the case study's three stages, with the late stage from r46.
2026-10-12 21:33:59 Fixed: the cold reader files served the middle stage, written after 8.2.3; they stay in the early line, which covers the early and middle stages.
2026-10-12 21:31:17 Removed: paper §2.3, "The fourth author", a term without a recoverable source; the rest of the paper carries its content.
2026-10-12 21:27:35 Changed: paper §3 gains the layout paradox and §4.3 the stumble rates of six fourth generation readers.
2026-10-12 21:25:15 Fixed: the revision each fourth generation reader read (r23 to r31), as the author confirms.
2026-10-12 21:22:36 Added: six fourth generation manuscript readings of 2026-08-14 in `genesis/captures/` (readers 1 to 5 and 9); the paper's three G4R05 quotations link to their source.
2026-10-12 21:19:14 Fixed: paper §4.1 and §4.8, three reader quotations settled against their source, the fifth reader of the fourth generation (r29, 2026-08-14); wording restored and labels corrected.
2026-10-12 21:01:39 Changed: paper §5.1 gains the protocol counts of every early version and the bootstrap as detector; 8.2.3 carries eight core protocols.
2026-10-12 20:53:51 Changed: `reachingConsensus.md` and `positiveFraming.md` move from `case-study/` to `paper/`, beside the paper, which links to them in §2.2 and §4.7.
2026-10-12 20:53:51 Changed: paper r3 per the author's reading: the island and mainland defined at §4, transcript size in §4.9, the cold reader files dated after 8.2.3, the count behind §6, the purpose of the switch, the reasons for the airlock and the captures.
2026-10-12 19:30:33 Added: the four generation 6 reader audits in `genesis/captures/`, which produced the late line's 9.3.0 to 9.3.3; linked from the README, the late README, `readerAudits.md`, the paper's §8.4 and `genesis/awakening.md`.
2026-10-12 19:14:59 Added: `case-study/positiveFraming.md`, the house style's reason in the author's words and the negation method; linked from the case study, the voice template and the paper's §7.2.
2026-10-12 19:12:13 Added: `case-study/reachingConsensus.md`, one paragraph through fifteen versions to consensus.
2026-10-12 18:54:50 Added: README section "How this was written", agreed in full with the author.
2026-10-12 18:44:20 Added: the late install guide covers Claude Code, the Claude API and claude.ai personal preferences.
2026-10-12 18:38:17 Added: `INSTALL.md` in each line's folder: Claude in a Project, Claude standalone, Gemini, Strada and other small local models, coding agents.
2026-10-12 18:38:17 Changed: README explains the repository's own `genesis/` folder and links both install guides.
2026-10-12 18:38:17 Changed: the paper names the late line's portable rules consistently.
2026-10-12 18:28:29 Added: `AGENTS.md` and `genesis/`, the repository's own use of the late line.
2026-10-12 18:28:29 Added: `case-study/`: the case study, its worked examples (`GENESIS-AWAKENING.md`, `VOICE-0-Reading-the-Author.md`) and `LINEAGE.md`.
2026-10-12 18:28:29 Added: `paper/GENESIS-PAPER.md`, draft r3, rebuilt from r2 with a chapter on the late line.
2026-10-12 18:28:29 Added: `genesis-framework-late/`: `GENESIS-FRAMEWORK-LATE.md` 9.0.0 to 9.3.3, the portable rules in three forms, six templates and the reader audit guide.
2026-10-12 18:28:29 Added: `genesis-framework-early/`: `GENESIS-FRAMEWORK-EARLY.md` 3.1 to 8.2.3, with its roles in `roles/`.
2026-10-12 18:28:29 Added: README with the choice between the lines and how the pieces fit; licences (MIT and CC BY 4.0), `.gitignore` and `.gitattributes`.
```
