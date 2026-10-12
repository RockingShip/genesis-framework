# Running reader audits

A reader audit spends one fresh agent to find where your material trips a newcomer. Once an agent
has understood something, it can never meet it for the first time again, so each reader is used
once. What accumulates is the record you keep.

The same method tests the material itself (a chapter, a document) or your onboarding (the rules and
the awakening). The paper's [§8.4](../paper/GENESIS-PAPER.md) shows four readers testing an
onboarding in one day, each audit producing the next version.

## Before the first reader

1. **Choose what is under test.** One thing per audit: the onboarding, or a named piece of the work.
2. **Decide what the reader may open.** Name the files by path. Everything else stays closed, because
   whatever a reader opens, it has read. If your environment lists all documents at the start,
   expect the reader to report that listing, and treat titles it saw as part of what it met.
3. **Prepare the welcome** from [`templates/readerWelcome.md`](templates/readerWelcome.md), with the
   reader's number, its generation and the goal.

## During the session

1. **Start a fresh session.** Load the rules and the awakening, then send the welcome.
2. **Optionally take a prior capture.** Before supplying anything, ask what the reader takes the work
   to be from its title alone, with a confidence for each reading.
3. **Let the reader read and report.** Answer questions about procedure. Hold back explanations of
   content, because the moment you explain, the reader's first encounter is spent.
4. **Mark the switch.** When you begin explaining, ask the reader to write its stumble report into
   its capture first. From then on it works as a co-author.
5. **Note every intervention.** Each time you had to supply background to keep the session moving,
   the material was missing something. The reader records these in its capture.

## Closing

Send [`templates/closingPrompt.md`](templates/closingPrompt.md). Save the capture.

## Folding it back

1. **Sort each stumble** into anticipated (the material already answers it), unanticipated (the main
   signal) or misread (the reader mapped your idea onto a neighbouring one; the most valuable kind).
2. **Count across readers.** A stumble one reader reports is an opinion. The same stumble from
   several independent readers is a rate, and it earns a place in your onboarding.
3. **Correct with background.** Write each correction as prior, truth, check: what a reader will
   expect, what holds, and how to verify it. A correction in that form travels to readers who were
   absent when the error was made.
4. **Place the correction where the stumble happens.** A correction kept only in a separate list
   protects few readers; one placed in the text at the point of the stumble does the work.
5. **Publish a new version** of the material or the onboarding, as a new file, with a changelog line
   naming the reader whose audit prompted it. Then wake the next reader against the new version.

## The transport test

The strongest audit gives your rules to a different model, ideally a small one. Rules that hold on
the smallest model they meet will hold anywhere; rules that fail there show which ones lean on the
model's size. Record the model and its settings with the capture.
