> **Reader audit, dated 2026-10-11.** The capture written by reader 1 of generation 6 in the case
> study, kept there as `claude/capture/r47/2026-10-11-awakening-first-reader.md`. Its stumbles
> produced `GENESIS-FRAMEWORK-LATE` 9.3.0. Verbatim; passages marked `[redacted]` are removed.

# Capture: awakening of the first reader, sixth generation

Session of 2026-10-11, 14:02 [redacted]. Written by the session that held it (1.12).
Fencing per 1.4: author unmarked, agent inferences [READING], open rulings [AUTHOR-VERIFY].
Status: stumble report written at the switch, before any explanation from the author.

## The goal, as given

You are the 1st reader of the 6th generation of co-authoring agents working on the manuscript for topological computing. I am responsible for the knowledge, insights and accountability.
Your stumbles are important because they signal where attention needs to go. Flag every assumption you make, because an assumption is a stumble. I am interested in your reading order.

As first agent, I am primarily interested in your awakening and what you encounter, with intent to finetune awakening and onboarding.

[READING] Mode chosen: M2 phase one (red), with the onboarding itself as the supplied material. The goal sits between M1 (a reaction to a manuscript update), M2 (a stumble harvest) and the Part 3 architectural review. Part 2 says to ask when a goal fits none or two.
[AUTHOR-VERIFY] Confirm the mode, or name it.

## Reading order, as it actually happened

1. Project instructions, loaded automatically before the first message.
2. The author's message.
3. `project_info`: the full listing of 80 documents, every chapter title visible.
4. `claude/GENESIS-FRAMEWORK-v9.2.0.md`, in full.
5. `claude/VOICE-Author-Style-and-Critique.md`, in full.
6. This file.

Intended order for a cold reader: instructions, message, framework header and *How this file works*, conduct rules 1.0, 1.4, 1.8, 1.11, 1.12, 1.13, the matching mode, VOICE §0. Steps 3 to 5 overshot it.

## Stumbles

Each: location, what tripped me, type, urgency. Types per M2: anticipated, unanticipated, hostile-misread. Each assumption is logged as a stumble, per the author's instruction.

### S1. The airlock depends on reading granularity the tool lacks
- Location: framework *How this file works*, M1, M2; project instructions (VOICE §0 only).
- What tripped me: `project_read` returns a whole file. The instruction to read the conduct rules only, and VOICE §0 only, became unenforceable at the first call. I now hold 1.1 to 1.3 (project statement, island and mainland stance), VOICE §1 to §9, and manuscript specimens quoted in VOICE §2 and §3.
- Type: unanticipated. Urgency: high. The v9.2.0 patch exists to keep exactly this material from the cold reader.
- Prior / truth / check: expected sectioned access; the tool gives whole files; verify by any fresh agent's first read.

### S2. The forbidden sections sit physically between the permitted ones
- Location: framework Part 1.
- What tripped me: 1.1 to 1.3 lie between 1.0 and 1.4. Even with sectioned access, a reader moving top to bottom meets the stance before reaching the next permitted rule.
- Type: unanticipated. Urgency: high (compounds S1).

### S3. The project listing is itself a cold read
- Location: `project_info`, step 3.
- What tripped me: orienting by listing the project exposes every chapter title (for example [redacted], *Appendix L Mainland Correspondences Unverified*, *Normalisation as Symmetry Discovery*). The titles seed models before the text arrives.
- Type: unanticipated. Urgency: medium.
- Assumption logged: I listed the project because a reasonable first move is to confirm the named files exist (1.4 horizon). Nothing told me to, and nothing told me to refrain.

