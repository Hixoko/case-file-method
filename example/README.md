# Worked example — Patient A

> **De-identified.** No name, no clinicians, no institutions, no locations, no
> absolute dates, no images. Dates are months relative to the index event (**M0**).
> Medicines are named by molecule, not brand. Clinical values are retained because
> they carry the teaching.
>
> **Published with the consent of the family member who assembled it.** Nothing
> here is guidance for any other patient — two people with the same results can
> have different conditions. This exists to show *how the techniques were applied*,
> not what they concluded. See [../DISCLAIMER.md](../DISCLAIMER.md).

## The case

A woman in her mid-50s. **M0:** treated for a uterine malignancy with surgery,
chemotherapy and pelvic radiotherapy. During chemotherapy she noticed weakness
while walking, which she attributed to the treatment.

Over the following five years: progressive lower-limb weakness, roughly ten falls,
a stick then a walker. At **M60** a fall preceded by dizziness, and the same day
complete urinary retention requiring a catheter that has twice failed to be
removed. By **M63** she is wheelchair-bound.

Three documents exist: imaging at **M60**, an electrophysiological study at **M62**,
and a neurology consultation at **M63**.

**No diagnosis has been made in five years.**

Relevant background, all of it recorded for the first time at M63: predominantly
vegetarian diet, hypothyroidism on replacement with normal thyroid function, a
sulfa drug allergy, no family history.

## What the three documents contain

| When | Document | What it found |
|---|---|---|
| **M60** | MRI spine (screening, no contrast), two days after the fall | No fracture, no compression, no bleed, cauda equina roots unremarkable, cord normal. Mild disc wear at two lower levels; cervical spondylosis |
| **M62** | Nerve conduction study, needle EMG, somatosensory evoked potentials | Reduced activation of *normal* motor units distally; posterior column dysfunction. No large-fibre neuropathy, no anterior horn cell disease, no myopathy |
| **M63** | Neurology consultation — history and examination | Brisk upper-limb reflexes. Knee jerks 1+. **Ankle jerks absent.** Position sense preserved. Asymmetric weakness, left worse than right |

## Running the eight techniques

### [1 — Document intake](../techniques/01-document-intake.md)

Transcribed all three verbatim. Three findings came from the transcription pass,
before any analysis:

- The prescription's **"Any Allergies" field was blank**, although the sulfa allergy
  is recorded in the same day's clinical notes.
- The M62 study's referral abstract read **"post-radiation therapy"** — framing the
  investigation around a presumed cause before it was run.
- Two values in the data tables sat **at the boundary of normal** and were
  summarised as normal.

### [2 — Timeline with steps](../techniques/02-timeline-with-steps.md)

→ [`timeline.md`](timeline.md)

Four discrete steps, not a slope: M0, ~M14, M60, M62→M63. Three followed a fall.

**The reframe:** the imaging two days after the M60 fall found no structural damage
of any kind. So the fall did not break anything — the cord dropped, and the drop
caused the fall. That reverses the question from *what did the fall damage?* to
*what makes a cord drop suddenly, repeatedly, over years?*

### [3 — Causal graph](../techniques/03-causal-graph.md)

→ [`graphs/causal-graph.md`](graphs/causal-graph.md)

Everything converged on one node: **cord and peripheral nerve damaged together**.
One orphan symptom — the dizziness preceding the M60 fall — with nothing pointing
at it.

### [4 — Differential tree](../techniques/04-differential-tree.md)

→ [`analysis/hypotheses.md`](analysis/hypotheses.md) · [`graphs/differential-tree.md`](graphs/differential-tree.md)

Four live candidates, eight excluded with specific evidence. Drawn backwards from
the tests, two candidates turned out to hinge on **conditions attached to tests
already ordered**, not on new tests.

### [5 — Gap analysis](../techniques/05-gap-analysis.md)

→ [`analysis/gaps.md`](analysis/gaps.md)

The ordered panel leaned rheumatological. The two most important tests *were* on
it. Around ten investigations speaking to the leading candidate were absent, most
addable to a blood draw already scheduled. The highest-value items were not
diagnostic: kidney function after three months of catheterisation, a one-minute
bedside vibration test, a free lying-and-standing blood pressure.

### [6 — Contradiction pass](../techniques/06-contradiction-pass.md)

→ [`analysis/contradictions.md`](analysis/contradictions.md)

Eight contradictions across three documents — including a reflex present on an
electrical test at M62 and absent on examination at M63, and a summary line that
was accurate but narrower than how it would be read.

### [7 — Iatrogenic check](../techniques/07-iatrogenic-check.md)

**The finding that justified the whole exercise.**

At M63 the patient was given, in one consultation:

- an order for a **serum vitamin B12** level
- a prescription for a nerve supplement whose principal active ingredient is
  **methylcobalamin — which is vitamin B12** — nightly for three months

Taken before the blood draw, the test reads normal whether or not she is
deficient. The candidate it was ordered to investigate was the **most treatable
one on the list**.

Also: two of the five new medicines list adverse effects that are precisely the two
problems she already had — urinary retention and dizziness causing falls. Both
would present as the disease progressing.

### [8 — Question generation](../techniques/08-question-generation.md)

→ [`analysis/questions-for-doctor.md`](analysis/questions-for-doctor.md)

Two actions above the questions. Eight questions, ordered so the first three are
the ones that matter.

---

## What the method produced

**A name for the pattern.** Brisk reflexes above, absent reflexes below, in the same
examination, means cord *and* peripheral nerve are affected together —
**myeloneuropathy**. That is a far shorter differential than "weak legs", and the
conditions near the top of it are treatable. The two findings sit one line apart in
a document that had been read many times.

**A leading candidate with ten converging findings** — and an honest caveat
attached to it.

**Two free actions that decided whether a round of testing would mean anything** —
a sequencing decision and a phone call.

**A page of questions** instead of a drive home spent realising what should have
been asked.

**What it did not produce: a diagnosis.** The method does not do that and is not
trying to.
