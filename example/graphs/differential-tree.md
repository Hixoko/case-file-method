# Differential tree — Patient A

Built **backwards from the tests**, which is what makes the decision points visible.

```mermaid
graph TD
    ROOT["Myeloneuropathy<br/>cord + peripheral nerve"]

    ROOT --> B12["B12 / copper deficiency<br/>LEADING"]
    ROOT --> CERV["Cervical myelopathy"]
    ROOT --> FIST["Dural AV fistula"]
    ROOT --> OTH["Inflammatory / autoimmune"]

    B12 --> T1{"Bloods drawn BEFORE<br/>the supplement?"}
    T1 -->|Yes| R1["B12 + MMA + homocysteine<br/>+ copper/ceruloplasmin/zinc<br/>→ ANSWERS IT"]
    T1 -->|No| R2["Serum B12 falsely normal<br/>→ needs MMA + homocysteine<br/>to salvage"]

    CERV --> T2["Cervico-dorsal MRI<br/>ORDERED"]
    T2 --> R3["Compression seen or not<br/>→ often surgically treatable"]

    FIST --> T3{"Same MRI<br/>WITH CONTRAST?"}
    T3 -->|Yes| R4["Fistula seen or excluded<br/>→ CURABLE, one procedure"]
    T3 -->|No| R5["Stays invisible<br/>exactly as at M60"]

    OTH --> T4["CK, ANA, HLA-B27<br/>ORDERED"]
    T4 --> R6["Screens out connective-tissue<br/>and spondyloarthropathy"]

    classDef risk fill:#f8e6e4,stroke:#95322f,stroke-width:3px,color:#000
    classDef good fill:#e3f0e8,stroke:#3b7557,stroke-width:2px,color:#000
    classDef warn fill:#f7ecdd,stroke:#a1611f,stroke-width:2px,color:#000
    class R2,R5 risk
    class R1,R3,R4 good
    class T1,T3 warn
```

## What the backwards view revealed

Two of the four branches hang on **diamonds, not on new tests**. The tests were
already ordered. What was undecided was a condition attached to each:

| Decision | Action | Cost | If missed |
|---|---|---|---|
| Bloods before the supplement | Draw blood first | Free — a sequencing decision | The most treatable candidate is crossed off for the wrong reason, and it looks like a normal result |
| Contrast on the MRI | One phone call | Free | The only *curable* candidate stays invisible |

**Drawn forwards**, the situation reads: *we have ordered the right tests and are
waiting for results.*

**Drawn backwards**, it reads: *two free actions this week decide whether these
results mean anything.*

That difference is the entire argument for drawing the tree.

## Prune order

If you can only chase one thing:

1. **Bloods before supplement** — cheapest, most reversible if positive, and the one
   actively being lost right now.
2. **Contrast on the scan** — one call, and the only curable candidate.
3. Everything on [`../analysis/gaps.md`](../analysis/gaps.md).
