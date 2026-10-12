# Lineage

The early line of the Genesis Framework and its companions: every recovered version, kept as
found, each version a commit of its file and each carrying a tag. Each consecutive pair of versions
brackets a change in practice, and often an incident. This note says where each version came from,
what can be read across versions, and what was left out.

**Model.** The framework, Archaeologist, pipeline and role files were written with, and
tuned to, Gemini 3.1 Pro. The red team and cold-start files followed 8.2.3, for the middle stage,
written for cold readers running on Claude Opus 5, the latest Opus at the time.

**Marks.** `[redacted]`: a passage removed from a verbatim file.

---

## Where the files came from

| file | versions | tags | source |
| :--- | :--- | :--- | :--- |
| `genesis-framework-early/GENESIS-FRAMEWORK-EARLY.md` | the co-creative framework, 3.1 to 8.2.3, sixteen versions | `framework-early-<version>` | see the table below |
| `genesis-framework-early/roles/GENESIS-ROLE-Digital-Archaeologist.md` | 2.1.3 to 5.3.0, ten versions | `archaeologist-<version>` | the Genesis r2 bundle |
| `genesis-framework-early/roles/CLAUDE-COLDSTART-orientation.md` | 1.0.0, 1.1.0 and 2.0.0 | `coldstart-<version>` | the Genesis r2 bundle |
| `genesis-framework-early/roles/CLAUDE-REDTEAM-standing-instructions.md` | 1.0.0 | `redteam-1.0.0` | the Genesis r2 bundle |
| `genesis-framework-early/roles/GENESIS-PIPELINE.md` | 1.3.0 | `pipeline-1.3.0` | the Genesis r2 bundle |
| `genesis-framework-early/roles/GENESIS-ROLE-Lexicographer.md`, `genesis-framework-early/roles/GENESIS-ROLE-Technical-Author.md` | 1.0.0 each | `lexicographer-1.0.0`, `technical-author-1.0.0` | the Genesis r2 bundle |

To read one version in full: `git show framework-early-7.2:genesis-framework-early/GENESIS-FRAMEWORK-EARLY.md`.

Every version is verbatim. The only changes are four passages of personal detail in the cold-start
versions, each shown as `[redacted]`.

## The co-creative framework

Sources, in order of trust: xyzzy's own markdown files, kept byte for byte (**original**);
then xyzzy's manual extracts from the session transcripts (**transcript**). From each
transcript only the document is kept, from its title line to its last protocol. The
surrounding conversation and the closing "Primary Directive" line belonged to the prompt
and are removed.

| version | source | transcript turn | note |
| :--- | :--- | :--- | :--- |
| 3.1 | transcript | 56-22-A | the earliest surviving version |
| 3.2 | transcript | 58-1-H | |
| 3.3 | transcript | 57-20-A | a proposal, drafted inside the Canon Evolution Framework sandbox |
| 3.6 | original | | |
| 3.7 | transcript | | |
| 4.0 | transcript | 63-30-H | the full version as xyzzy expected it, pasted by him |
| 5.0 | transcript | 64-1-A | |
| 6.0 | transcript | 63-100-A | Part 3 shortened by the model to a one-line reference to 4.0 |
| 7.1 | transcript | 67-1-H | the successor preamble removed |
| 7.2 | original | | carries the bootstrap hardening: 0.0-F, 0.1, and the Structural Interpretation Mandate |
| 7.3 | transcript | 74-26-A | a draft, written while 7.2 was operational |
| 7.4 | original | | |
| 7.7 | original | | |
| 8.1.0 | original | | |
| 8.2.0 | transcript | 101-1-H | header corrected to v8.2.0 and stray trailing text removed, by xyzzy |
| 8.2.3 | original | | the last version before v9 |

**Read across versions.** 3.1 carries four core protocols, six cognitive systems and nine
executable protocols. 8.2.3 carries seven core protocols, twelve systems and twenty-nine
executable protocols. All nineteen elements of 3.1 are still present in 8.2.3 at their
original numbers, and four carry new names: the State Vector Snapshot became Dynamic State
Persistence, Revert to Snapshot became Revert to Dynamic State, the Canon Evolution
Framework became the Interactive Canon Evolution Framework, and Generate Genesis Prompt
became Generate Genesis Framework. The framework grew by accretion, roughly tripling
without a redesign.

**Two drafts of 7.2 exist.** The transcript at turn 72-1-H holds an earlier 7.2 on a
branch built around a "Cognitive Engram". Later versions carry nothing from that branch.
The original 7.2 is the one on the main line, and the only one kept here.

**Turn numbers.** They run against version order in two places: 57 before 58, and 66
(where 7.4 and 7.7 sit) before 67, 72 and 74. The prefixes most likely count transcript
files rather than time.

