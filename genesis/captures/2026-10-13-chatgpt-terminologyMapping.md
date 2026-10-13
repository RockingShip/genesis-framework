> **Outside reading, dated 2026-10-13.** ChatGPT mapping the paper's vocabulary onto established research terms, the second of the two replies. ChatGPT read the public repository at release 1.1.0, with the paper at r3. Verbatim; image links and source favicons inserted by the chat interface are removed. One of the cold readings that feed the paper's r4.

# Genesis terminology: a translation into established research language

Yes. Having gone back through the paper, I think the important distinction is that you have coined language at several different levels: some terms name known phenomena, some name your particular operational solution to those phenomena, and some are genuinely useful conceptual metaphors that connect several existing fields.

The paper explicitly distinguishes the island, your architecture as discovered through a running system and expressed in its own vocabulary, from the mainland, the established scientific literature. That distinction is itself a useful starting point for translating your terminology into established research language.

Here is my best mapping. I distinguish established equivalent from closest analogue: the latter means the concept overlaps with existing work, not that your exact term is already standard.

## 1. Your core conceptual vocabulary

These are the terms I consider most important to the paper's intellectual contribution.

| Your term                       | Closest established terminology                                       | What your term adds                                                                                                                             |
| ------------------------------- | --------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Island                          | Domain-specific conceptual framework; emergent theory; novel ontology | A whole body of concepts discovered through observation of a working system, before its terminology has been aligned with existing disciplines. |
| Mainland                        | Established literature; disciplinary knowledge; prior art             | A memorable name for the external body of knowledge against which the island's concepts must be compared.                                       |
| Island language                 | Domain-specific terminology; local ontology; technical vocabulary     | Highlights that the words may be internally coherent while having misleading meanings in other disciplines.                                     |
| Mainland correspondence         | Concept mapping; theoretical alignment; cross-disciplinary mapping    | Identifies a proposed relationship between an island concept and an established concept without automatically claiming they are equivalent.     |
| Stumble                         | Comprehension breakdown; reader difficulty; usability problem         | Makes the reader's difficulty a valuable observation about the interaction between reader and text, rather than merely a reader error.          |
| Disposable reader / cold reader | Independent evaluator; fresh-context evaluation; novice-user testing  | Treats lack of accumulated context as a deliberate property of the measuring instrument.                                                        |
| The author as the boundary      | Human oversight; epistemic authority; human-in-the-loop verification  | Specifies the point at which exploratory model output must be reviewed before it becomes an accepted research claim.                            |

The first four terms form a particularly useful group. The island/mainland metaphor distinguishes the development of a new conceptual system from the later task of relating it to existing knowledge. It is not simply a glossary problem: a translation may be linguistically plausible and conceptually wrong.

Your example of a reader interpreting an unfamiliar operator through Boolean logic illustrates this directly. The reader is not failing to understand the notation at random; the reader is applying an established conceptual model to a new construct.

A terminology note I would make in the paper: island language is not the same as jargon in the usual sense. Jargon can be precise and well established within a discipline. Your concern is language whose meaning is locally grounded in a newly discovered architecture, where an established field supplies a plausible but incorrect interpretation.

That distinction is worth preserving.

## 2. Your vocabulary for failure modes

This is probably the most immediately useful part of the terminology for researchers and practitioners. Several terms give names to failure mechanisms that otherwise require a paragraph to describe.

