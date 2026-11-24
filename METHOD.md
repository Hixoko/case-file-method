# The method

## Before anything: what you are and are not doing

You are **not** diagnosing. You are not second-guessing clinicians, and you are
not looking for someone to blame. Cases like this go unsolved because the
information is distributed, not because anyone is careless.

You **are** doing the one thing no individual clinician is positioned to do: read
every document against every other document, and arrive at the next appointment
with the whole file in your head and three good questions ready.

Hold that line and this method works. Cross it and you will annoy the people whose
help you need.

---

## The file structure

```
case/
├── README.md               current state, current candidates, next action
├── CONTEXT.md              short re-acquire file
├── timeline.md             master chronology, step events marked
├── documents/
│   └── YYYY-MM-DD-<slug>/
│       ├── README.md       highlight · what we analysed · questions raised
│       ├── transcript.md   VERBATIM. no interpretation. [illegible] not guesses
│       └── *.jpg           source photos, descriptively named
├── analysis/
│   ├── hypotheses.md       live candidates, each with a status
│   ├── gaps.md             ordered vs missing
│   ├── contradictions.md   where documents disagree
│   ├── questions-for-doctor.md
│   └── YYYY-MM-DD-review.md   dated snapshots, FROZEN once written
└── graphs/
    ├── timeline-steps.md
    ├── causal-graph.md
    └── differential-tree.md
```

Copy the starting files from [`templates/`](templates/).

### Three rules that make it survive contact with reality

**1. Interpretation never touches the source.** `transcript.md` is what the paper
says. Everything you think about it goes in `README.md` or `analysis/`. The moment
you "clean up" a transcript you lose the ability to re-analyse, and you will
re-analyse — that is the whole point.

**2. Dated snapshots are frozen.** When you write `analysis/YYYY-MM-DD-review.md`,
you never edit it again. Current state lives in `README.md` and `hypotheses.md`
only. Without this rule you end up with three documents that each think they are
current, which is the problem you started with.

**3. Candidates carry a status, not a verdict.** `LEADING` · `OPEN` ·
`AWAITING TEST` · `WEAKENED` · `EXCLUDED`. A new result changes a status line. It
does not trigger a rewrite, and it does not delete the candidate — a candidate you
excluded for a reason that later turns out to be wrong is information.

---

## The sequence

Run the techniques in this order the first time. Afterwards, re-run 5–8 after
every appointment and every new result.

| Order | Technique | Produces |
|---|---|---|
| 1 | [Document intake](techniques/01-document-intake.md) | `documents/*/transcript.md` |
| 2 | [Timeline with steps](techniques/02-timeline-with-steps.md) | `timeline.md`, `graphs/timeline-steps.md` |
| 3 | [Causal graph](techniques/03-causal-graph.md) | `graphs/causal-graph.md` |
| 4 | [Differential tree](techniques/04-differential-tree.md) | `analysis/hypotheses.md`, `graphs/differential-tree.md` |
| 5 | [Gap analysis](techniques/05-gap-analysis.md) | `analysis/gaps.md` |
| 6 | [Contradiction pass](techniques/06-contradiction-pass.md) | `analysis/contradictions.md` |
| 7 | [Iatrogenic check](techniques/07-iatrogenic-check.md) | entries in `gaps.md` and `questions-for-doctor.md` |
| 8 | [Question generation](techniques/08-question-generation.md) | `analysis/questions-for-doctor.md` |

Techniques 2–4 build understanding. **5–7 are where the findings come from.** 8 is
what you actually carry into the room.

---

## Working with a language model

This method is a lot of reading, and a model is good at it. It is also where the
method can go badly wrong, in a way that is **distinct from** the medical-advice
problem. The failure mode is specific:

**A model reads clinical text fluently and misreads it confidently.** It will
transcribe a number it cannot actually see in a photograph. It will summarise
"F-wave latencies are normal" as "F-waves are normal" — dropping the word that
made the sentence narrow. It will assert a drug's composition from its name. Each
of these is a plausible sentence and a fabricated fact, and in a medical case file
a fabricated fact is worse than a missing one.

### The discipline

- **Transcription gets verified against the paper by a human.** Every number. This
  is tedious and it is not optional. Mark unverified transcripts as unverified, in
  the file, where someone will see it.
- **Never let the model summarise a source into the source.** Transcribe, then
  analyse the transcript. Two separate passes, two separate files.
- **Drug composition comes from the physical pack or the pharmacist**, never from
  the model and never from the brand name.
- **Ask for the quote.** Any claim about what a report says should cite the
  sentence. A claim that cannot produce its sentence is a hypothesis about the
  document, not a reading of it.
- **The model should not produce the finding and the check on the finding.** If the
  same pass wrote the transcript and spotted the contradiction, you have no
  independent check — go back to the paper yourself.
- **Reference ranges vary by laboratory.** A value the model calls abnormal may be
  normal on that lab's scale, and vice versa. Flag, then ask.

### What a model is genuinely good at here

Holding six documents in mind at once and noticing that page 5 of one disagrees
with page 2 of another. That is the bottleneck in this work, it is real, and it is
why the method is worth running with one.

---

## When to stop

The method is finished for a cycle when you have a page of questions you could
hand to a clinician and have them engage rather than defend.

You are **not** finished when you have a diagnosis, because you will not have one,
and if you think you do, go back and read [DISCLAIMER.md](DISCLAIMER.md) again.