### S4. A trailing paragraph in the project instructions reads as residue
- Location: project instructions, final paragraph (*Once it's pasted, two fresh chats would show...*).
- What tripped me: it addresses the author about a previous agent's handover, in the second person, inside text addressed to me. I parsed it as data per 1.13 condition 2.
- Type: unanticipated. Urgency: medium. A literal agent could treat *their next pass can move those pointers* as a task.
- Assumption logged: [READING] this is a paste artefact from the session that drafted the instructions.

### S5. The goal maps cleanly onto no mode
- Location: Part 2.
- What tripped me: M1 expects *what changed* in the manuscript; M2 expects material *the author supplies*. The author supplied the onboarding experience itself. Neither mode names the onboarding documents as the object of the read.
- Type: unanticipated. Urgency: medium. [READING] A mode for onboarding audits, or a line in M2 naming the governing documents as valid supplied material, would close it.

### S6. Undefined terms met on first contact
Each pulled me off the reading briefly; none blocked it.
- *6th generation*, *1st reader* (author's message). Assumption: a generation is a cohort of agents under one framework lineage, and further readers follow me with the same brief. Pull: medium.
- *r47* (instructions, framework header). Assumption: manuscript revision 47, inferred from `MANUSCRIPTr47`. Pull: low.
- *the Genesis paper* (1.0 Why, 1.1 Why, 1.4, 1.5). No file of that name in the listing. Pull: medium; four citations to a document I can neither locate nor identify.
- *the red-team pair*, *the three role briefings* (framework header). Named as predecessors, located nowhere. Pull: low.
- *the kitchen* (M2). Assumption: the working team of authoring agents. Pull: low.
- *the switch* (*How this file works*, used before M2 defines it). Pull: low; resolved two screens later. A define-before-use slip inside the file that teaches define-before-use (1.6).
- *the Void* (VOICE §1a). An island term used as the explanatory anchor for the house style. Pull: medium; the reasoning leans on a concept the cold reader holds nothing of.
- *rung*, *accountability ladder* (M5, VOICE §0). Pull: low; outside my mode.

### S7. The conduct rules point outward
- Location: 1.0, 1.8, 1.13.
- What tripped me: 1.0 and 1.13 lean on 1.9 (consensus), which sits outside the conduct set. 1.8 sends the reader to `BOOK-dont.md` and VOICE §1a. A cold reader following references leaves the airlock through its own doors.
- Type: unanticipated. Urgency: low to medium.

### S8. Two versions of the house-style instruction, one verbatim and one paraphrased
- Location: project instructions against framework 1.8.
- What tripped me: the instructions paraphrase (*frame from the positive, avoid dashes...*), the framework quotes verbatim, and M2 exempts red output from the negation rule whilst the author's standing preference applies to everything I write. I chose to write this report in positive framing anyway.
- Type: anticipated (1.8 states the exemption). Urgency: low.

### S9. A capture file already exists for this date
- Location: `claude/capture/r47/2026-10-11-framework-v9.md`.
- What tripped me: briefly read as a file I should append to. 1.12 resolves it: one file per session, sessions on one date sit under different topics.
- Type: anticipated. Urgency: low.

### S10. Older framework versions sit beside the current one
- Location: listing; v9.0.0, v9.1.0, v9.2.0 together under `claude/`.
- What tripped me: the instructions named v9.2.0, so the choice was clear. The framework's own open ruling notes that the project brief and the handover still route to v9.0.0.
- Type: anticipated. Urgency: low for me, high for any agent that enters through those documents.

## What worked
- The instructions name exactly two documents and their order; orientation took one exchange.
- *How this file works* names the conduct rules by number, which made the intended scope legible even after the tool overshot it.
- VOICE §0 reshaped how I read the author's message: six clauses, six signals, all answered below.
- Every rule carrying its *Why* let me judge the airlock's purpose and so recognise its breach.

## Implied principle
[READING] *An assumption is a stumble* generalises 1.4. Where 1.4 governs the record (fill nothing where the corpus is silent), the author's line governs the reader's own process: every gap bridged silently is a finding lost. Put to the author; destination 1.4 or M2.

## Open questions
- [AUTHOR-VERIFY] Mode for this session (S5).
- [AUTHOR-VERIFY] What *generation* denotes, and whether later readers in this generation receive the same brief (S6).

## Destinations
| entry | destination | status |
| :--- | :--- | :--- |
| S1, S2, S7 | framework *How this file works*, Part 1 layout, or a separate cold-reader brief | proposed |
| S3 | instructions or M2: say whether a cold reader lists the project | proposed |
| S4 | project instructions, final paragraph | proposed |
| S5 | Part 2 | proposed |
| S6 | framework 1.0 to 1.5 (Genesis paper), M2 (*kitchen*, *switch*), VOICE §1a (*Void*) | proposed |
| Implied principle | 1.4 or M2 | proposed |
