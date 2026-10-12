# Positive framing

The house style of the case study asks for positive framing, and it was an issue from the very
first sessions. This file holds the author's reason for it and the method agents use to apply it.
It sits beside [`reachingConsensus.md`](reachingConsensus.md), where the same rule shapes one
paragraph across fifteen versions.

**The rule**, the author's standing instruction, verbatim:

> Avoid negative words. Frame from the positive. Avoid the use of NOT and all it's variations like
> don't, won't can't, shouldn't. Avoid using dashes in prose as separator. Spelling British English.
> Keep asking for clarifications until we mutually agree on the topic before presenting code or
> proposals.

**Who can use it.** Any author who holds the same rule. The method below was written for the case
study and keeps its examples; the reasoning carries to any work whose readers arrive with a model
the work has to replace.

---

## Why: one direction of flow

The author's statement, given 2026-10-11:

> With the AI co-authoring, blue team is enthusiastic, inviting and positive, and red is grounding
> and challenging. Also, because the manuscript is paradigm changing and the readers are considered
> naturally hostile towards change, the general tone should be positive and inviting. This is also
> one of the pillars of using a positive framing. It is based on the same idea as the "Void", where
> the *flow* comes from one direction, thereby avoiding atmospheric contradictions, giving friction
> and hooks to put attention on things that could distract attention and could be avoided making a
> more powerful statement.

*The Void* is the case study's single reference value: every difference in the architecture is
measured as a departure from it, in one direction, with no second pole to reconcile. The style
follows the same shape. The readings below are the agents', confirmed with the author, and marked.

`[READING]` **A negation installs a second pole in the prose.** The claim and its rival occupy the
room together, and the reader holds both until they work out which is operative.

`[READING]` **The contradiction is atmospheric rather than logical.** Nothing in the text is
formally inconsistent. What exists is a tone carrying two directions at once, and a resistant reader
meets the tone before the argument.

`[READING]` **Each pair is a hook**, and what it catches is the rival rather than the claim.
Removing the pole lets the statement land, because nothing competes for the attention the claim
needs.

`[READING]` **The rule governs hooks, and negation is one kind.** Two more have been removed by the
same reasoning. An invented figure of speech, where a reader stops to appraise the phrase instead
of the claim it carries (version 9 of [`reachingConsensus.md`](reachingConsensus.md) shows the
repair). And a demonstration that outshines what it demonstrates; in the author's words:

> Cryptography has also been removed and replaced wity Zeno, the toy cypher, as to avoid hostile
> readers diverting attention trying to make a single application a major topic.

`[READING]` **Position outweighs rate.** A negation on a chapter's first page meets a reader still
deciding whether to continue; one in an appendix meets a reader already committed. So a target rate
wants a positional companion: the early pages carry the least.

**The two teams are mandates, as well as exemptions.** Blue is enthusiastic, inviting and positive.
Red is grounding and challenging. The method below governs blue prose; red output reports plainly.

---

## The method

*Written by the agents as a standing instruction for writing and editing the case study, and kept
here as it stands. Its figures were measured on the case study.*

### 1. What a negation costs a reader

The reason matters more than the rule, because the reason tells you which cases are in scope.

**A reader meeting a negated statement builds the affirmative picture first, then inverts it.** Inversion runs slower than reading speed. So a reader moving at pace skips the operator, carries the un-inverted image forward, and is left with a vague sense that the text is withholding something.

Three separate costs ride on that, and they stack:

**Processing time.** Negative sentences are verified more slowly and less accurately than affirmative ones. The reader assembles the proposition, then applies the operator as a second step.

**Residual activation.** The negated concept stays partly live. *This is nothing like a hash table* leaves hash table in the room.

**Pragmatic suspicion.** A denial implies somebody held the belief being denied. A reader meeting an unlicensed negative starts reconstructing who believed that and why it needed answering. This is the cost that damages trust, and it is the one the instruction exists to prevent.

*The first two are recalled from the psycholinguistic literature rather than checked against sources. The third comes from the author's own observation and is the load-bearing one.*

---

### 2. Four levels, by grammatical scope

Cost tracks scope. **Negating a proposition costs two images; negating a noun slot costs one; a word that carries the negation inside its meaning costs none.**

| level | form | examples | cost |
| ---: | :--- | :--- | :--- |
| 1 | lexical | `ignores`, `absent`, `alone`, `avoids`, `empty`, `bare` | lowest |
| 2 | phrase | `without X`, `no + noun` | lower |
| 3 | fused | `never`, `cannot` | middle |
| 4 | propositional | `is not`, `does not`, contractions | **highest** |

**Level 4 is the target.** It carries all three costs. Levels 1 and 2 are cheap and usually fine as written.

Why the split works: `not` is a propositional operator, arriving after the reader has assembled a proposition, applying to the whole of it, with frequently ambiguous scope. `without` is a preposition attaching to a noun phrase, so the reader carries a modified object rather than reworking a proposition. `ignores` arrives from the lexicon already assembled, so no operator gets applied to anything.

---

### 3. Closure: the exception that matters most

> **It is not this because it is that.**

A negation that supplies its replacement **in the same breath** performs the inversion for the reader. Nothing has to be reversed, and nothing feels withheld. This construction is correct and should be left alone.

Closure landing one sentence later also counts:

> *The runtime does not tell the engine what type to use. The runtime selects which pre-computed answer it needs.*

The underlying principle: a negative that **corrects an expectation the reader actually holds** is cheap, because the correction is what they were already reaching for. A negative that merely describes is expensive.

**Practical test.** Read to the full stop. If the replacement has arrived, leave it.

