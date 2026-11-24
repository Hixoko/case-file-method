# 3 — Causal graph

**Symptom → finding → mechanism → candidate. Then look for the orphans.**

## What it is

A directed graph with four layers. Every symptom the patient has, traced through
to a candidate explanation — or left visibly dangling if nothing explains it.

```
What she experiences  →  Objective findings  →  Mechanism  →  Candidate
```

## When it pays

When you have more than two documents and more than three symptoms, and the
symptoms are being treated as a list rather than a system.

The specific value is **negative**: it makes visible the symptoms that nothing
accounts for. Those are usually either a second condition, or the clue to the first.

## How to run it

1. **Layer 1 — every symptom**, in the patient's own words where possible. Not the
   clinical paraphrase. "Can't control sitting down" carries more than "impaired
   proprioception", because it tells you what she notices.
2. **Layer 2 — every objective finding** across all documents. Test results,
   examination findings, imaging. Only things someone measured.
3. **Layer 3 — mechanism.** What would have to be true for that finding to produce
   that symptom. This is the layer where you will need to look things up, and the
   layer where a model is most useful and most dangerous. Cite your sources.
4. **Layer 4 — candidates.** What conditions produce that mechanism.
5. **Draw the edges.** Then look at what has no incoming edge.

## Reading the finished graph

Three things to look for, in order:

**Orphan symptoms** — nothing in layer 2 points at them. Either a finding is
missing (a test nobody ordered), or there is a second process. Both are worth a
question. In the worked example exactly one symptom was an orphan, and it pointed
straight at a five-minute bedside test nobody had done.

**Convergence** — many paths arriving at one node. That node is your centre of
gravity. If eight symptoms route through one mechanism, that mechanism is the case.

**Load-bearing dotted lines** — the findings that constrain rather than cause. "The
muscle is healthy" does not explain a symptom; it rules out a whole branch and
tells you what is recoverable. These are easy to leave out and worth drawing.

## What it caught in the worked example

Everything converged on a single node: **cord and peripheral nerve damaged
together**. Individually, the leg weakness pointed at the cord and the burning feet
pointed at the nerves, and the two were being managed as separate problems by
separate specialists. Drawn as a graph, they are one node, and that node has a
name and a much shorter differential than either symptom alone.

The orphan was dizziness immediately preceding the index fall. Nothing in any
report addressed it. It is the only symptom in the file with no finding behind it,
and it generated a specific, free, five-minute question for the next appointment.

The load-bearing dotted line was **"normal muscle throughout"** — meaning the
muscle is intact and under-driven, not wasted. That is the most hopeful fact in the
file and it is not a symptom explanation, so a symptom-by-symptom reading drops it
entirely.

## Rendering it

Mermaid `graph TD` with `subgraph` per layer. Use a `classDef` to colour orphans
distinctly — the point of the diagram is that they stand out.
