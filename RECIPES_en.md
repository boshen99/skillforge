# Recipes — Five Quick Entry Points

> **How to use**: Pick the entry closest to your scenario → follow the guide for that entry → complete all seven steps
> **Core**: Each entry brings targeted questions for the seven operations (Search/Split/Stack/Expand/Balance/Verify/Complete)
> **Note**: The entry changes the questions you ask — not the operations. Seven steps remain the same.

---

## Choose Your Entry

```
┌─────────────────────────────────────────────────┐
│ My Skill...                                      │
│                                                  │
│ ├─ Is a node in a chain (collect/clean/pattern/insight) │
│ │      → Entry 1: Chain Node                     │
│                                                  │
│ ├─ Has its own upstream/downstream, not in chain │
│ │      → Entry 2: Independent Domain            │
│                                                  │
│ ├─ Is in a strategy chain (understand/change/hold)     │
│ │      → Entry 3: Strategy Chain                │
│                                                  │
│ ├─ Core is statistics (what) + insight (why)     │
│ │      → Entry 4: Analytics & Insight           │
│                                                  │
│ └─ Just want something simple, fast             │
│        → Entry 5: 5-Minute Quick Start          │
└─────────────────────────────────────────────────┘
```

---

## Entry 1: Chain Node

### When to use

```
Your Skill is part of:
  VOC chain: data-collection → data-etl → pattern-finder → voc-insight
  Or: extends a specific node (adds a sub-node)

Does it have clear upstream and downstream?
  Yes → Chain Node ✓
  No  → Might be independent → go to Entry 2
```

### Chain Node — Split questions (specific)

```
In addition to the three universal questions, also ask:

Q-L1: What data will upstream give me?
       → Most of Qian (Input) comes from here

Q-L2: What data does downstream need from me?
       → Most of Kun (Output) goes here

Q-L3: What would upstream/downstream most mistakenly think I can also do?
       → Key Yin rules for Gen (Boundary) grow from here

Q-L4: What is the data format of upstream/downstream?
       → Defines Xun (Flow) and Dui (Handshake) protocols
```

### Chain Node — Stack questions (specific)

```
Sun (Tools):
  Upstream uses what tools? → Do I need to be compatible?
  Downstream needs what tools? → Do I need to output in a format it can read?

Young Yang (Task Order):
  Do upstream/downstream Steps align?
  → Does my Step 1 correspond to which upstream output?
  → Does my last step correspond to which downstream input?

Kan (Risk):
  Upstream data fails? → Do I tolerate bad input or reject it?
  Downstream can't receive? → Do I wait or alert?
```

### Chain Node — Template

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Intent (Seed): ________________

【Split】
Yang:
  1. ___
  2. ___
  3. ___

Yin (source = AI overstepping / upstream-downstream boundary / human reservation):
  ✗ ___ (most likely overstepping)
  ✗ ___ (upstream/downstream scope)
  ✗ ___ (human reservation)

【Stack】
Sun: Tool 1, Tool 2, Tool 3
Young Yang: Step1 → Step2 → Step3
Young Yin: Judgment 1: ___?  Judgment 2: ___?
Dark: □ ___  □ ___

【Expand】
Qian (Input, from upstream): ___  ← key fill
Kun (Output, to downstream): ___  ← key fill
Zhen (Trigger): ___
Xun (Flow): ___ → downstream Skill
Kan (Risk): upstream fail→___  downstream fail→___
Li (Standard): ___
Gen (Boundary): ___  ← key fill (upstream/downstream scope)
Dui (Handshake): ___  ← key fill (format/trigger)

【Balance】
Metal→Wood: ___ (tools sufficient?)
Wood→Fire: ___ (tasks have judgment support?)
Fire→Water: ___ (judgment determines flow?)
Water→Earth: ___ (flow determines position?)
Earth→Metal: ___ (position determines tools?)

