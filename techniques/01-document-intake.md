# 1 — Document intake

**Transcribe verbatim. Keep interpretation out of the source.**

## What it is

Every document gets typed out, exactly as written, into `transcript.md`. Then,
separately, a `README.md` next to it says what it found and what you concluded.

Two files, because they have different lifespans. The transcript is written once
and never changes. The README gets rewritten every time your understanding moves.

## When it pays

Always, and it is the least appealing technique here, so it gets skipped. Don't.

Three things it buys you:

**Re-analysis becomes possible.** Six weeks from now a blood result arrives that
makes you want to re-read the September study with new eyes. If you summarised it
back then, you will re-read your summary — which was written by someone who did
not know what you now know.

**Search works.** Fifteen photos are not searchable. Fifteen transcripts are.

**You read it properly, once.** Typing out a nerve conduction table forces you
through every number. Half the findings in the worked example came from the
transcription pass, not the analysis pass.

## How to run it

1. **One folder per document**, named `YYYY-MM-DD-<slug>`. The date is the
   document's date, not the day you photographed it.
2. **Type it out exactly.** Keep the original's oddities — double full stops,
   inconsistent capitals, the struck-through word. They occasionally matter.
3. **`[illegible]` where you cannot read it. Never a guess.** This is the single
   most important rule in the method. A guessed number in a medical file is worse
   than a gap, because a gap gets checked and a guess gets trusted.
4. **Record what the form left blank.** An empty field on a prescription is data.
   In the worked example an empty field was one of the findings.
5. **Note the metadata** — who wrote it, who it was addressed to, who referred the
   patient, what the stated reason for the test was. The referral reason in
   particular shapes what gets looked for, and nobody re-reads it.
6. **Mark the transcript unverified** until a human has checked it against the
   paper. Put the mark in the file, not in your head.

Then, in `README.md` next to it, three sections:

- **Highlight** — the one thing that matters most in this document
- **What we analysed** — your reading, clearly separated from what the document says
- **Questions this document raises** — numbered, so you can point at them later

## What it caught in the worked example

Typing out the prescription revealed that the **"Any Allergies" field was blank** —
although the allergy was recorded in the same day's clinical notes, and the patient
had an indwelling catheter whose likeliest infection is reflexively treated with
exactly the drug class she reacts to. Nobody reading the prescription for its
*contents* would notice an empty field. Transcribing it structurally forced the
question "what goes here?"

Typing out the nerve study's header surfaced that the referral abstract read
**"post-radiation therapy"** — the investigation was framed around a presumed cause
before it was run. That line is at the top of page one and had been read past
perhaps a dozen times.

Typing out the data tables surfaced **two numbers that sat at the boundary of
normal and were summarised as normal**, and **one nerve named differently in the
summary than in the data**. All three are in the source. None is in any summary of it.
