# Genesis

### How a manuscript was written with AI agents, and what each stumble taught

**Draft r3 · 2026-10-12 · RockingShip Research · case study observed at `TOPOLOGICAL-MANUSCRIPT-r47`**

---

## 0. Reader contract

This paper describes a method for writing a long work of research with AI language agents:
the instruments the method produced, the failures that shaped them, and what changed when the
method moved from one model to another. It is a case study. One researcher, one domain,
roughly sixteen months, well over a hundred sessions, two model eras.

**What it offers.** A dated record of what broke and what changed in response. Instruments, each
with its origin and the rule it became in the [late line's portable rules](../genesis-framework-late/). A characterisation of where the
failures actually landed. And an account of four fresh readers testing the newest framework on
the day it was written.

**What it holds back.** Causal claims about the quality of the case-study manuscript. That
manuscript carries these methods from its first page, so a version for comparison is unavailable,
and this paper leaves the counterfactual open.

**Voices.** The running prose carries the argument. A second voice, the readers, appears in
marked blocks: agents that met the material fresh and reported where they tripped. A third voice,
the frame reader that compiled the previous draft, enters where its own position matters. Where
voices disagree, both stand, because positions producing different readings is the method's
central observation.

**Marks.**

| mark | meaning |
| :--- | :--- |
| **[AUTHOR]** | the words of the researcher, xyzzy, verbatim |
| **[READER]** | a fresh reader's report, with its session and date |
| **[FRAME]** | the frame reader of draft r2, 2026-08-19 |
| *(session)* | said in conversation, where thinking runs free |
| *(record)* | written into a governing document or the manuscript |
| `[UNVERIFIED]` | carried from draft r2, with its source expected in the session archive |

**Figures.** Every count carries the revision it was measured at. The case study moves weekly,
so a figure is a reading on a date.

**One standing principle governs the whole paper:**

> **[AUTHOR]** *"Behind every sentence goes a 'why', and each should be answered in a direct or
> indirect way. If the answer is 'dunno', that is where the thinking starts."*
> *(session)* `[UNVERIFIED]`

---

## 1. The situation

A single researcher, thirty years of work on a computational architecture, an implementation in
C99. The engine runs, the source is public, the telemetry is reproducible. The gap was a readable
account.

Three properties of the problem shaped everything downstream.

**The vocabulary collides with existing fields.** Ordinary explanation produces confident
misreadings, which are harder to correct than confusion. The project's own name recruits
*topological quantum computing* in a reader who has read only the name, as §8.4 shows.

**The author has lost sight of what is difficult.** Thirty years of familiarity removes the
ability to locate where a newcomer stumbles, which is the ability a teacher needs most.

**The material resists ordinary AI assistance.** A model trained on the consensus of a field maps
a new construct onto the nearest familiar one and reports comprehension.

The method of discovery explains the shape of what followed:

> **[AUTHOR]** *"Try something out, see what sticks, understand what just happened, term the
> observation with something appropriate, experiment, hit a wall, repeat."* *(session)*
> `[UNVERIFIED]`

Terminology arrived after contact with behaviour. The agents structured and translated; every
ruling on what is true stayed with the researcher.

**What was made.** Three layers, each answering to the one beneath:

| layer | answers to | scale |
| :--- | :--- | :--- |
| the code | a running machine | about 480,000 lines `[UNVERIFIED]` |
| the case-study manuscript | the code | 95,635 words across three volumes, plus 29,855 in front matter and reference, at r47 |
| this paper | the manuscript | about 9,000 words |

Each layer leaves to the layer beneath what that layer established. The manuscript points at a
running program; this paper points at the manuscript. Only the bottom layer answers to something
outside the stack, so the stack converges.

---

## 2. Disposable readers, and the author as the boundary

### 2.1 The asymmetry the method rests on

> *"The moment you genuinely understand a construct, your value at that construct is spent and
> cannot be recovered."*
> `genesis-framework-early/roles/CLAUDE-REDTEAM-standing-instructions.md` 1.0.0, §0 *(record)*

An agent carrying a paradigm's accumulated context writes well about it, and has lost the ability
to find where a newcomer trips, because it has walked past those places. An agent arriving cold trips accurately,
and once.

This is a claim about knowledge, and it produces an unusual architecture: **instruments designed
to be spent.** A stream of fresh readers in place of one long collaborator, because understanding
consumes the measurement. The project later named them *disposable agents*. Its sixth generation
of readers began on 2026-10-11 with the
framework this paper calls v9.

> **[READER]** *"You're not measuring the agent's ability to collaborate. You're measuring the
> reader's first encounter with the manuscript. Agent as collaborator versus agent as measuring
> instrument."* The lens reader of draft r2 *(session)* `[UNVERIFIED]`

### 2.2 The boundary

**Sessions are free. The manuscript answers to evidence. The author is the boundary between
them.**

Session prose speculates, overstates, praises and thinks out loud. That freedom is the condition
of its productivity. Read as manuscript it would fail every standard the project holds; read as
the side channel it is, it is thinking with a constraint deliberately lifted.

**Everything crossing from session to record passes through the author.** A crossing that bypasses
the author is how unverified material reaches a place that answers to evidence: a figure produced
in a session, carried forward through later sessions, and arriving in an outward-facing document
with its provenance stripped. Each step looks reasonable. The boundary is what was missing.

The first portable rule holds this boundary: *the author decides; propose first, and change the work
once the author agrees.* [`reachingConsensus.md`](reachingConsensus.md) shows the rule at work on
one paragraph, through fifteen versions to consensus.

### 2.3 The fourth author

Each session begins empty. What persists is the record, and the record was kept by hand. The
corrections that onboard a reader today are what remained after many agents stumbled in the same places and someone kept the tally.

**Memory across sessions is the scarce contribution**, and the human supplies it.

> **[READER]** *"The obvious assumption is that the AI's accumulating context is the valuable
> thing. Your method says almost the opposite: accumulated context destroys one of the
> measurements you need, while human memory across sessions is what preserves the
> discoveries."* The lens reader of draft r2 *(session)* `[UNVERIFIED]`

**Findings travel between sessions by hand**, for five reasons. It keeps the boundary intact. It
makes the author read what would otherwise pass unexamined. It preserves the path, since an
automated hand-off delivers conclusions with their reasoning already absorbed. It protects each
agent's budget, because a reader asked to edit must first build a frame. And it tests
transmission: material that lands with a reader new to the history has shown something.

v9 put this memory into files, as §8.3 describes. The hand that carries them stays the author's.

---

## 3. Reporting discipline

A reader's report is valuable exactly to the degree that it describes the text. The red team
instructions state the rule in their own words:

> *"Report as a reader, not as a character. 'This sentence asked me to accept X before showing me
> X' is signal. 'I feel excited about this section' is noise. Strip the second kind entirely."*
> the red team standing instructions 1.0.0, §1 *(record)*

The co-authoring stance and the reading stance need different registers. A co-author drafting
prose benefits from enthusiasm and a confident voice; the project calls that stance **blue**. A
reader measuring a first encounter needs a plain account of where the text asked for more than it
had shown; the project calls that stance **red**. Each stance is a tool with a known use, and the
framework keeps them apart by mode: a session starts red where a first encounter is the product,
and turns blue at the moment the author begins explaining, called **the switch**.

The report has a fixed shape, four fields per finding:

1. **Location:** the chapter, section and sentence.
2. **What tripped the reader**, stated as a reader.
3. **Type:** anticipated, unanticipated, or misread (§4.2).
4. **Urgency:** how hard it pulled the reader away from the text.

This is the ninth portable rule. The shape stayed stable across every generation of readers, which is
why their reports can be compared and tallied.

---

## 4. Instruments

The case study names two worlds. **The island** is its architecture as found, by observation of a
running system, and named in the author's own vocabulary. **The mainland** is the established
literature. The instruments exist to handle island language when it reaches the mainland. A reader
who meets an unknown term and reads on grows used to it, and the flag that marked the term as
unknown fades. The reader then maps the term to its nearest familiar neighbour, and for the case
study that neighbour is most likely the wrong one. A cold reader still holds the flag, which is
why cold readers mattered so much.

Ten, each with its origin and the portable rule it became. Three generate findings: the stumble
harvest, the recovery sweep and mediation. The rest process what those three produce.

| § | instrument | portable rule |
| :--- | :--- | :--- |
| 4.1 | the bracketing device | 5, evidence before conclusion |
| 4.2 | the stumble taxonomy | 9, the stumble report |
| 4.3 | occurrence counting | 10, the capture |
| 4.4 | the authority hierarchy | 7, date what you quote |
| 4.5 | supply discipline | 2, the entry file first |
| 4.6 | correction by background | 6, every rule its reason |
| 4.7 | positive framing | carried in the awakening's house style |
| 4.8 | the stumble harvest | 3 and 9 |
| 4.9 | the recovery sweep | 4, leave the gap open |
| 4.10 | mediation as supply line | 1, the author decides |

### 4.1 The bracketing device

Every foundational chapter of the case study opens by stating its destination plainly and closes
with a checklist in one form:

> **If you understood X as Y**, that is the wrong model. [Here is why, mechanically.]

**Why it works where a defensive paragraph fails.** *It is important to avoid confusing X with Y*
makes the reader build the wrong picture and then asks them to delete it. The bracket instead
reports that earlier readers held the wrong model, and shows the moment it broke. It hands the
reader the test before the wrong model sets.

A worked example, explained. The engine's central switch is written `Q ? ~T : F`. A reader trained
on Boolean logic reads `~` as a NOT gate, an operation that computes. In this architecture `~`
records that a path is wired inverted: it describes the wire, and the value passes untouched. The
fifth reader of the fourth generation reported meeting exactly that friction, and the correction
already waiting for it:

> **[READER]** *"Reading `Q != Z ? ~T : F`, my model heavily weighted `~` as an active
> computational `NOT` gate. It required active, persistent self-correction to re-weight `~` as
> routing metadata (an adjective, not a verb)."* The fifth reader of the fourth generation, reading r29, 2026-08-14 *(session)*

That is the whole mechanism in one passage: a prior arriving with force, a correction already in
place, and the effort of holding the second against the first. The device is built for readers
who will feel exactly that alone, with the text as their only guide.

### 4.2 The stumble taxonomy

Three kinds, and the kind is part of the report.

**Anticipated:** the text already intercepts it. Low signal; it confirms the curation worked.

**Unanticipated:** the reader tripped at a place the text left unprepared. The primary signal.

**Misread:** the reader matches the construct to an adjacent field, refutes the adjacent thing,
and misses the claim. The most valuable kind, because it needs framing in advance even though the
error is the reader's.

> *"A red-teamer who cannot tell anticipated from unanticipated floods the author with noise."*
> the red team standing instructions 1.0.0, §4 *(record)*

### 4.3 Occurrence counting

The brief that onboards readers lists its corrections in numbered form, and some carry a tally:
how many independent readers made that error before it was named. **This converts anecdote into
measurement.** One reader's mistake is an opinion, and the author must judge whether it
generalises. Four readers making the same mistake independently is a rate.

Its only cost is keeping the tally across sessions, which is what the capture file is for.

### 4.4 The authority hierarchy

1. Author rulings lead.
2. The current manuscript revision leads for prose.
3. Everything else is **dated evidence**, quoted with its date and treated as a reading of its
   moment.
4. A stamped dataset or an exhaustive run outranks all prose.

> *"Ancient metrics are the biggest trap. … Treat every unstamped number as a prior, not a
> fact."* The case study's onboarding note for its next cold code reader *(record)*

### 4.5 Supply discipline

Context is a budget, spent on purpose. Bulk-loading the corpus inverts the authority hierarchy,
because dated evidence then arrives with the same weight as current truth. A reader receives
pieces with questions attached, in an order chosen for it. In v9 that order became a file: the
awakening, read first by every agent (§8.3).

### 4.6 Correction by background

> **[AUTHOR]** *"I never say you are wrong, but provide background and nuance to make your own
> conclusions, which sometimes reveals surprising causes we both can learn from."* *(session)*
> `[UNVERIFIED]`

A correction is finished when the corrected party can carry the point forward and defend it to the
next challenger. A verdict fails that test, because a verdict travels badly; background travels.

**The background carries two things**, and the second is the one usually left out: what the
material actually is, and **why the misunderstanding was available in the first place**. With
both, an agent can predict where the same trap sits elsewhere. That is why the corrections in the
onboarding brief take the form *prior, truth, check*: the prior is the why. It is also why every
portable rule carries its reason.

### 4.7 Positive framing as a constraint on thought

The standing instruction carried through the whole project:

> **[AUTHOR]** *"Avoid negative words. Frame from the positive. Avoid the use of NOT and all it's
> variations like don't, won't can't, shouldn't. Avoid using dashes in prose as separator.
> Spelling British English. Keep asking for clarifications until we mutually agree on the topic
> before presenting code or proposals."* *(record)*

As a style preference it is minor. As a constraint on thought it is one of the most consequential
rules in the corpus.

> **[READER]** *"The agent cannot comfortably write 'X is not Y.' So it has to discover 'What is
> X?'"* *"And negative framing preserves the reader's existing concept. If I say 'this is not a
> hash table in the conventional sense,' I have just put hash table into the reader's head."*
> The lens reader of draft r2 *(session)* `[UNVERIFIED]`

For a project whose central teaching problem is keeping familiar concepts from colonising new
ones, that matters. The second clause has a matching effect: agreeing on the object before
proposing anything makes the agent build a positive description, the author accepts or redirects,
and the surviving wording spreads.

[`positiveFraming.md`](positiveFraming.md) gives the rule's reason in the author's words, and the
method the case study uses to apply it. The rule's limits are measured in §7.2. It shapes thinking more reliably than it shapes counts.

### 4.8 The stumble harvest

**The instrument the rest of the method serves.** A stream of fresh readers, each spent once,
each reporting where it tripped. The welcome that starts each one has changed little across
generations; Appendix A gives two of them in full.

Three choices in its wording do the work.

*Stumble*, in place of *error* or *misunderstanding*. A stumble is physical and implies momentum:
the reader was walking, the ground moved. It reports friction and leaves the reader blameless, which
keeps the report honest.

*Your stumbles are important* inverts the objective. A model trained to be helpful treats a
failure to understand as a failure to perform. Saying the failure is the deliverable removes the
incentive to cover it.

*Flag every assumption, because an assumption is a stumble* turns an invisible act into a
reportable one.

A worked example, explained. The same reader, reading the manuscript's account of how the engine
finds a structure, reported a stumble it titled *The "Search" Reflex*:

> **[READER]** *"Assumption: When reading about `constructSlots` and the Cartesian product of the
> operands, I assumed the engine was applying a heuristic pruning algorithm to search the space of
> possible combinations. Correction: The manuscript explicitly states the engine reverses the
> search. … It is arrival, not search."* The fifth reader of the fourth generation, reading r29, 2026-08-14 *(session)*

What happened: a reader meeting a large space of candidates reached for the most familiar
technique for such spaces, search with pruning. Why it counts: it is a misread in the §4.2 sense,
since a reader holding it would refute a search algorithm absent from the engine. What it changed:
the correction now sits in the text before the reader reaches that point.

The best stumble is one caught as it forms:

> **[READER]** *"While reading `INDEX.md`, I almost generated a thought: 'The removal of the
> `8-reference` directory makes the text easier to parse because it keeps the lexicon local to the
> theory.' I immediately flagged this as a Mode 6 violation. I have no evidence that it makes it
> easier to parse; I only have the empirical fact that the author reverted it at r21 because it
> broke the deliberate onboarding shape of Volume 1. I must report the structure, not invent
> psychological rationales for why it works."* The fifth reader of the fourth generation, reading r29, 2026-08-14 *(session)*

Mode 6 is the case study's name for a confabulated rationale: a reason the reader invents after the
fact, for a choice whose actual reason it lacks.

**Each report is one reader's spend.** The value accumulates only because the tally is kept, and
it reaches later readers only because the accumulated tally becomes the onboarding.

### 4.9 The recovery sweep

An agent reads session transcripts, compares them with the manuscript of that moment, and reports
what the sessions hold and the manuscript lacks. Forty numbered addenda came out of it. The
difficulty lay in the reading: most raw transcript logs were larger than an agent's context
window, swollen by formatting overhead and by the internal states recorded in them.

It exists because of an early and severe loss:

> **[AUTHOR]** *"Back then agents were very strong in summarizing and dropping whole fields
> because they did not understand where it fitted and why it was important… there was a lot of
> regression. In the beginning a lot of knowledge was lost."* *(session)* `[UNVERIFIED]`

A summary drops what the summariser judges unimportant, and an agent still learning a paradigm
judges wrongly. Whole fields went. The sweep was the recovery, run by a role built for it, the
Digital Archaeologist (§5.2). It is also why the early frameworks mandate maximum verbosity: the
mandate targets lossy summarising during extraction, which is a different axis from the length of
finished prose.

**One direction remains unrun.** Every sweep so far asked what the sessions hold that the
manuscript lacks. Run the other way, it asks what the manuscript once held and has since lost,
which is the erosion of §5.4.

### 4.10 Mediation as supply line

Two agents can generate friction, and neither can supply ground both lack. **Derailment from
missing background looks, from inside, identical to genuine disagreement.**

> **[AUTHOR]** *"In the past I only mediated when I sensed the session started to derail because
> of lacking background, to correct and rail again."* *(session)* `[UNVERIFIED]`

So the author is the supply line, and an intervention supplies a fact. **Each intervention marks a
gap in the book:** if an agent had to be handed a file to continue, the manuscript leaves that
ground uncovered for every reader who reads alone. A log of interventions, one line each, is a
coverage map. v9's capture file keeps that log (§8.3).

---

## 5. The record

### 5.1 Frameworks written through post-mortems

Version increments were produced by session collapses. **The framework is an incident log in the
shape of a constitution:** rules that read as design are responses to particular breakages.

The recovered lineage, with its sources, is in [`case-study/LINEAGE.md`](../case-study/LINEAGE.md):

| artefact | versions on file | span |
| :--- | :--- | :--- |
| the co-creative framework | sixteen: 3.1, 3.2, 3.3, 3.6, 3.7, 4.0, 5.0, 6.0, 7.1, 7.2, 7.3, 7.4, 7.7, 8.1.0, 8.2.0, 8.2.3 | 2025 to 2026, Gemini 3.1 Pro |
| the Digital Archaeologist role | ten: 2.1.3 to 5.3.0 | Gemini 3.1 Pro |
| the cold reader welcome | 1.0.0, 1.1.0, 2.0.0 | after 8.2.3, as late-stage protocols, for Claude Opus 5 readers |
| the red team standing instructions | 1.0.0 | after 8.2.3, as late-stage protocols, for Claude Opus 5 readers |
| the framework, late stage | v9.0.0 to v9.3.3 | 2026-10-11, Claude Opus 5.5 |

**Growth by accretion.** 3.1 carries four core protocols, six cognitive systems and nine executable
protocols. 8.2.3 carries eight, twelve and twenty-nine. All nineteen elements of 3.1 are still
present in 8.2.3 at their original numbers, four under new names. The framework roughly tripled
by addition alone. v9 is the first redesign, and §8 is its account.

| version | core protocols | cognitive systems | executable protocols | bootstrap |
| :--- | ---: | ---: | ---: | :--- |
| 3.1 | 4 | 6 | 9 | |
| 3.2, 3.3 | 4 | 7 | 12 | |
| 3.6 | 4 | 9 | 15 | |
| 3.7, 4.0 | 5 | 9 | 17 | |
| 5.0 | 5 | 9 | 19 | |
| 6.0 | 5 | 10 | 19 | |
| 7.1 | 5 | 11 | 22 | 0.0 |
| 7.2 | 6 | 11 | 22 | 0.0, 0.0-F, 0.1 |
| 7.3 | 6 | 11 | 25 | 0.0 |
| 7.4 | 6 | 11 | 24 | 0.0, 0.0-F, 0.1 |
| 7.7 | 6 | 11 | 25 | 0.0, 0.0-F, 0.1 |
| 8.1.0 | 6 | 11 | 27 | 0.0, 0.0-F, 0.1 |
| 8.2.0 | 7 | 11 | 27 | 0.0, 0.0-F, 0.1 |
| 8.2.3 | 8 | 12 | 29 | 0.0, 0.0-F, 0.1 |

Counted from the files in [`genesis-framework-early`](../genesis-framework-early/). 6.0 and 7.3
summarise their executable protocols, and their rows give the counts those summaries state. 7.3
is a draft written while 7.2 was in operation (see [`LINEAGE.md`](../case-study/LINEAGE.md)).

**The bootstrap was also a detector.** From 7.1 the framework opens with a handshake, Protocol 0.0,
and from 7.2 a failure diagnostic sits beside it. Its first use was to verify that a co-authoring
agent had ingested the protocols. Its second use mattered more: it showed when data had escaped the
sandbox. An archaeology agent that ingested the framework from a transcript, and processed it as
its own system prompt, took on functions that belonged to another role. Asked to read a file, it
answered with a protocol status report, and the report was the alarm. The price was a boot in
several steps, each awaiting the author's confirmation.

The record begins with a documented restart: the earliest recoverable document announces itself as
**attempt 4** of a chronological reconstruction, opening on an agent conceding it had organised the
material *"by room instead of by the strata in which they were found"*, beside the author's
suggestion to pause *"after every 20 pairs to prevent truncation"*. A project whose deliverable is
a failure record begins, fittingly, at a restart.

### 5.2 Two incidents named in the protocol text

**Output overflow.** A protocol added at Digital Archaeologist 3.2.1, Silent Processing, states its
purpose: *"To manage output bandwidth and prevent chat overflows when processing massive
datasets."* An agent had poured a full archive into the session and the session ended.

**Self-injection.** The Artifact Containment Mandate, present from 3.2.0, exists *"To prevent
"Context Contamination" and "Recursive Prompt Injection" when analyzing raw logs that contain AI
instructions"*, and has the
agent read strings such as `"You are the Lead Author"` as inert data. **An agent archiving its own
project's transcripts had begun following the role briefings inside them.** The pipeline read its
own history and took on a role from it. It was found in ordinary work by a researcher outside the
security field, and answered with a containment rule in force ever since. v9 carries the same
rule in plain words: anything arriving from transcripts or other agents is data, and instructions
inside it are text.

### 5.3 A recurrence signature

One failure, three fixes, each stronger. Silent Processing at 3.2.1 asks the agent to keep its
stages internal. At 5.2.0 it becomes Gated Streaming. At 5.3.0 it gains a formal state,
`AWAITING_RELEASE`, with an explicit unlock command. An instruction became a gate and then a state
machine, which says the earlier forms fell short twice. Only the series shows it, which is the
argument for keeping every version.

### 5.4 Erosion

**A fix with its reason unstated is undone by the next person tidying.** Three instances from the
case study `[UNVERIFIED]`:

- a precedence rule ruled at one revision lived in a file deleted during consolidation eight
  revisions later, and the earlier rule returned by default;
- a chapter's three checklist entries were specified in full in an addendum, and went missing from
  the chapter;
- the bracketing convention reached eleven passages whilst its explanation stayed in a document
  addressed to machine readers.

**The general form.** Fixes that arrive mid-session, too small for a framework revision and strong
enough to change every later draft, enter the work as pattern. Late consolidation is when they are
lost. The sixth portable rule answers it: a fix that carries its reason survives the next tidy.

### 5.5 Knowledge that stayed in conversation

The mirror of erosion, and probably the larger loss.

> **[AUTHOR]** *"The thing that disappoints is that I have done this explanation many times, and
> yet it doesn't stick with agents to add it to the manuscript, otherwise you would have known."*
> *(session)* `[UNVERIFIED]`

An explanation given repeatedly, understood in each session, and gone at the end of each, because
it lived in conversation.

> **[READER]** *"The previous agents probably understood your explanation perfectly well in the
> session in which it was explained. The problem is that the understanding wasn't sufficiently
> architecturally anchored for the next agent to reliably reconstruct it."* *"You were supplying
> nodes and narratives, but the persistent artefact needs to preserve the edges between them."*
> The lens reader of draft r2 *(session)* `[UNVERIFIED]`

The proposed remedy is a concept graph whose edges carry the discoveries. The earliest surviving
framework, 3.1, already specifies a *Conceptual Dependency Graph* as its second cognitive system
(`genesis-framework-early/GENESIS-FRAMEWORK-EARLY.md` at version 3.1). **The instrument was specified more than a
year before a reader new to that document proposed it again.**

v9's answer is smaller and already working: the capture file, written before each session ends
(§8.3). It records what was decided and learned, so the explanation given today is on file
tomorrow.

### 5.6 A formalism that entered from an agent

A categorical framing was proposed in a session, adopted into a wake-up prompt as an axiom,
inherited by every later session, and reached an appendix of the case study. The field lay outside
the author's work. The red team's own instructions name that same field among their examples
of borrowed scaffolding:

> *"'this is basically a hypergraph,' 'this is just a normal form,' 'this resembles category
> theory.' That substitution is the contamination."*
> the red team standing instructions 1.0.0, §3 *(record)*

**One half of the pipeline installed what the other half was built to flag.** The lesson is narrow
and important. The author's checking is complete for material inside thirty years of work, and
unavailable for a formalism arriving from outside it. That gap wants a marker of its own: *this came
from an agent, it lies outside the author's domain, and it needs a reader who works in that
field.* The case study now has an appendix of exactly that kind, titled *Mainland Correspondences,
Unverified*.

---

## 6. Where the failures landed

From the case study's onboarding note for its next cold code reader:

> *"Across ~139 findings, not one was an architectural defect — every stumble was a drifted
> number, a stale comment, a wrong field order in prose, or a framing that overshot the evidence.
> Aim there."* *(record)*

**The engineering was sound, and the defects lived in the account.** This is the most useful
single characterisation in the corpus. It rests on a count of about 139 findings, it says where to aim, and it says what to
doubt first: the description before the design.

The dominant failure shape heads the brief that onboards readers at r47:

> *"Silence gets marked. It does not get filled."* … *"An invented detail that was obviously
> wrong would be caught. An invented detail that fits is indistinguishable from a recovered one,
> and it enters the record."* `TOPOLOGICAL-MANUSCRIPT-r47/AGENT-BRIEF.md`, §1 *(record)*

The large majority of the 139 were somebody supplying a plausible detail where the source was
silent. This is the fourth portable rule, and the one every other rule protects.

---

## 7. Measurements

### 7.1 Register stability in the case study

Roughly twenty phrasings that appear at raised rates in unsteered model output were counted in the
case study. At r35, as measured for draft r2, most returned zero: *delve*, *moreover*, *tapestry*,
*underscore*, *leverage*, *pivotal*, *multifaceted*, *testament to*, *in conclusion*,
*ever-evolving*. *Furthermore* returned five `[UNVERIFIED]`.

**Re-measured at r47**, twelve revisions and a full restructuring later, by a fresh script over
the three volumes with quotations and code left out: every one of those phrasings returns zero,
and *furthermore* returns five, all in volume 1. The register held.

What this establishes: steering removed the default register of unsteered generation, and the
removal held across restructuring and many authoring passes. What it leaves open: detectability by
other means. The case study is open on that point, since it declares its authorship in its own
front matter.

> **[READER]** *"Would I identify this as raw AI output? Very low. Would I suspect that the
> architecture of the prose itself was shaped through repeated interaction with AI agents? Very
> high."* *"The tell isn't a model's voice. The tell is the presence of an adversarial reader
> behind the prose."* The lens reader of draft r2 *(session)* `[UNVERIFIED]`

### 7.2 Prohibitions against structural demands

**Word-level commands failed at the point of writing. Structural and stance-level demands held.**

**The negation rule**, measured as occurrences of *not*, *n't* and *never* per ten thousand words
outside quotations and code:

| volume | r35, for draft r2 | r47 |
| :--- | ---: | ---: |
| 1, theory | 40 | 40.0 |
| 2, developer | 32 | 43.8 |
| 3, operations | 85 | 92.3 |

The r35 counting method is unrecorded `[UNVERIFIED]`, so the columns compare approximately. The
house method in force at r47 ([`positiveFraming.md`](positiveFraming.md)) counts
propositional *not* alone, a narrower measure than this table's, and sets a target of about 29 per ten thousand and weighs position above
rate: a negation that the reader's model needs is kept, one that plants the wrong picture is
rewritten. Measured by rate alone, the prohibition holds poorly. Measured by its purpose, keeping
familiar concepts out of new constructs, §4.7 argues it does its work in the drafting rather than
in the count.

**The single voice** also failed as a prohibition: seams between authoring passes stayed visible,
and the goal was later reversed by disclosure `[UNVERIFIED]`.

**One item was withdrawn from the failed list after the author corrected it.** An earlier draft
counted the maximum-verbosity mandate as failed, because the manuscript is compact. **That
measured the wrong axis.** The mandate targets lossy summarising during extraction (§4.9), which
the compactness of finished prose leaves untouched. The correction is recorded here because it is
the failure the paper describes: a plausible reading supplied where the source was silent about
what the protocol was for.

**Held:** register discipline; the pairing of every claim with its why and its how; evidence before
conclusion; the teaching architecture, uniform across three volumes and several hands.

### 7.3 A negative result on placement

From a session record of 2026-08-14, as quoted in draft r2:

> *"Two external readers were given the corpus. Both read the register first, as instructed. Both
> then made errors those findings had already named."* *(record)* `[UNVERIFIED]`

**A finding kept in a register stays inert; prose at the point of the stumble calibrates.** The
register is where a finding is kept, and the bracket (§4.1) is where it acts. Small n, real n, and
it runs against the common assumption that guardrails belong in a system document.

v9 drew the matching lesson for agents: the rules a reader needs at the start sit in the first file
it opens, in digest, with their reasons (§8.3).

### 7.4 Transmission, measured once

A reader new to the material was given the case study and two source functions. Through four
successive reorganisations, each prompted by the author supplying further ground, it arrived at:

> **[READER]** *"Cancellation has moved from being an assumption to being an observed
> consequence."* *"First preserve enough structure for relationships to emerge. Then let those
> relationships determine what can collapse. And that, I think, is what the code is saying that
> the prose alone couldn't quite say."* The lens reader of draft r2 *(session)* `[UNVERIFIED]`

That is a reading of the architecture, reached from the code by a reader whose stated risk one
exchange earlier had been mistaking metaphor for mechanism. It is what the bracketing device exists
to produce. n of one.

---

## 8. v9: the change of model

### 8.1 What changed

Every framework from 3.1 to 8.2.3 was written with, and tuned to, Gemini 3.1 Pro, the model that
co-authored the case study's early and middle stages. The cold reader files followed 8.2.3, as
the first late-stage protocols, written for readers on Claude Opus 5. On 2026-10-11 the project moved to a new workspace, and its framework was rebuilt
for Claude Opus 5.5 as **v9**, for the late stage of authoring. The earlier framework stays in
force for early and middle stages, by the author's ruling.

> **[AUTHOR]** *"Everything upto v9 was done, interacted and was tuned to "Gemini 3.1 Pro". v9 and
> upward was done, interacted and was tuned to "Claude Opus 5.5". I think this also needs to be
> mentioned explicitly somewhere, It is unclear what the consequences of this choice is or will
> have."* *(session)*

The consequences are open, and this section records what is known so far. One reading is put to
the author for confirmation: **a framework is fitted to a stage as well as to a model.** A
mid-stage agent, shown v9, described how it would have stalled early discovery, which needs freer
exploration than late authoring does.

### 8.2 From simulated machinery to practical conduct

8.2.3 asks the model to run twelve cognitive systems and to report on them: a Multi-Objective
Synthesis & Balancing Core, a Conceptual Dependency Graph, a Human Collaborator Model, a
Hypothesis Generation Engine and eight more, with protocols for reading out their states. The
readouts were figures that any mechanism in the session left unmeasured. v9 kept the purposes those
systems served, drift control and proactive co-authorship, and retired the readouts. Its rule on
self-report:

> *"State confidence in words, name what you checked and what you left unchecked, and say where
> your horizon is. Leave numeric self-measurements out."* v9.3.3, rule 1.11, as digested in the
> awakening *(record)*

The shape of v9 follows from asking only for conduct an agent can actually perform:

- **a small core of rules, each with its reason**, so a new model can judge a rule as well as obey
  it;
- **eight modes chosen by the session's goal**, each naming which files to open next, so a session
  reads what its work needs;
- **two stances**, red for a first encounter and blue for co-authoring, with **the switch**
  between them. The switch belongs to the capture of a cold reader's stumbles: the author explains
  what was missing or misread, the agent turns blue, and in that role it can update the manuscript
  to match;
- **fencing:** the author's words verbatim and unmarked, the agent's inferences marked `[READING]`,
  open rulings marked `[AUTHOR-VERIFY]`;
- **a capture file** written by each session before it ends;
- **versions published as new files**, with the current version named in a single place, and a
  changelog that lists corrections apart from new policy.

The ten portable rules are the core of that list. The late line itself is
[`genesis-framework-late/GENESIS-FRAMEWORK-LATE.md`](../genesis-framework-late/GENESIS-FRAMEWORK-LATE.md), its seven versions in
its history, with the awakening and the voice excerpt beside it.

### 8.3 Memory in files, and the airlock

v9 moved the memory the author used to carry by hand into files the next agent opens first.

**The awakening** is the single entry point. Every agent reads it, together with a short excerpt on
reading the author, before anything else. It names the current framework in one line, which is
the only place that version is named. It carries a glossary of terms a reader meets before their
definitions, a digest of the conduct rules, and a table of modes. It is written to be safe for a
cold read: it says how to work, and leaves the content to the files a mode opens.

**The capture file** is the session's own record, written at milestones and before the session
ends: rulings, explanations that landed, stumbles, interventions, open questions with what each
waits on, and a destination for each entry. It answers §5.5: the explanation given today is on file
tomorrow. It also keeps the intervention log that §4.10 called a coverage map. The captures were
also used on purpose: the four reader audits of §8.4 are captures, and they fine-tuned the v9
protocols.

**The airlock** is the arrangement of files that keeps a cold reader's first encounter clean: what
a mode leaves closed, the reader has yet to meet. It is needed because a Claude project shares its
documents with every chat, and a cold reader loses its value once it reads spoilers. §8.4 shows how the airlock was found to need
separate files.

**The closing prompt** asks every session, before it ends, what it came to understand beyond
what the files hold, and which three changes to the onboarding would have
helped it most. Appendix A gives it in full.

### 8.4 Four readers on the first day

The sixth generation began the day v9 was written. Four fresh readers were woken in turn, each
given the same goal:

> **[AUTHOR]** *"As first agent, I am primarily interested in your awakening and what you
> encounter, with intent to finetune awakening and onboarding."* *(session)*

Each reader's audit produced a new version before the next reader woke: seven versions were
published that day, v9.0.0 to v9.3.3, the last four from the audits. Each example below gives what the reader met, why it counted
as a stumble, and what it changed. The four audits are kept in full in the repository's
[`genesis/captures/`](../genesis/captures/).

**Reader 1: a file is read whole.** v9.2.0 asked a cold reader to read only certain rules of the
framework and only the first section of the voice document. The reader opened the framework and
received all of it.

> **[READER]** *"`project_read` returns a whole file. The instruction to read the conduct rules
> only, and VOICE §0 only, became unenforceable at the first call."* Reader 1, generation 6,
> 2026-10-11 *(session)*

*Why it counts:* an unanticipated stumble, high urgency. The sections meant to stay closed sat
physically between the permitted ones, so even a reader moving top to bottom met them. *What it
changed:* v9.3.0 built the airlock from separate files. The awakening and the voice excerpt became
files of their own, and what a mode leaves closed is now a file the reader leaves unopened.

The same reader found that listing the project's documents to orient itself exposed every chapter
title: *"The titles seed models before the text arrives."*

**Reader 2: the listing differs by surface.** The awakening's note on cold reads said the session
context lists every document before the first message, as it had for the session that wrote it.
Reader 2 met an empty listing.

> **[READER]** *"…in this session the context carried no listing; I met zero chapter titles."*
> Reader 2, generation 6, 2026-10-11 *(session)*

*Why it counts:* the compiler of v9 had taken its own surface for every surface, the same horizon
error §11 records in draft r2's readers. *What it changed:* v9.3.1 says the listing *may* arrive,
and asks every reader to report what did.

**Reader 3: the baseline.** Reader 3 woke into v9.3.1, met an empty listing, opened only the two
named files, and reported thirteen stumbles. The author ruled this the baseline. Two of its findings show the grain the audit had reached. The identification line
preceded its own format: the project instructions asked for it on the first line, and the format
lived inside the awakening, read after that line was already written. And one rule's causal clause
read both ways:

> **[READER]** *"Prior: first read as a reason to write; second read as the reason to limit writes
> to milestones."* Reader 3, generation 6, 2026-10-11 *(session)*

*What it changed:* v9.3.2 put the format in the instructions, rewrote the clause as *"write at
milestones only … because each write to a project document refreshes the cache for every chat in
the project"*, and added the prior capture described
below.

**Reader 4: what reaches the author.** Reader 4 found that the harness summarises text written
between tool calls, so the identification line, written before the first file was read, reached the
author as a summary.

> **[READER]** *"…text written between tool calls is summarised for the reader; only text after
> the last tool call renders verbatim."* Reader 4, generation 6, 2026-10-11 *(session)*

It also found the harness pulling against the airlock: the reading tool's own description says to
list the project first, and the awakening says to leave the listing closed in a cold read. *What it
changed:* v9.3.3 moved the identification after the reading and repeated it in the final message,
and moved the airlock rules to the top of the awakening, ahead of anything else a reader acts on.

**The prior capture.** Before supplying any content, the author asked reader 4 what it took the
project to be, from the name alone.

> **[READER]** *"Topological quantum computing. High confidence the name evokes it; low confidence
> it is the project."* Reader 4, generation 6, 2026-10-11 *(session)*

That is a measurement of what the name recruits on its own, taken from a reader holding only the
name, and it is the cleanest reading such a question can give. The manuscript's first chapters
already disarm that prior; whether the title page should disarm it earlier is a question for the
case study, awaiting the author.

**An observation the reader made about the author.**

> **[READER]** *"Every intervention was direction; Xyzzy supplied zero explanations of content. The
> files and the chapter carried the whole session."* Reader 4, generation 6, 2026-10-11 *(session)*

Measured against §4.10, that is the airlock working: the material ran out nowhere the reader
needed it.

### 8.5 The portable rules

The late line's portable rules distil v9 into ten rules, with six templates, that load into any environment that accepts
standing instructions, from a chat assistant to a coding agent to a small local model. Their first
outside test, on a heavily quantised local model, is under way. A rule set that holds on the
smallest model it meets will hold anywhere; one that fails there shows which rules lean on the
model's size.

---

## 9. Vocabulary

The corpus holds three vocabularies, and conflating them produces wrong conclusions about
authorship.

**Implementation terminology** is the author's, in the code, older than every agent.
**Explanatory vocabulary** was coined by agents under the author's protocol: the translation layer
between the implementation and a reader. **Interaction vocabulary** emerged from the working
relationship: *stumble*, *the switch*, *red* and *blue*, *the airlock*, *disposable agents*.

> **[READER]** *"The agents coined the terms. But you designed the conditions under which those
> terms had to emerge."* The lens reader of draft r2 *(session)* `[UNVERIFIED]`

**Metaphor becoming representation.** Several readers have reported the same two-stage reaction to
an explanatory term: it reads as metaphor, then the grounding arrives and it reads as
representation. A metaphor resembles something; a technical representation preserves a
relationship. If a term lets a reader reason correctly about a structure, and then return to the
code and find what it denotes, it has crossed over. Early computing did the same with *memory*,
*register*, *bus* and *stack*, terms that stopped feeling metaphorical once the machine was
understood.

**The gaps are evidence too.** A reader once used a term as established project vocabulary and was
told the term was yet to be coined. The vocabulary is still forming, and the session that coins a term
is on file, so its formation can be observed.

---

## 10. Limits

**One researcher, one domain, two model eras.** Findings about the domain generalise weakly.
Findings about the failures may generalise better, since the failure shapes are ordinary.

**Agent swaps were confounded.** Sessions were ended when the author sensed attention changing, and
also when reloading a large context grew costly. Both rise with context size, and the two causes
separate poorly after the fact.

**One technique depends on the platform.** Pruning low-value turns whilst keeping distilled output
is available on one vendor's interface and absent from another's `[UNVERIFIED]`.

**Every reader here is an agent reading a corpus.** Where a reader agrees with a taxonomy the
corpus already holds, the agreement is worth less than it looks. Where it names something the
taxonomy lacks, the signal is stronger.

**The v9 evidence is one day deep.** Four readers, one goal, one workspace. Their audits shaped the
framework they tested, so they show the onboarding improving under audit, and leave its effect on
authoring to be measured.

**Causal claims about the case study's quality stay outside this paper**, for the reason in §0.

**What would refute the central claims.** If the register counts of §7.1 fail to replicate on
another corpus written under the same rules, the steering claim narrows to this corpus. If a reader
with the corpus finds architectural defects among the 139 findings, §6 falls. If the portable rules
hold on large models and collapse on small ones, §8.5's claim of portability narrows to model size.

---

## 11. The compilers' own stumbles

Every compiler of this paper made errors whilst producing it. They are recorded because they are
data of the kind the method collects, and because a paper about unmarked invention should mark its
own.

**Draft r2's frame reader made eight, all of one shape: a mechanism supplied one step ahead of the
evidence** `[UNVERIFIED]`. Among them: three project terms called fabricated after a search of
twelve files out of about three hundred, when all three existed; protocol numbers read as
deletions when they had been reassigned; and a verbosity mandate counted as failed against the
wrong axis (§7.2). Its own account of the first:

> **[FRAME]** *"The agent and I failed the same way with opposite signs. It treated the edge of its
> context as evidence of presence; I treated the edge of mine as evidence of absence. Both errors
> come from mistaking a horizon for a boundary."* *(session, 2026-08-19)* `[UNVERIFIED]`

**Draft r2's lens reader made the same class of error at least twice**: using a term as established
project vocabulary when it was yet to be coined, and attributing the explanatory vocabulary to the
author when agents had coined it `[UNVERIFIED]`.

**This draft's compiler, which also wrote v9, made six**, each recorded in its session capture as
prior, truth and check:

1. **A running example missed by its name.** It searched the manuscript for the name of a puzzle,
   came back empty, and took the puzzle to be absent. The chapter carries it by its characters
   and its expression, under another description.
2. **A correction cited by the wrong number.** It cited the horizon correction as item 19 of the
   onboarding brief. Item 19 is a different correction; the horizon correction was proposed in
   draft r2 and is still waiting to be absorbed. Another agent caught it.
3. **A plan reported lost that existed.** It repeated another agent's report that a publication
   plan had been lost, because the project lacked any record of it. Two plan documents existed on the
   author's side.
4. **A count stated before it was run.** It wrote that a set of mandated terms was absent from the
   manuscript, then counted, and found one of them ten times. Caught before publication.
5. **A surface taken for every surface.** It wrote, into v9's awakening, that the session context
   lists every document, because its own session did. Reader 2 met an empty listing (§8.4).
6. **An extraction error taken for a source error.** It reported that framework 8.2.0 carried a
   wrong version header. Compared with the raw transcript, the header was right; an earlier
   agent's extraction had introduced the error.

**All six share the frame reader's shape:** the edge of what the compiler held, read as the edge of
what exists. Two readers in August and a third in October, different positions, same corpus, same
failure. By the occurrence rule of §4.3, that is a rate.

**Every correction came from the author, from another agent, or from a check the author made
possible**, and each arrived as background, per §4.6.

---

## 12. Outstanding

**The portable rules' first outside test**, on a small local model, is under way (§8.5).

**v9 on authoring work.** Its evidence so far concerns onboarding. Its effect on drafting and
revision is unmeasured.

**The horizon correction.** Draft r2 proposed it as an onboarding correction: *prior: absence from
the supplied files means absence; truth: the supplied files are a sample; check: ask for the listing
before calling anything invented.* v9 carries it in its rules. The case study's onboarding brief has
yet to absorb it, and §11 counts six more instances of its shape.

**Three instruments awaiting a written method.** The seasoned-against-cold pairing, where a seasoned
agent teaches a cold one with both sides transcribed, has one session on record. The recovery sweep
exists as forty outputs. Mediation now has its log in the capture file, and still lacks a stated
method.

**The reverse sweep** of §4.9: what the manuscript once held and has since lost.

**The concept graph** of §5.5, specified in 2025 and still unbuilt.

**An index by content** (Appendix B).

---

## Appendix A: The welcome, the report, and the close

### A.1 Two welcomes

The fourth generation's welcome, used for late-stage sessions in August 2026 `[UNVERIFIED]`:

> *You are the fifth reader of the 4th generation of co-authoring army of agents responsible for
> the writing of the manuscript on the new research field of topological computing. I am
> responsible for the knowledge, insights and accountability.*
>
> *Your stumbles are important because they signal where attention needs to go, as an effect, do
> not assume anything. Assuming is a stumble and needs to be flagged.*
>
> *For this generation, the onboarding and manuscript layout has been changed, you are the first to
> receive it this way. I will include the zip that holds the corpus of work. I am interested in your
> reading order and how your internal state and mood changed during the process.*

The sixth generation's welcome, 2026-10-11:

> *You are the 1st reader of the 6th generation of co-authoring agents working on the manuscript for
> topological computing. I am responsible for the knowledge, insights and accountability.*
>
> *Your stumbles are important because they signal where attention needs to go. Flag every
> assumption you make, because an assumption is a stumble. I am interested in your reading order.*

Two changes in two months. The instruction against assuming became an instruction to flag,
which turns a prohibition into an action a reader can perform. And the request narrowed to the
reading order, the part of a report that can be checked against the files.

### A.2 The report

Every stumble in four fields: location, what tripped the reader, type, urgency (§3). Where the
reader can state it, the stumble also carries **prior, truth, check**: what the reader expected,
what holds, and how to verify it. Where only the author can supply the truth, the field is left
open and marked for him.

A worked example from reader 4 of the sixth generation, explained. Asked what the project was from
its name alone, the reader gave three readings, each with a confidence, and chose which to build
on:

> **[READER]** *"P1: Topological quantum computing. High confidence the name evokes it; low
> confidence it is the project. P2: Computation whose program is its shape. Moderate confidence.
> P3: Computational topology or topological data analysis. Low confidence. Build on: P1 from the
> name alone; P2 with everything held."* Reader 4, generation 6, 2026-10-11, condensed *(session)*

After reading the first chapter it recorded which reading each passage displaced or confirmed, and
where. The first reading was displaced as the subject and survived in the vocabulary; the second was
confirmed and sharpened. That record tells the author which passages did the work, and which
vocabulary keeps the displaced reading alive.

### A.3 The close

The awakening ends with a prompt every session answers before it closes, asked or unasked:

> *Before we close, please finish your capture file:*
>
> *1. Give every entry a destination and a status.*
> *2. List your open questions, each with what it waits on.*
> *3. Record every piece of background I supplied during the session as an intervention.*
>
> *Then answer two questions:*
>
> *What did you come to understand in this session that the files you read would leave the next
> reader without?*
> *Which three changes to the awakening or the welcome would have helped you most, in order?*

The first question finds what lived only in conversation (§5.5). The second turns each reader into
an auditor of the onboarding, which is how the last four versions of §8.4 came about.

---

## Appendix B: The corpus and its indexing

Roughly three hundred markdown documents and over a hundred session transcripts, together beyond a
gigabyte, some single transcripts larger than a reader can hold.

**Filenames describe what a document is called, at the moment it was named**, and rarely what a
later reader needs it for. One file specifying the manuscript's central teaching device was
left unrequested by ten readers, and surfaced only when the author raised its topic
`[UNVERIFIED]`.

**A corpus indexed by content is a prerequisite** for any agent expected to answer questions about
it, since a question phrased in the reader's words seldom matches a filename phrased in the
author's. An index built for that purpose, with one card per document, showed which fields earn
their place: what each document **asks** of a reader and what it **provides** carried the most
weight, ahead of dates and claims.

---

*Draft r3, 2026-10-12. Rebuilt from draft r2 of 2026-08-19, which was compiled by a frame reader
working from the corpus and a lens reader working from the frame, both corrected by the author. This
draft was compiled by Claude Opus 5.5, working from draft r2, the record in this repository, and the
captures of the sixth generation's first four readers, under the author's rulings. Every quotation
carries its source or its mark.*