【Verify】
Breaks: ___ → go back to: ___
Breaks: ___ → go back to: ___

【Complete】
Split✓  Stack✓  Expand✓  Balance✓  Verify✓
Eight Dimensions: __/8
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Entry 2: Independent Domain

### When to use

```
Your Skill:
  □ NOT in VOC chain
  □ NOT in strategy chain
  □ Has its own upstream/downstream (or none at all)
  □ Does NOT share data format with other Skills

Examples: internal knowledge base, legal compliance, product specs, competitor monitoring
```

### Independent — Split questions (specific)

```
Q-I1: What does the user most fear AI will do?
       → This is Yin Rule #1

Q-I2: What are the professional judgments in this domain?
       → This determines how deep Young Yin (Judgment) needs to be

Q-I3: Who is responsible when things go wrong?
       → This determines how strict Dark (Gate) needs to be

Q-I4: Are there existing standards/norms in this domain?
       → This determines how to fill Li (Standard)
```

### Independent — Expand questions (specific)

```
Xun (Flow): No fixed downstream
  → Define: who reads this Skill's output after completion?
  → Could be: human users, external systems, scheduled triggers

Dui (Handshake):
  → No standard format — define your own protocol
  → Core three elements: what to output + who receives it + how to trigger
```

### Independent — Template

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Intent (Seed): ________________

【Split】
Yang: 1. ___  2. ___  3. ___
Yin:  ✗ ___ (what user fears AI doing)
      ✗ ___ (professional boundary)
      ✗ ___ (human reservation)

【Stack】
Sun: ___, ___, ___
Young Yang: Step1 → Step2 → Step3
Young Yin: Professional judgment 1: ___?  Judgment 2: ___?
Dark: □ meets domain standard  □ has traceable records

【Expand】
Qian: ___
Kun: ___
Zhen (Trigger): ___ (who/what triggers it)
Xun (Flow): No standard downstream  ← define your own: ___ → ___
Kan (Risk): Domain-specific exception 1: ___  Exception 2: ___
Li (Standard): ___ (domain norms)
Gen (Boundary): ___ (professional scope)
Dui (Handshake): output___  deliver to___  trigger___

【Balance】
Metal→Wood→Fire→Water→Earth
  Any breaks? → go back to: ___

【Verify】
Break: ___ → go back to: ___

【Complete】
Split✓  Stack✓  Expand✓  Balance✓  Verify✓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Entry 3: Strategy Chain

### When to use

```
Your Skill is in:
  L1 Understand — Where am I? (user insights / market analysis / category assessment)
  L2 Change — Where am I going? (reposition / validate hypotheses)
  L3 Hold — How do I keep it? (brand building / execution)

Are you making decisions or analyzing data?
  Decision-driven → Strategy Chain ✓
  Data-driven → Might not be strategy → go to Entry 1 or 4
```

### Strategy — Split questions (specific)

```
Q-S1: What can this level (L1/L2/L3) NOT skip to?
  L1: Cannot give execution advice (still in understanding phase)
  L2: Cannot skip validation and go straight to conclusion
  L3: Cannot give strategic options (already in execution phase)

Q-S2: What decisions must be left to humans?
  Strategic direction / resource allocation / make-or-break choices

Q-S3: Can your hypothesis be falsified?
  Yes → can enter L2  No → still in L1
```

### Strategy — Stack questions (specific)

```
L1 (Understand) Four Forces:
  Sun: interview tool, analysis tool, mapping tool
  Young Yang: collect insights → categorize → form understanding
  Young Yin: Does user really think this? Where's the evidence? Any counter-examples?
  Dark: □ data-supported  □ has categorization  □ has priority

L2 (Change) Four Forces:
  Sun: hypothesis tool, validation tool, decision tool
  Young Yang: propose hypothesis → design validation → confirm direction
  Young Yin: Is hypothesis bold enough? Can it be falsified? Is evidence sufficient?
  Dark: □ hypothesis clear  □ falsifiable  □ conclusions actionable

L3 (Hold) Four Forces:
  Sun: execution tool, monitoring tool, evaluation tool
  Young Yang: plan → allocate resources → execute
  Young Yin: Can plan be executed? Resources sufficient? Milestones defined?
  Dark: □ has execution plan  □ has milestones  □ has evaluation metrics
```