---

### 4. Repair order

**First, absorb into a verb.** Minimal intervention, sentence shape preserved.

| shape | affirmative verbs |
| :--- | :--- |
| `without` | avoids, sidesteps, skips, bypasses, forgoes, spares, dispenses with, leaves untouched, … alone |
| `does not` | ignores, declines, omits, overlooks, passes over |
| `never` | stops at, stays, remains, passes through un‑ |
| `cannot` | receives from outside, reaches only, stops at, resists |
| `fails to` | observes X instead, settles at |

Also `absent` as an adjective, which names a state in one image where *is not present* asks for two.

**Second, state what is there.** Where no verb absorbs it, supply the positive fact. This usually improves the sentence, because the negative form only removed a wrong reading whilst the positive form carries content:

| before | after |
| :--- | :--- |
| The engine **cannot generate** it internally. | The engine **receives** it from outside. |
| This number **is not** a measurement of speed. | This number **counts** the structural redundancy annihilated in one step. |
| its components **were not mutually prime** | its components **shared factors** |
| A structure **without tension has no** driving force toward its ground state. | **Tension is the driving force toward the ground state.** |

**Third, if the propositional form must stay, mark it.** See §6.

---

### 5. Two hard constraints on every repair

#### 5a. Named objects survive

**If the negated object is a named technique, field, or tool, the name stays and only the verb moves.**

> ✗ The runtime engine achieves these results **without backtracking or heuristic state-space traversal**.
> ✗ The runtime engine **arrives at these results by address**. ← names lost
> ✓ The runtime engine achieves these results, **avoiding** backtracking and heuristic state-space traversal.

This constraint exists because the positive reframe reaches naturally for the paradigm's own vocabulary, and that vocabulary is more abstract than the rival names it displaces. Across hundreds of repairs the bias runs one way and erodes exactly the comparisons a synthesis reader needs.

#### 5b. Contrast budget

Banning `not` diverts traffic into contrastive constructions. Measured on this corpus, `rather than` runs at **36 per 10,000 words against a natural ceiling of 3** across every general English corpus tested. That is twelve times the highest natural rate and has no analogue anywhere.

So a naive pass trades a mild anomaly for a severe one.

**The best repairs introduce no contrast at all.** *The Footprint ignores how the structure was built.* *Its components shared factors.* Reach for `rather than` last, and spread across *instead of*, *in place of*, *over*, *as against*, or restructure.

---

### 6. The `**not**` marker

Where a propositional negation is genuinely unavoidable, **mark the operator word in bold** to interrupt the skim and buy the reader the milliseconds the inversion needs.

> The tilde is an adjective, **not** a verb.

**Bold the single word only.** Bold on the whole clause already carries a different job in this corpus (marking the load-bearing clause, at roughly 1,900 spans), and two jobs on one marker dilutes both. Scope distinguishes them: word-level says *slow down, an inversion is happening*; clause-level says *this sentence carries the weight*.

**Avoid capitals.** `NOT` names the logic gate throughout this manuscript.

**Markdown, since this trips people.** One asterisk is italic, two is bold. `*not*` renders italic; `**not**` renders bold. Same for underscores.

**This convention is already emergent.** Eight instances of a bolded bare negation exist in the corpus, unprompted and unnamed, against one italic. Applying it is declaring an existing convention rather than imposing a new one. A convention used silently reads as ordinary emphasis and buys nothing, so it must be **declared** where a reader meets it early.

---

### 7. Scope: what to leave alone

| leave alone | why |
| :--- | :--- |
| quoted author speech, session transcripts | altering them falsifies evidence |
| code, operators, formulas | `!=`, `~`, `Q & ~T` are notation |
| `Anti-Void`, `non-recursive`, `non-local`, `inversion-free` | named terms; the first is a proper noun of the architecture, the rest are field vocabulary or global invariants |
| level 1 and level 2 forms | cheap for the reader |
| closed constructions | see §3 |
| the Researcher's Note (`1-02`) | spoken register; its anaphora is built on repeated negation and is good writing |
| red-team and red-red output | confrontation is negatively framed by nature; an unhedged negative is the clearest signal for an auditor checking a claim |

**The rule governs blue prose.** Red output is exempt by design.

---

### 8. Target, with numbers

Measured with one regex across standard corpora and this manuscript. **The destination is ordinary expository prose, not zero.** Driving below it makes the text anomalous in the other direction.

| corpus | propositional `not` per 10,000 words |
| :--- | ---: |
| unconstrained agent prose (this project, before the instruction) | **91** |
| Brown: learned (academic) | 36 |
| Brown: news | 29 |
| **manuscript, current** | **29** |
| Brown: government | 21 |

**The manuscript has already reached target.** The instruction cut its own form by roughly 70% and landed below the academic norm. Further reduction is purism.

What remains elevated is the cheap band: `nothing` at 4.2×, `never` at 4.6×, `without` at 2.8×, `none` at 5.0× the academic rate. Some of that is displacement from §5b. It costs readers little and has been ruled out of scope.

---

### 9. Checklist

For each negation encountered:

1. Quoted, code, named term, red output, or the Researcher's Note? → **leave**
2. Level 1 or 2 (lexical or phrase-level)? → **leave**
3. Closed in-sentence or next sentence? → **leave**
4. Level 4, unclosed? → absorb into a verb, keeping every named object
5. No verb available? → state the positive fact, adding no contrast
6. Genuinely unavoidable? → mark it `**not**`

Aim for the minimum edit. A single verb swap beats a rebuilt sentence, and a rebuilt sentence that reads worse than the original is a failed repair however clean its negation count.