| Your term                             | Existing field / nearest equivalent                                            | Assessment                                                                                                                  |
| ------------------------------------- | ------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------- |
| Stumble taxonomy                      | Qualitative coding scheme; error taxonomy; usability evaluation                | A structured way to classify reader observations. Your three categories are specific to the workflow.                       |
| Anticipated stumble                   | Known usability issue; anticipated error; regression-test case                 | A difficulty the text already anticipates and tries to intercept.                                                           |
| Unanticipated stumble                 | Previously unidentified usability problem; exploratory finding                 | A new difficulty revealed by a fresh encounter.                                                                             |
| Misread                               | Misconception; semantic misinterpretation; false analogy                       | A reader applies an adjacent conceptual framework and consequently misses the actual claim.                                 |
| Mode 6                                | Post hoc rationalization; confabulation; unsupported causal attribution        | A reader invents a plausible explanation for a design decision without evidence of the actual reason.                       |
| Erosion                               | Knowledge loss; regression; requirements drift; documentation decay            | A previously established decision or correction disappears during later revisions or consolidation.                         |
| Knowledge that stayed in conversation | Tacit knowledge; undocumented decisions; knowledge-transfer failure            | Knowledge is repeatedly understood in individual sessions but never becomes persistent, transferable documentation.         |
| Horizon error                         | Bounded-context reasoning; partial-observability error; sampling bias          | The agent mistakes the limits of the material it can see for the limits of what exists.                                     |
| False familiarity                     | Familiarity bias; semantic anchoring; schema-driven misinterpretation          | A reader becomes accustomed to an unfamiliar term and stops treating it as unresolved, then substitutes a familiar meaning. |
| Recovery sweep                        | Provenance audit; retrospective requirements recovery; archival reconstruction | A systematic comparison of historical conversations and current documentation to recover material that was lost.            |

The paper explicitly defines anticipated, unanticipated, and misread as three different kinds of stumble. It also identifies Mode 6 as a confabulated rationale and erosion as the disappearance of previously established fixes.

A few distinctions are worth making.

Erosion is not quite the same as regression. In software engineering, regression usually means a change reintroduces a defect or breaks previously working behaviour. Your term covers a broader problem: the reasoning behind a decision can disappear even if no software defect is introduced. A rule can still be present somewhere, yet its rationale or application can erode.

Horizon error is especially interesting. Your examples include both treating absent material as proof of absence and assuming that another agent shares the same project context. These are related, but not identical, problems. I would define the general phenomenon as mistaking a boundary of observation for a boundary of reality. That is a concise and potentially reusable definition. The paper itself notes that this failure appeared in different forms across multiple readers and the compiler.

Mode 6 deserves its own name if you can operationalize it. It is more specific than ordinary hallucination. The agent does not necessarily invent an obviously false fact; it invents a plausible rationale for an observed decision and presents that rationale as if it were known. In research writing, this can quietly transform an undocumented motivation into apparent historical fact.

I would keep Mode 6 as your internal framework label, but use unsupported post hoc rationale as its initial plain-language translation for new readers.

## 3. Your operational vocabulary: how the framework works

These terms describe the method you developed in response to those failures. Most have close counterparts in established practice, but the combination and the operational details are what distinguish your implementation.

| Your term                | Established analogue                                                                   | What is distinctive in Genesis                                                                                     |
| ------------------------ | -------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Red                      | Red teaming; adversarial review; independent evaluation                                | Used specifically to report the experience of reading without collaboratively repairing the text.                  |
| Blue                     | Collaborative drafting; co-authoring; assisted editing                                 | The constructive mode that begins when the author explains or revises.                                             |
| The switch               | Mode switching; phase transition; role separation                                      | An explicit transition from measuring a first encounter to collaborating on a correction.                          |
| Stumble harvest          | Exploratory usability testing; issue discovery; qualitative data collection            | A stream of fresh readers is deliberately used to find problems the author has become unable to see.               |
| Disposable agents        | Stateless workers; ephemeral evaluators; fresh-context replication                     | The agent is deliberately not allowed to accumulate the very familiarity that would weaken the measurement.        |
| Bracketing device        | Anticipatory misconception correction; contrastive explanation; conceptual scaffolding | A known wrong interpretation is named and corrected before it becomes the reader's working model.                  |
| Correction by background | Explanatory feedback; conceptual change; error remediation                             | Explains both the correct interpretation and why the wrong interpretation was initially plausible.                 |
| Mediation as supply line | Human-in-the-loop mediation; knowledge brokering; dependency analysis                  | Each author intervention is treated as evidence that the persistent documents may lack knowledge the agent needed. |
| Authority hierarchy      | Source-of-truth policy; data provenance; evidence hierarchy                            | Gives explicit precedence to author rulings, current text, dated evidence, and stamped measurements.               |
| Positive framing         | Affirmative instruction design; contrastive learning; cognitive debiasing              | Describes what a construct is rather than activating a familiar but incorrect concept through negation.            |

