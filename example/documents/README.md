# Documents — Patient A

**De-identified excerpts, not full transcripts.** In a real case file each document
gets a complete verbatim `transcript.md` plus its own `README.md` — see
[technique 1](../../techniques/01-document-intake.md) and the
[document README template](../../templates/document-README.md).

Reproduced here: only the passages the techniques actually turn on. Headers,
identifiers, institutions and the bulk of the numeric tables are omitted. Keeping
the example thin is itself a de-identification measure.

---

## M60 — MRI spine (screening sequences, no contrast)

Performed two days after the fall, so it covers that event.

**Reported:** no fracture, no crushed vertebra, no displaced disc, no bleed, no
cord compression, no spinal malignancy, normal bone signal throughout, normal
conus, **"cauda equina nerve roots are unremarkable."**

**Positive findings:** *mild* disc bulges at the two lowest lumbar levels with mild
canal stenosis; cervical spondylosis; loss of the normal cervical curve.

> **What the techniques did with this.** The disc findings are a red herring: the
> M62 study found no root damage, those levels sit *below where the spinal cord
> ends* so they cannot cause position-sense loss, and mild disc wear in the
> mid-50s is near-universal. A scan read in isolation could lead to an operation
> that fixes nothing.
>
> The clean scan is *informative*, not disappointing — it removes compression,
> malignancy, fracture and cauda equina syndrome from the differential, at a known
> date, two days after the index event.
>
> What it cannot do: a screening study without contrast cannot see a dural AV
> fistula. Which is why the next scan must use contrast.

---

## M62 — Nerve conduction study, needle EMG, evoked potentials

**Referral abstract:** *"...presenting with bilateral lower limb weakness
**post-radiation therapy**. To assess for lower limb weakness."*

**Conclusions as reported:**

- Reduced activation of normal motor unit action potentials, distal > proximal
  lower limb — *"indicating a possible upper motor neurone pathology"*
- No electrodiagnostic evidence of large fibre neuropathy
- No electrodiagnostic evidence of generalised anterior horn cell disease
- No electrodiagnostic evidence of myopathy
- **Evidence of posterior column dysfunction**

**Values the contradiction pass turned on:**

| Measure | Right | Left | Why it was flagged |
|---|---|---|---|
| H-reflex latency | 31.0 ms | 31.1 ms | Present and normal — contradicted by examination a month later |
| Peroneal F-wave persistence | 4/10 | 6/10 | Reduced, while the summary addresses latency only |
| Tibial motor conduction velocity | 40.6 m/s | 41.9 m/s | At the boundary, summarised as normal |
| Tibial SSEP, P40 latency | 52.1 ms | 53.3 ms | Prolonged — the posterior column finding |
| Median SSEP | normal | normal | Normal above, abnormal below: localises the problem |

The report carries its own caution: *"EMG impression is not a final diagnosis. It
needs to be co-related with clinical and other investigative findings."*

> **What the techniques did with this.** A normal scan plus an abnormal functional
> study is a *clue*, not a contradiction. A scan shows structure; this study
> measures function. Damage from compression, tumour or disc shows on a scan.
> Damage from a missing vitamin or mineral characteristically does not — the cord
> looks normal while the insulation on exactly these pathways fails.
>
> So the combination argues *against* the causes needing surgery and *for* the ones
> treated with a tablet or an injection.
>
> Also: this study tests **large** fibres only. A normal result says nothing about
> small-fibre damage, which is what burning feet usually are. An earlier family
> reading treated it as excluding chemotherapy neuropathy — too broad, and
> corrected in [`../analysis/contradictions.md`](../analysis/contradictions.md) §3.

---

## M63 — Neurology consultation

**New in the history, recorded for the first time:** predominantly vegetarian diet ·
hypothyroidism on replacement with normal thyroid function · sulfa drug allergy ·
no family history.

**Examination, verbatim where it matters:**

> Motor: Upper-limb power greater than 4+/5. Profound weakness of both lower limbs.
> **Deep tendon reflexes: Brisk reflexes in the upper limbs. Knee jerks are 1+
> bilaterally, and ankle jerks are absent.**
> Sensory: Joint position sense is preserved. Numbness and burning in both lower
> limbs below the knees.
> Asymmetric weakness in limbs left more than right.
> Adduction and flexion of hip weak left more than right.
> **"The urinary retention has not been formally evaluated."**

**Ordered:** cervico-dorsal MRI *(no mention of contrast)* · creatine kinase · ANA
panel · HLA-B27 · vitamin D · **vitamin B12** · X-rays of knees, pelvis and hips.

**Prescribed, same consultation, three months each:**

| Molecule | For |
|---|---|
| **Methylcobalamin** + alpha lipoic acid | Nerve repair and nerve pain |
| Duloxetine 10 mg | Nerve pain |
| A gabapentinoid, 300 mg | Burning pain |
| Omega 3 & 9 | General support |
| A second nerve supplement | General support |

**On the prescription form, the "Any Allergies" field is blank.**

> **What the techniques did with this.** The two reflex lines sit one line apart:
> brisk above, absent below. That is cord *and* peripheral nerve together —
> **myeloneuropathy** — a far shorter differential than "weak legs", and the whole
> basis of the analysis. Nobody had attached a name to it.
>
> **Methylcobalamin is vitamin B12.** Prescribed in the same consultation that
> ordered a serum B12 level. Taken first, the test reads normal regardless of the
> truth. See [technique 7](../../techniques/07-iatrogenic-check.md).
>
> Two of the five medicines list adverse effects that are exactly the two problems
> she already has — urinary retention and dizziness causing falls — so both would
> present as the disease progressing.
>
> The blank allergies field, in a catheterised patient whose likeliest infection is
> reflexively treated with a sulfonamide, is the single most consequential line on
> the page.