## The Digital Archaeologist

Ten versions. Byte sizes are measured on the files here.

| transition | change | cause, as read from the protocols |
| :--- | :--- | :--- |
| 2.1.3 → 3.0.0 | 15,577 → 5,485 bytes, a total rewrite | philosophy stripped for operations |
| 3.0.0 → 3.1.0 | +28 bytes | cosmetic |
| 3.1.0 → 3.2.0 | Cycle Completion and the Artifact Containment Mandate added | a run failed to finish; logs containing instructions |
| 3.2.0 → 3.2.1 | Silent Processing added | **chat overflow, named in the protocol** |
| 3.2.1 → 4.4.0 | renumbered; Artifact Triage added; 8,319 → 4,878 bytes | log noise |
| 4.4.0 → 5.0.0 | +1,590 bytes | prose repair |
| 5.0.0 → 5.1.0 | Reference Abstraction added | the archive flooded by pasted blocks |
| 5.1.0 → 5.2.0 | +2,416 bytes; Silent Processing renamed Gated Streaming | the overflow fix strengthened |
| 5.2.0 → 5.3.0 | `AWAITING_RELEASE` state added; the forensic series added | a rescope rather than a repair |

An earlier note, verified by the author, dates nine of the ten versions to six days, 2025-11-19 to
2025-11-25, with a six-month gap before 5.3.0. The files themselves are undated.

**Two incidents named in the protocol text.**

*Output overflow.* Silent Processing, added at 3.2.1, states its purpose: *to manage output
bandwidth and prevent chat overflows when processing massive datasets.*

*Self-injection.* The Artifact Containment Mandate, present from 3.2.0, exists *to prevent
"Context Contamination" and "Recursive Prompt Injection" when analyzing raw logs*, and has
the agent read strings such as `"You are the Lead Author"` as inert data. An agent
archiving its own project's transcripts had begun to follow the role briefings inside them.

**One fix, three strengths.** Silent Processing at 3.2.1 asks the agent to keep its stages
internal. At 5.2.0 it becomes Gated Streaming. At 5.3.0 it gains a formal state,
`AWAITING_RELEASE`, with an explicit unlock command. An instruction became a gate and then
a state machine, which says the earlier forms fell short twice. Only the series shows it.

**Diff by title.** Protocol numbers were reassigned at 4.4.0, so comparing by number
produces false additions and deletions.

## The cold reader welcome

| version | bytes, as found | shape |
| :--- | ---: | :--- |
| 1.0.0 | 14,855 | a vocabulary primer, and a section on *The Failure Modes of Prior Cold Instances* |
| 1.1.0 | 4,426 | both removed: about 70% of the file was the teaching |
| 2.0.0 | 4,132 | a file manifest, tiers of pointers, and status fields left as templates |

The middle version holds the idea: teaching a cold reader in advance spends the cold read.
An earlier note, verified by the author, dates the three to 2026-05-28, 2026-05-29 and 2026-06-22.

The red team standing instructions, 1.0.0, were written as the invariant partner of the
welcome: they ride along unchanged, and the welcome carries whatever goes stale.

## Corrections to the r2 lineage note

Checked against the files, three statements in the Genesis r2 bundle's own lineage note
were adjusted here:

- the Artifact Containment Mandate first appears at 3.2.0, before 4.4.0;
- Gated Streaming first appears at 5.2.0, and 5.3.0 adds `AWAITING_RELEASE`;
- 8.2.3 carries seven core protocols, where the earlier note gave ten; and four of the
  nineteen 3.1 elements were renamed rather than kept under the same name.

## The paper's own revisions

The account of the method is [`paper/GENESIS-PAPER.md`](../paper/GENESIS-PAPER.md), with its
revisions tagged `paper-r<n>`. Draft r2, of 2026-08-19, was filed at the time as
`GENESIS-MANUSCRIPT-r2.md`; the repository starts at r3.
The case study is filed as `TOPOLOGICAL-MANUSCRIPT-r<n>`; its earlier revisions were filed as
`MANUSCRIPTr<n>`.

## Left out, and why

| item | reason |
| :--- | :--- |
| the earlier agent extracts of 3.1, 3.6, 4.0, 5.0, 6.0 and 7.2 | replaced by xyzzy's originals and transcript extracts |
| the transcript 7.2 (turn 72-1-H) and the transcript 7.4 (turn 66-36-A) | covered by the originals |
| the Genesis Generation Protocol proposal | an agent reconstruction; retired by xyzzy |
| a late-stage framework of the Gemini era | retired by xyzzy: built on an early mindset he has since left behind |
| personal detail | removed by xyzzy's ruling, each passage marked `[redacted]` |
| the session transcripts | over a gigabyte, and already mined; available on request for checking a specific claim |