The red/blue distinction and the switch are explicitly defined in the paper as separate modes of interaction, while the stumble harvest and recovery sweep have different functions: one discovers difficulties in a fresh reading, and the other recovers material that historical work may have lost.

### Three terms I would particularly preserve

The switch

This is a useful operational concept because it makes the purpose of a session explicit. Are you measuring the reader's first encounter, or are you now working with the author to change the text? The distinction is related to role separation in evaluation research, but your named transition makes it easier to implement and discuss.

Mediation as supply line

This is more than a metaphor for human oversight. It turns an intervention into a diagnostic signal: if the author has to supply background for an agent to proceed, the persistent record may not contain enough information for the next agent. This is closely related to knowledge management and requirements traceability, but the intervention log gives it an actionable form.

The airlock

The paper uses this for the separation of files that preserves a genuinely fresh reading. In evaluation terms, it controls information leakage: a reader must not see material that would reveal the intended interpretation before encountering the passage under test. It is a particularly clear metaphor for the mechanism.

The airlock is a good example of a term that becomes more than decoration. In the paper, an initial instruction to read only selected sections failed because the interface supplied the whole file. The response was to separate the files physically, so the desired information boundary was enforced by the artifact rather than by instructions alone.

That maps closely to a principle from security and systems engineering: enforce a boundary in the system where possible rather than relying on a participant to remember a rule.

## 4. Your terms for preserving knowledge and controlling evidence

This final group is less about how an agent misunderstands a concept and more about how a long-running research project maintains continuity and intellectual integrity.

| Your term                        | Established equivalent                                                  | Why the distinction matters                                                                                                         |
| -------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Awakening                        | Bootstrap instructions; onboarding document; initialization protocol    | A single, controlled entry point that tells an agent how to work before exposing it to the full corpus.                             |
| Capture file                     | Session log; decision log; research diary; structured provenance record | Records decisions, explanations, misunderstandings, interventions, and unresolved questions for the next session.                   |
| Portable rules                   | Operational protocol; reusable prompting policy; workflow specification | Rules intended to survive changes of model, session, and execution environment.                                                     |
| Supply discipline                | Context management; information filtering; progressive disclosure       | Deliberately selects which evidence an agent receives and when.                                                                     |
| Fencing                          | Provenance labeling; claim attribution; source separation               | Distinguishes the author's statements, the agent's interpretations, and decisions still awaiting verification.                      |
| Authority hierarchy              | Evidence hierarchy; source-of-truth governance                          | Specifies which source wins when current documentation, historical records, and conversational claims disagree.                     |
| Recovery sweep                   | Retrospective audit; requirements recovery; knowledge archaeology       | Reconstructs missing documentation from historical records.                                                                         |
| Metaphor becoming representation | Operationalization; conceptual modeling; semantic grounding             | A metaphor becomes a usable technical concept when it preserves a real relationship and maps back to the underlying implementation. |

The paper explicitly separates implementation terminology, explanatory vocabulary, and interaction vocabulary. It also describes the awakening, capture file, airlock, and portable rules as components of the latest framework design.

Two of these ideas are especially transferable.

“Silence gets marked. It does not get filled.”

The closest research terms are epistemic uncertainty, abstention, and provenance-aware claim generation. But your formulation is a stronger operational instruction: when the available evidence does not establish a fact, record the gap rather than completing it with a plausible detail.

The paper reports that many of the roughly 139 findings in the case-study corpus involved plausible details being supplied where the source was silent. That gives this principle a concrete origin in the project, although the generality of the reported pattern still needs independent testing.

“Every rule its reason.”

This is related to explainable systems, design rationale, and requirements traceability. Your version is more specific than simply asking for explanations: a rule must carry the reason that makes it intelligible to the next agent. Without that reason, later agents may obey the wording in one context and remove or reverse it in another.

That is an important design principle for any workflow where instructions evolve across many sessions.