### Strategy — Template

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Intent (Seed): ________________
Level: □ L1 Understand  □ L2 Change  □ L3 Hold

【Split】
Yang: 1. ___  2. ___
Yin:  ✗ No skipping levels: ___ (L1→no exec advice / L2→no skip validation / L3→no strategy options)
      ✗ No mixing: ___
      ✗ Human reservation: ___

【Stack】
Sun (per L1/L2/L3 standard):
Young Yang (per L1/L2/L3 standard):
Young Yin (per L1/L2/L3 standard):
Dark (per L1/L2/L3 standard):

【Expand】
Qian: L1→market data+user insights+competitor info
      L2→L1 conclusions+hypothesis
      L3→L2 conclusions+resources
Kun:  L1→category understanding report+map
      L2→hypothesis+validation plan
      L3→brand plan+execution milestones
Xun: L1→L2  L2→L3  L3→execution team
Kan: hypothesis falsified→___  insufficient resources→___  wrong timing→___
Li: hypothesis falsifiable? conclusions actionable?
Gen: no level-skipping, no mixing, no overstepping
Dui: L1→L2, L2→L3, L3→execution team

【Balance】
All five links? → any breaks: ___

【Verify】
Break: hypothesis not bold enough→strengthen Young Yin
Break: milestones unclear→supplement Dark

【Complete】
Split✓  Stack✓  Expand✓  Balance✓  Verify✓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Entry 4: Analytics & Insight

### When to use

```
Your Skill's core is two layers:
  Layer 1: Statistics (what is happening)
  Layer 2: Insight (why is it happening)

Is the user asking "how many" or "why"?
  First ask how many → Analytics & Insight ✓
  Only ask what's there → might be collection/cleaning → go to Entry 1
```

### Analytics & Insight — Stack questions (specific)

```
Statistics Layer (Sun + Young Yang):
  Sun tools: frequency counter, co-occurrence analyzer, trend tool, comparison tool
  Young Yang: Step1 frequency → Step2 co-occurrence → Step3 trend/comparison

Insight Layer (Sun + Young Yang):
  Sun tools: root cause excavator, opportunity identifier, strategy generator
  Young Yang: Step4 from stats → hypothesize
              Step5 validate → find evidence
              Step6 form strategy → output recommendations

Core: Statistics conclusions → Insight layer inputs
  Not two separate Skills — one Skill with two-layer architecture
```

### Analytics & Insight — Young Yin (judgment) questions

```
J-H1: Is the statistical conclusion credible?
      → Sample size >= ___ records
      → Data sources traceable

J-H2: Does the insight have evidence?
      → Each insight >= 3 data points
      → No counter-examples (or counter-examples explained)

J-H3: Is the insight actionable?
      → Not generic talk
      → Has specific recommendation/direction

J-H4: Is the hypothesis bold enough?
      → Not an obvious fact
      → Has insight delta (something user doesn't know)
```

### Analytics & Insight — Four-Quadrant (core tool)

```
            High Satisfaction
                  │
   Competitor Strong │     Maintain Advantage
   (Learn from)       │     (Strengthen)
                      │
───────┬──────────────┼──────────────────── High Attention
                      │
   Low Priority        │     Act Immediately
   (Ignore)            │     (Opportunity)
                      │
                  Low Satisfaction

High Attention + Low Satisfaction = Act Now 🔥🔥🔥
High Attention + High Satisfaction = Maintain ⭐
Low Attention + High Satisfaction = Spread
Low Attention + Low Satisfaction = Defer
```

### Analytics & Insight — Template

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Intent (Seed): ___ analysis + insight

