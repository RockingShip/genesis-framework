# Backlog: genesis-framework

*The one list where this repository's open points live until they are resolved, after
[`templates/backlog.md`](../genesis-framework-late/templates/backlog.md). Captures in
[`captures/`](captures/) stay as written; their open lines are carried here. Items are struck as
resolved only on xyzzy's ruling. This list is paired with the case study's
`claude/GENESIS-BACKLOG.md`: a change to one is made to the other in the same step.*

| item | source | who acts | destination | status |
| :--- | :--- | :--- | :--- | :--- |
| the repository's description, homepage link and topics, so it reaches GitHub search and the `genesis-framework` topic | the session of 2026-10-13 | author rules, agent sets | the repository settings | open, later |
| a destination test in the framework: before following a thread, name its destination (framework, paper or case study) and spend effort in proportion to what it needs | the session of 2026-10-13, the drift after reader 6 | author rules, agent drafts | `genesis-framework-late/GENESIS-FRAMEWORK-LATE.md` | open |
| an island and mainland section in the awakening template: what readers will mistake the work for, what it is, and where the comparison ends | Gemini's review, 2026-10-13 | author rules, agent drafts | `genesis-framework-late/templates/awakening.md` | open |
| a script listing every open `[AUTHOR-VERIFY]` across the captures, to check that each has reached this backlog | Gemini's review, 2026-10-13 | author rules, agent writes | a `scripts/` folder, under MIT | open |
| an init script that copies the templates into a new `genesis/` folder and starts a dated capture | Gemini's review, 2026-10-13 | author rules, agent writes | a `scripts/` folder, under MIT | open |
| a ChatGPT section in the late install guide | the session of 2026-10-12 | agent drafts, author rules | `genesis-framework-late/INSTALL.md` | open, later |
| a lean download of the late line, attached to a release | the session of 2026-10-12 | author | the next release | open, later |
| the genesis image: the footprint favicon (32, 180, 192) into `assets/` and `_config.yml`, an SVG link in `_includes/head.html`; the social preview uploaded by the author | the session of 2026-10-14; the author's choice | agent installs, author uploads the preview | `assets/`, `_config.yml`, repository settings | open, with r4 |
| the late line's first outside test, on a small local model run on Strata | the session of 2026-10-12 | the author's friend, then author | a capture in `captures/` | open, later |
| the table width fix carried into the theme itself, for every RockingShip site | the session of 2026-10-13 | author | `RockingShip/moonwalk`, `moonwalk.css` | open, optional |
| the next release, carrying the changes listed as Unreleased; its notes name each versioned artefact by its path, with the version in brackets | `CHANGELOG.md`; the author's remark on 1.1.0 | author | tag `vX.Y.Z` and a release | open |
| the tag `paper-r3` at `cd0eda0`, signed, and the tag script extended to place `paper-rN` from r4 | the session of 2026-10-13 | author | tag `paper-r3` | open |
| delete the unpacked copy of the author's private session snapshots, and the two internal BOOK10 files of 2026-10-14 (friction flags, epiphanies), kept for knowledge extraction only | the author's ruling of 2026-10-13 | agent | the session's scratch space | open, when r4 is settled |
| licensing as ruled: CC BY 4.0 for everything by default, MIT stated in-file where a file differs; update the README's licence section, the late line's README and `INSTALL.md`, and the author's guide | the author's ruling of 2026-10-14 | agent drafts, author rules | `README.md`, `genesis-framework-late/` | open, with r4 |
| the paper r4, drafted on a branch and landed as one commit `GENESIS-PAPER r4` after the author's review in a pull request | the session of 2026-10-13 | agent drafts, author rules | `paper/GENESIS-PAPER.md` | open |
| r4: a line under the title naming the repository, with permalinks at its tag `paper-rN` and its release | the author, 2026-10-13 | agent drafts, author rules | `paper/GENESIS-PAPER.md` | open |
| r4: an authorship statement near the front, along three dimensions (drafted prose, ideas, editorial authority), with the three models' estimates as evidence | the authorship readings of 2026-10-13; the author's ruling of 13:25 | agent drafts, author rules | `paper/GENESIS-PAPER.md` | open |
| r4: one sentence in the abstract separating observed process outcomes from unmeasured quality outcomes | the repository assessment of 2026-10-13 | agent drafts, author rules | `paper/GENESIS-PAPER.md` | open |
| r4: a paragraph naming co-author and cold reader as two roles of one agent, each with its obligations, after red, blue and the switch | the author, 2026-10-13 | agent drafts, author rules | `paper/GENESIS-PAPER.md` | open |
| r4: terms defined in island words at first use, a pointer in the introduction, and a late section mapping them onto the mainland | the terminology reading of 2026-10-13; the author's ruling on placement | agent drafts, author rules | `paper/GENESIS-PAPER.md` | open |
| r4: an observation that a cold reader's register is itself a property of the measurement, shown by the enthusiastic and the measured readings of 2026-10-13 | the session of 2026-10-13; the author's ruling of 13:25 | agent drafts, author rules | `paper/GENESIS-PAPER.md` | open |
| r4: the untangle v2 README (2020 to 2021, by hand) as the baseline of the author's own prose, quoted in short lines, the staircase and the chiasmus included | the session of 2026-10-13; the author's ruling of 13:42 | agent drafts, author rules | `paper/GENESIS-PAPER.md`, §7.1 | open |
| r4: a rhythm table comparing the README and the paper (sentence length, short and long sentences, negations), recomputed with a stated method | the session of 2026-10-13 | agent measures, author rules | `paper/GENESIS-PAPER.md`, §7.1 | open |
| r4: the summarising reader that kept the README's content and lost its form, recorded as a stumble | the session of 2026-10-13 | agent drafts, author rules | `paper/GENESIS-PAPER.md` | open |
| r4: an origin paragraph near the front, in the third person: writing stalled under ideas too large for the page; AI as a writing tool disappointed (quality and detail, erosion by summarising, misunderstanding, a lack of pushback); the framework was built to answer each frustration, with the untangle README as the standard held | the author, 2026-10-13 13:45; ruling of 13:46 | agent drafts, author rules | `paper/GENESIS-PAPER.md`, introduction | open |
| r4: the findings of reader 6 of generation 6 (P1 to P23, S1, S2), each to be triaged with the author; P7 ruled: frameworks 3.1 to 8.2.0 on Gemini 2.5 Pro, Gemini 3 Pro from its release in November 2025, 3.1 Pro by March 2026, dated from the session dumps, with later Gemini work marked unrecorded, beside the author's verbatim quote | `captures/2026-10-13-g6r06-paperReading.md` | author rules, agent drafts | `paper/GENESIS-PAPER.md` | open |
| r4 inputs still to gather: the friend's response, once its place is ruled | the session of 2026-10-13 | author, agent | `genesis/captures/` | open |
| GitHub's sidebar shows both licences: `LICENSE-MIT.txt` and `LICENSE-CC-BY.txt`, the latter as canonical legal code under a name GitHub's patterns accept | the session of 2026-10-13 | author checks, agent writes | the repository page | resolved, 2026-10-13 |
| framework sessions share the Topological project with the case study, separated by the `GENESIS-` prefix and kept in step through paired files | the framework session, 2026-10-13 | author | the case study's `claude/STANDING-Project-Layout.md` | resolved, 2026-10-13 |
| release 1.1.0, signed, with `late-9.4.0` tagged | the session of 2026-10-13 | author | tags `v1.1.0`, `late-9.4.0` | resolved, 2026-10-13 |
| the Pages view on the moonwalk theme, outside the RockingShip showcase | the session of 2026-10-12 | author, agent | `_config.yml`, `assets/genesis.css` | resolved, 2026-10-13 |
| release 1.0.0, signed | the session of 2026-10-12 | author | tag `v1.0.0` | resolved, 2026-10-13 |
