# Causal graph — Patient A

```mermaid
graph TD
    subgraph SYM["What she experiences"]
        S1["Profound leg weakness<br/>can't lift legs into chair"]
        S2["Can't control sitting<br/>or lying down"]
        S3["~10 falls<br/>knees buckling"]
        S4["Urinary retention<br/>since M60"]
        S5["Constipation"]
        S6["Burning + numbness<br/>below both knees"]
        S7["Dizziness<br/>before the M60 fall"]
        S8["Worsening<br/>finger control"]
    end

    subgraph FIND["Objective findings"]
        F1["Reduced activation of<br/>normal motor units (EMG)"]
        F2["Posterior column<br/>dysfunction (SSEP)"]
        F3["Brisk arm reflexes"]
        F4["Absent ankle jerks"]
        F5["Normal muscle<br/>throughout (EMG)"]
        F6["Structurally normal<br/>cord (MRI)"]
    end

    subgraph MECH["Mechanism"]
        M1["Corticospinal tract<br/>weak descending signal"]
        M2["Posterior columns<br/>position sense lost"]
        M3["Cord involvement<br/>reaches the neck"]
        M4["Peripheral nerve<br/>involvement"]
        M5["Small-fibre damage"]
        M6["Autonomic?<br/>NOT EXPLAINED"]
    end

    subgraph DX["Candidate"]
        D1["MYELONEUROPATHY<br/>cord + nerve together"]
        D2["B12 / copper deficiency"]
        D3["Cervical myelopathy"]
        D4["Dural AV fistula"]
        D5["Chemo small-fibre<br/>neuropathy"]
    end

    S1 --> F1 --> M1 --> D1
    S2 --> F2 --> M2 --> D1
    S3 --> M1
    S3 --> M2
    S4 --> M1
    S5 --> M1
    S8 --> F3 --> M3 --> D1
    S6 --> F4 --> M4 --> D1
    S6 --> M5 --> D5
    S7 --> M6

    F5 -.->|"muscle is intact<br/>and trainable"| M1
    F6 -.->|"chemical, not<br/>mechanical damage"| D2

    D1 --> D2
    D1 --> D3
    D1 --> D4

    classDef orphan fill:#f7ecdd,stroke:#a1611f,stroke-width:3px,color:#000
    classDef lead fill:#e3f0e8,stroke:#3b7557,stroke-width:3px,color:#000
    class M6 orphan
    class D2 lead
```

## Reading it

**Convergence.** Every path arrives at one node — cord *and* peripheral nerve
affected together. Individually, the leg weakness pointed at the cord and the
burning feet pointed at the nerves, and they were being managed as separate
problems by separate specialists. As one node they have a name and a much shorter
differential than either symptom alone.

**The orphan.** `Dizziness before the M60 fall` (amber) has nothing pointing at it —
the only symptom in the file with no finding behind it. It generated a specific,
free, five-minute request: a lying-and-standing blood pressure.

**The load-bearing dotted line.** `Normal muscle throughout` explains no symptom, so
a symptom-by-symptom reading drops it. It is the most hopeful fact in the file: the
muscle is intact and under-driven, not wasted, so strength is recoverable if the
signal is restored.

## The same thing as an analogy

| Part | What it is | State |
|---|---|---|
| Control room | The brain | **Working** — cognition, speech, swallowing, eye movements all normal |
| Main cable | The spinal cord | **Damaged** — the main problem |
| Floor wiring | Nerves in the feet | **Also affected** — new at M63 |
| Motors | The muscles | **Healthy** — and trainable |