【Split】
Yang: Statistics layer (frequency/co-occurrence/trend of ___)
      Insight layer (why___ / where's opportunity / strategy)
Yin:  ✗ Do not modify raw statistical results
      ✗ Do not fabricate insights
      ✗ Do not skip statistics and give insights directly

【Stack】
Sun: stats tools (frequency/co-occurrence/trend/compare) + insight tools (root cause/opportunity/strategy)
Young Yang:
  Stats: Step1 frequency  Step2 co-occurrence  Step3 trend/compare
  Insight: Step4 stats→hypothesis  Step5 validate→evidence  Step6 strategy→recommendation
Young Yin:
  Stats: sample>=___  sources traceable
  Insight: each>=3pts  no counter-examples  has delta
  Quadrant: HighAtt+LowSat=Act Now, HighAtt+HighSat=Maintain...
Dark: □ stats credible  □ insights evidenced  □ actionable

【Expand】
Qian: cleaned structured data + analysis dimensions
Kun: stats report (JSON) + insight report (Markdown)
Xun: flows to voc-insight or directly to human users
Kan: insufficient sample→stop  no evidence→mark pending
Li: stats+insight double report, each insight with evidence
Gen: no data modification / no fabricated insights / no skip stats
Dui: stats output→insight input, insight→human/downstream

【Balance】
Metal→Wood: dual tool chain covers 6 steps ✓
Wood→Fire: stats steps support insight steps ✓
Fire→Water: insight judgment determines flow (to human or downstream) ✓
Water→Earth: flow determines position (analysis chain step 3-4) ✓
Earth→Metal: position requires stats+reasoning tools ✓

【Verify】
Break: stats conclusion unreliable→go back, increase sample
Break: insight has no evidence→go back, validate hypothesis

【Complete】
Split✓  Stack✓  Expand✓  Balance✓  Verify✓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Entry 5: 5-Minute Quick Start

### When to use

```
Your Skill:
  □ < 10 tools
  □ < 5 task steps
  □ Independent use, not in a chain
  □ Just needs to work

Don't chase completeness. Chase usability.
Don't chase optimal. Chase functional.
```

### 5-Minute Quick Start Template

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Intent (Seed): ___

【Split】 (30 sec)
Yang: 1. ___  2. ___
Yin:  ✗ ___  ✗ ___  ✗ ___

【Stack】 (1 min)
Sun: ___, ___, ___
Young Yang: Step1→Step2→Step3
Young Yin: ___?
Dark: □ ___

【Expand】 (1 min, minimum 3 fills)
Qian (Input): ___
Kun (Output): ___
Gen (Boundary): ___

【Balance】 (30 sec)
Metal→Wood→Fire→Water→Earth
  Tools sufficient? → ___ (Y/N)
  Judgment supported? → ___ (Y/N)
  Chain intact? → ___ (Y/N)
  If broken: ___ → fix: ___

【Complete】 ✓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  Split✓  Stack✓  Expand___/8  Balance✓/✗
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Entry Selection Decision Tree

```
Does your Skill have upstream/downstream?
│
├─ Yes, in VOC chain
│    → Entry 1 (Chain Node)
│    → Focus: Qian/Kun aligned with upstream/downstream
│
├─ Yes, in strategy chain
│    → Entry 3 (Strategy Chain)
│    → Focus: L1/L2/L3 level
│
├─ Yes, but not in any chain
│    → Entry 2 (Independent Domain)
│    → Focus: define your own handshake
│
└─ No, just one thing
     → Entry 5 (5-Minute Quick Start)
     → If it needs statistics + insight → Entry 4

Is your Skill core "what is it" or "why is it"?
├─ What (statistics) → Entry 1
├─ Why (insight) → Entry 4
└─ Both → Entry 4 (Analytics & Insight)
```

---

*This document is provided by skillforge — pick the right entry, fill it and you're done*