## 5. Which terms are genuinely distinctive?

I would group the vocabulary into three categories.

Preserve as signature terms

Island / mainland; stumble; horizon error; erosion; the switch; airlock; mediation as supply line; Mode 6.

These give the paper a recognizable conceptual vocabulary. Some are novel metaphors for known phenomena; others combine several established ideas into a specific mechanism. Their value lies in making the failure recognizable, discussable, and potentially measurable.

Use with a plain-language gloss

Stumble harvest; recovery sweep; awakening; capture file; portable rules; supply discipline; fencing.

These are good operational names, but a new reader should be able to infer their function without first learning the entire Genesis vocabulary.

Define carefully before making general claims

Disposable reader; positive framing; anticipated stumble; misread; metaphor becoming representation.

These concepts are useful but need clear boundaries. For example, a fresh model session is not necessarily an independent evaluator, and a reader's misinterpretation is not automatically evidence of a defect in the text. The experimental conditions determine what can be inferred.

One particularly interesting idea is metaphor becoming representation. The paper suggests that an explanatory term first sounds figurative, then becomes a technical representation once the reader can reason with it and locate what it denotes in the code.

I would not claim that this is a wholly new phenomenon. It connects to established work on conceptual modeling, semantic grounding, and the history of technical terminology. But your formulation makes a useful distinction between a metaphor that merely helps someone imagine a system and one that preserves a relationship they can use to reason about the system.

That could become a research question of its own: Can we predict which explanatory metaphors will support correct reasoning, and which will cause readers to import the wrong model?

## 6. How I would present the vocabulary to researchers

I would add a short terminology table to the paper or repository README with three columns: Genesis term, established analogue, and operational definition. It would help readers translate your language without flattening the concepts into supposedly exact synonyms.

Here is a compact example of how that might read.

### Genesis terminology and established concepts

Genesis uses a project-specific vocabulary to describe recurring failure modes in long-running AI-assisted research. The terms are not intended to replace established terminology where an exact equivalent exists. They name observations and operational mechanisms that arose within the case study.

- **Island / mainland:** a distinction between a locally developed conceptual system and the established literature against which its concepts must be mapped.
- **Stumble:** an observable difficulty encountered during a reader's first encounter with a text, analogous to a comprehension breakdown or usability finding.
- **Horizon error:** treating the boundary of the evidence or context available to an agent as the boundary of what exists.
- **Erosion:** the loss of an established decision, correction, or rationale during later revisions, related to but broader than software regression.
- **Mode 6:** an unsupported post hoc rationale attributed to a decision whose actual motivation is unknown.
- **The switch:** the transition from evaluating a reader's first encounter to collaboratively explaining or revising the text.
- **Airlock:** an information-separation mechanism intended to preserve a reader's fresh encounter with material under evaluation.
- **Mediation as supply line:** treating each author intervention as evidence that the persistent documentation may not yet contain the knowledge required for independent continuation.
- **Silence gets marked. It does not get filled:** an epistemic rule requiring unsupported details to remain explicit gaps rather than being supplied as plausible inventions.

These terms are presented as operational definitions within Genesis. Their relationships to established concepts are correspondences, not claims of terminological or theoretical equivalence.

## My final take

Your terminology is doing three different jobs, and I think that is worth making explicit in the paper.

1. Descriptive language: stumble, erosion, horizon error, Mode 6. These help identify what went wrong.
2. Method language: red, blue, the switch, stumble harvest, recovery sweep. These tell a researcher what to do about it.
3. Architectural language: island/mainland, airlock, capture file, mediation as supply line. These explain how the workflow preserves knowledge and separates tasks.

The strongest contribution is not that every term names a previously unknown phenomenon. Most have recognizable relatives in existing fields. It is that you have connected those phenomena to a repeatable research workflow and given them names that can be carried from one session to the next.

I would make one further distinction as you develop the paper: a term can be novel without the underlying phenomenon being novel, and a framework can be useful without its effectiveness being established. Keeping those claims separate will make the vocabulary more credible and make it easier for other researchers to adopt, test, or improve it.
