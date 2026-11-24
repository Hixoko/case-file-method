# case-file-method

**A method for families holding a medical case nobody has solved yet.**

> ⚠ **This is not medical advice and contains none.** It is a set of reading and
> organising techniques. It does not diagnose, and it is not written or reviewed by
> clinicians. Everything it produces is **questions to take to a doctor** — never a
> decision to take without one. See [DISCLAIMER.md](DISCLAIMER.md).

---

## The problem this is for

Someone you love has a condition that has been investigated for years without a
name. The case is handed between specialists, each of whom sees a slice. Reports
accumulate as photos on a phone. Nobody disagrees with anybody; it is just that
**no one party is holding the whole file.**

Except you. You are the only person who has read every document, been at every
appointment, and watched the decline day to day. That is a real analytical
position, and it is almost always wasted — because it lives in your head and in a
camera roll instead of somewhere it can be reasoned over.

This repo is what to do about that.

## What it is

Eight techniques for reading a stack of medical documents as a **set** rather than
one at a time, plus the file structure that makes it repeatable, plus a worked
example running a real (de-identified) case through all eight.

The techniques are ordinary analytical moves — build a timeline, draw a graph,
list what's missing, check for contradictions. The reason to write them down is
that **nobody does them on medical records**, because the records arrive one at a
time and each one feels like a complete thought.

## What it caught in the worked example

A five-year undiagnosed progressive neurological decline. Running the eight
techniques over three documents surfaced, among other things:

- **A prescribed supplement that would invalidate a blood test ordered in the same
  consultation** — erasing the most treatable candidate on the list, in a way that
  would read as a normal result. *(Technique 7)*
- **A reflex pattern spanning two reports** that narrows "weak legs" to a specific
  and much shorter differential — visible only when both reports are read together.
  *(Techniques 3, 6)*
- **A curable candidate that the ordered scan would miss**, because the order didn't
  specify contrast. *(Technique 5)*
- **A decline that looks like a slope but is a staircase** — which reverses the
  apparent cause-and-effect between falls and deterioration. *(Technique 2)*
- **An allergy recorded in the notes but left blank on the prescription**, in a
  patient whose likeliest infection is reflexively treated with that drug class.
  *(Technique 6)*

None required medical training. All required reading the documents against each
other instead of in sequence.

## Start here

1. **[METHOD.md](METHOD.md)** — the end-to-end workflow and the file structure
2. **[techniques/](techniques/)** — the eight lenses, one file each
3. **[example/](example/)** — a real case run through all eight, de-identified
4. **[templates/](templates/)** — copy these into your own case file

## The eight techniques

| # | Technique | What it's for |
|---|---|---|
| 1 | [Document intake](techniques/01-document-intake.md) | Transcribe verbatim; keep interpretation out of the source |
| 2 | [Timeline with steps](techniques/02-timeline-with-steps.md) | Is it a slope or a staircase? The answer narrows everything |
| 3 | [Causal graph](techniques/03-causal-graph.md) | Symptom → finding → mechanism → candidate. Find the orphans |
| 4 | [Differential tree](techniques/04-differential-tree.md) | Candidate → support → **which one test prunes it** |
| 5 | [Gap analysis](techniques/05-gap-analysis.md) | What was ordered vs what this pattern calls for |
| 6 | [Contradiction pass](techniques/06-contradiction-pass.md) | Read every report against every other |
| 7 | [Iatrogenic check](techniques/07-iatrogenic-check.md) | Does the treatment break the test, or worsen the symptom? |
| 8 | [Question generation](techniques/08-question-generation.md) | Turn findings into questions a clinician will engage with |

Technique 7 is the one that earns the repo.

## A word on working with an AI assistant

The worked example was produced by a family member working with a language model.
That is a reasonable way to use this, and it carries a specific hazard that is
**not** the same as the medical-advice warning: models read clinical text fluently
and misread it confidently. [METHOD.md](METHOD.md) has the verification discipline
this requires. Do not skip it.

## Licence

Prose and templates: [CC BY-SA 4.0](LICENSE).
