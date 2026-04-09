# Principles — Seven Meta-Cognitive Operations, From Any Intent to Skill

> **Core**: Not a rule library, a meta-cognitive operation set
> **Seven Operations**: Search / Split / Stack / Expand / Balance / Verify / Complete
> **Any intent, processed through these seven steps, grows into a complete Skill**

---

## The Seven Meta-Cognitive Operations

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Search  → Search Existing    → Learn from real-world Skills first
Split   → Cut Yin/Yang      → What to do / What not to do
Stack   → Stack Four Forces → Tools / Tasks / Judgment / Gate
Expand  → Expand Eight Dims  → Input / Output / Trigger / Flow / Risk / Standard / Boundary / Handshake
Balance → Five Elements      → Metal→Wood→Fire→Water→Earth conduction chain
Verify  → Fix Breaks         → Find gaps, go back and fill
Complete→ Stop When Done      → Fill what's fillable, mark what's pending
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

These seven are not seven rules — they are seven ways of thinking.
Each can be used independently. Fill as much as you need.

---

## Step 0: Search — Search Existing Skills

```
Seed → Search

Before deriving, ask:
  Are there similar Skills online I can learn from?

What to search:
  □ GitHub — Claude Code Skills / other AI Agent skill libraries
  □ Hugging Face / Coze / Dify — agent workflows
  □ AirTable / Notion — skill collections
  □ Keywords: "[your intent] + Claude Skill / AI workflow / automation"

How to search:
  Use MindSearch or a search engine
  Keyword = [intent] + "Claude Skill" / "AI workflow" / "automation"

After searching:
  ┌─────────────────────────────────────────────┐
  │ Found similar Skill →                       │
  │                                             │
  │ Learn Point 1: Tool selection                │
  │   → Adjust "Stack" Sun (tools)              │
  │                                             │
  │ Learn Point 2: Task flow                    │
  │   → Adjust "Stack" Young Yang (task order) │
  │                                             │
  │ Learn Point 3: Exception handling            │
  │   → Supplement "Expand" Kan (risk)          │
  │                                             │
  │ Learn Point 4: Quality gate                 │
  │   → Adjust "Stack" Dark (gate thresholds)  │
  └─────────────────────────────────────────────┘

  No similar Skill found → Confirm the gap, derive from scratch
  → But at least know: what tools does this type use? What pitfalls exist?

Search output (feeds into later steps):
  = Tool candidate list (tools actually used in the wild)
  = Process reference template (how others do it)
  = Exception handling reference (pitfalls recorded)
  = Quality standard reference (industry default thresholds)
```

**Search Example:**

```
Intent: "Build a video production Skill"

Search process:
  Search "video production Claude Skill"
  → Found Claude Code's official ai-video-ad-workflow
  → Found MiniMax video generation Space on Hugging Face
  → Found KLING AI API docs and best practices

What was learned:
  Tools: MiniMax KLING / Runway / Pika Labs / FFmpeg
  Flow: script → storyboard → generate → post-production
  Pitfalls: malformed video / copyrighted music / duration limits
  Quality: thumbnail CTR / completion rate (post-hoc; production stage only checks visual quality)

Applied:
  → Sun (Tools): reference KLING API, not invented from scratch
  → Young Yang (Tasks): reference storyboard step, add "storyboard" after script
  → Kan (Risk): reference pitfall records, add "page structure change" handling
  → Dark (Gate): reference industry standards (duration / dimensions)
```

---

## Step 1: Split — Cut Yin/Yang

```
Seed → Two儀

Cut an intent into two halves:
  Yang: What this Skill must do
  Yin:  What this Skill must NOT do

How to cut?

Ask yourself three questions:

Q1: What would AI most easily overdo with this intent?
    → That's Yin Rule #1

Q2: What data/decisions in this stage belong to someone else's scope?
    → That's Yin Rule #2

Q3: What judgment must be left to humans?
    → That's Yin Rule #3

Q4 (optional): What would upstream/downstream Skills mistakenly think this one can do?
    → That's the boundary Yin Rule
```

**Split Example:**

Intent: "I want to analyze customer reviews"

```
AI overdoing: AI might modify raw data, fabricate reviews, skip quality checks for conclusions
→ ✗ Do not modify raw data
→ ✗ Do not fabricate or falsify review content
→ ✗ Do not skip data quality checks before giving conclusions

Scope question: Raw review data belongs to the collection stage
→ ✗ Do not collect data (that's another Skill's job)

Human judgment: Final verdict on individual reviews (positive or negative) may need human review
→ ✗ Do not make final qualitative decisions on single reviews

Yang: Count frequencies, find co-occurrence patterns, generate reports
```

---

## Step 2: Stack — Yin/Yang → Four Forces

```
Two儀 → Four Forces

Yang (what to do) + Yin (what not to do) = Four Forces

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Force           Derive from         Ask what?
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Sun (Tools)      Yang               What tools do I need?
Young Yang       Tools → Order      What comes first, what next?
Young Yin        Yin → Judgment     How to judge right/wrong at each step?
Dark (Gate)      Quality Standard   How to know it's done?
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

How to stack?

Sun (Tools):
  1. Take every Yang item
  2. Ask for each: what tool completes this?
  3. Merge: combine similar tools → final list 3–10 tools

Young Yang (Task Order):
  1. From tool list: which tool is most foundational (others depend on it)?
  2. Sort by dependency
  3. Result: Step 1 → Step 2 → Step 3 ...

Young Yin (Judgment):
  1. At each task step: what counts as right? What counts as wrong?
  2. Right proceeds, wrong handles in next step
  3. Result: Judgment 1, Judgment 2, Judgment 3 ...

Dark (Gate):
  1. From all judgments, extract final quality standards
  2. Ask: on delivery, what must absolutely be present?
  3. Result: Gate checklist (typically 2–4 items)
```

**Stack Example:**

Intent: "I want to analyze customer reviews"

```
Split result:
  Yang = count frequencies, find co-occurrence patterns, generate reports
  Yin  = don't modify data, don't fabricate, don't skip checks, don't collect, don't judge single reviews

Stack → Four Forces:

Sun (Tools):
  Count frequencies → counting tool
  Find co-occurrence → co-occurrence analysis tool
  Generate reports → report generation tool
  = 3 tools total

Young Yang (Task Order):
  Step 1: Receive cleaned data
  Step 2: Frequency statistics
  Step 3: Co-occurrence analysis
  Step 4: Generate report

Young Yin (Judgments):
  Judgment 1: Is the statistical result credible? (sample size >= ___)
  Judgment 2: Are co-occurrence relationships logical? (appear at least ___ times)
  Judgment 3: Does the report have data support? (each conclusion >= 3 data points)

Dark (Gate):
  □ Sample size sufficient
  □ Each insight has data support
  □ Raw data unmodified (traceable)
```

---

## Step 3: Expand — Four Forces → Eight Dimensions

```
Four Forces → Eight Dimensions

Each Force expands into two Dimensions:

Sun (Tools)       expand → Qian (Input) + Kun (Output)
Young Yang (Task) expand → Zhen (Trigger) + Xun (Flow)
Young Yin (Judge) expand → Kan (Risk) + Li (Standard)
Dark (Gate)       expand → Gen (Boundary) + Dui (Handshake)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Dimension    From Force    How to fill
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Qian        Sun           What data does this Skill receive?
Kun         Sun           What files does this Skill produce?
Zhen        Young Yang    Which task starts it?
Xun         Young Yang    Where does output go after completion?
Kan         Young Yin     What happens when a judgment fails?
Li          Young Yin      After all steps: what state means success?
Gen         Dark          What must never happen? (from Yin)
Dui         Dark          Who receives it, how?
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**Expand Example:**

Intent: "I want to analyze customer reviews"

```
From Split + Stack results:

Qian (Input, from Sun):
  = data-etl output path
  = Fields: platform, username, timestamp, content, rating, likes

Kun (Output, from Sun):
  = Statistics report (JSON): frequency stats + co-occurrence matrix
  = Insight report (Markdown): pain points / delights / opportunities

Zhen (Trigger, from Young Yang):
  = Step 1: read data file, begin frequency stats

Xun (Flow, from Young Yang):
  = output to voc-insight (stats + insight reports)

Kan (Risk, from Young Yin):
  = Judgment 1 fails (insufficient sample) → stop, output "insufficient sample, cannot analyze"
  = Judgment 2 fails (no logical co-occurrence) → skip co-occurrence, proceed with frequency only
  = Judgment 3 fails (no data support) → mark report conclusions "pending verification"

Li (Standard, from Young Yin):
  = Both stats and insight reports generated
  = Each insight has data evidence
  = Raw data unmodified

Gen (Boundary, from Dark):
  = Do not modify raw data
  = Do not collect new data
  = Do not make final qualitative judgments on single reviews

Dui (Handshake, from Dark):
  = Output to agreed directory
  = voc-insight triggers by reading that directory
  = Include metadata: processing time, sample size, insight count
```

---

## Step 4: Balance — Five Elements Dynamic Reasoning

```
Eight Dimensions → Five Elements

After filling Eight Dimensions, use Five Elements as a living dynamic reasoning framework —
not a checklist, but a chain of forces that generate and restrain each other.

Five Forces are not five labels — they are five powers:

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Force      Represents              Not
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Wood        Direction / Intent     "tasks" as a word
Fire        Judgment / Decision    "quality gate" as a word
Earth       Output / Deposit       "position" as a word
Metal       Tools / Structure      "tool list"
Water       Flow / Connection      "flow" as a word
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Mutual Generation = where power comes FROM:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Wood → Fire    Direction gives judgment its purpose
Fire → Earth   Judgment produces deposits (outputs)
Earth → Metal  Deposit shapes structure (tools)
Metal → Water  Structure enables flow (tasks → downstream)
Water → Wood   Flow creates new direction (extension)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Mutual Restraint = where power constrains:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Metal → Wood   Structure prunes over-scattered direction
Wood → Earth   Innovation breaks over-stable deposit
Earth → Water  Accumulation blocks flow
Water → Fire   Flow balances over-heated judgment
Fire → Metal   Decision reshapes rigid structure
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**Five Elements — correct way: not checking, asking**

```
Not asking: "Are tools sufficient? Are tasks ordered? Do judgments have thresholds?"

Instead asking:

Wood (Direction) → What is this Skill's core direction?
  → What pushes it forward (Water)? Is the push sufficient?
  → Does it have judgment support (Fire)?
  → Is it over-scattered (Metal → Wood over-restrained)?

Fire (Judgment) → Where does judgment come from?
  → Does it have directional support (Wood → Fire)?
  → Does it produce outputs (Fire → Earth)?
  → Is it over-rigid (Water → Fire over-cooling)?

Earth (Deposit) → What does this Skill produce?
  → Does the deposit become structure (Earth → Metal)?
  → Is it over-redundant / disordered (Wood → Earth over-restraining)?

Metal (Structure) → What are the tool boundaries?
  → Does structure enable flow (Metal → Water)?
  → Is structure over-rigid (Fire → Metal over-restraining)?

Water (Flow) → How is upstream/downstream connected?
  → Does flow create new direction (Water → Wood)?
  → Is flow over-scattered / blocked (Earth → Water over-restraining)?
```

**Symptoms of broken generation/restraint chains (not errors — imbalances):**

```
Wood → Fire broken:
  → Has intent but doesn't know how to act (direction exists, judgment doesn't)
  → Fire weak: judgment insufficient, thresholds vague

Fire → Earth broken:
  → Keeps judging but produces nothing (many judgments, no deposit)
  → Earth weak: output unclear, report quality low

Earth → Metal broken:
  → Has output but no standards form (result exists, structure doesn't)
  → Metal weak: tools unstandardized, flow fragmented

Metal → Water broken:
  → Has structure but no flow (tools exist, task flow doesn't)
  → Water weak: upstream/downstream don't connect, I/O mismatched

Water → Wood broken:
  → Flowed but no new direction (flowed, but no growth)
  → Wood weak: no extension presets, Skill dies once finalized

Metal → Wood broken:
  → Direction too scattered to execute (structure too weak to constrain direction)
  → Wood over Metal: wants too much, tools can't keep up

Fire → Metal broken:
  → Structure too rigid to adjust (judgment too hard, structure can't move)
  → Metal over Fire: standards locked, exceptions can't be handled
```

**Five Elements reasoning template (use after filling Eight Dimensions):**

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Wood (Direction):
  Where is this Skill going? → What are the extension presets?
  What pushes it (Water)? → Where does upstream come from? Is it sufficient?
  Does it have judgment support (Fire)? → Is it over-scattered?

Fire (Judgment):
  What is judgment's basis? → Where does judgment come from (Wood → Fire)?
  What does judgment produce (Earth)? → Is there deposit?
  Is judgment over-rigid? → Water → Fire? Is flow balanced?

Earth (Deposit):
  What is deposited? → Output file / insight / report
  Does deposit become structure (Metal)? → Are tools standardized?
  Is deposit blocking? → Wood → Earth? Is there innovation breakthrough?

Metal (Structure):
  What are the tool boundaries? → Yin rules
  Does structure allow flow (Water)? → Are upstream/downstream connected?
  Does structure limit growth? → Fire → Metal? Is it over-rigid?

Water (Flow):
  How are upstream/downstream connected? → Xun (Flow) + Dui (Handshake)
  Does it flow to new direction (Wood)? → Is there extension?
  Is it over-scattered / blocked? → Earth → Water? Too much deposit?
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**Five Elements full example — Competitor Price Monitoring:**

```
Wood (Direction):
  Skill direction: monitor competitors → support brand strategy
  Water → Wood: brand strategy as upstream, sets monitoring direction ✓
  Fire sufficient? 10% alert threshold → judgment clear ✓
  Metal → Wood: tool precision (parsing dynamic pages) ✓

Fire (Judgment):
  Judgment from Wood: collect → compare → alert, direction clear ✓
  Fire → Earth: judgment produces daily_report + alert ✓
  Earth sufficient? Two outputs (report + alert) ✓
  Water → Fire: alert deduplication mechanism ✓

Earth (Deposit):
  Deposits: daily report + price alert
  Earth → Metal: deposits become standards → output format fixed ✓
  Metal sufficient? Tools standardized (scraping/parsing/format) ✓
  Wood → Earth: new product detection = innovation breakthrough ✓

Metal (Structure):
  Tool boundaries: no price modification / no prediction / no cross-category
  Metal → Water: standards defined, upstream/downstream can connect ✓
  Water sufficient? Flow clear: alert → brand-strategy ✓
  Fire → Metal: threshold (10%) adjustable → structure not locked ✓

Water (Flow):
  Upstream/downstream: Independent Skill → brand-strategy
  Water → Wood: flow supports direction → monitoring informs strategy ✓
  Earth → Water: daily accumulation → historical comparison ✓
  Water sufficient? Direction clear, alert triggers downstream ✓

Five Elements pass, no breaks, no imbalance ✓
→ Derivation has no structural issues
```

---

## Step 5: Verify — Fix Imbalances

```
Imbalances found through Five Elements reasoning are fixed by going back and filling gaps.

Not a checklist — identify symptoms of five-force imbalance:

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Imbalance Symptom                      Five-Element Root    Fix
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Wants too much, achieves too little    Wood over Metal       Stack (Sun) strengthen boundaries
Always doing, never delivering         Fire over Earth       Stack (Young Yin) strengthen standards
Has output but it's scattered          Earth over Water      Expand (Kun) clarify output format
Output right, upstream/downstream blocked Metal over Water   Expand (Xun/Dui) define handshake
Upstream/downstream connected, no direction Water over Wood Verify (Wood) preset extension
Keeps judging but can't decide         Water → Fire overdone  Stack (Dark) tighten thresholds
Structure over-rigid to adjust         Fire → Metal overdone  Stack (Sun) relax forbidden boundaries
Direction over-scattered to execute    Metal → Wood overdone  Balance (Wood) focus extension direction
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**Verification flow (not a checklist — dynamic questions):**

```
1. Ask Wood (Direction):
   → Is there direction? Is it clear? (no direction = weak Wood)
   → Does it have extension presets? (no extension = Wood is dead)

2. Ask Fire (Judgment):
   → Does judgment have basis? Where does it come from? (no basis = weak Fire)
   → Is it over-rigid / over-loose? (over-rigid = Fire→Metal overdone / over-loose = Water→Fire overdone)

3. Ask Earth (Deposit):
   → Is there output? Is output clear? (no output = weak Earth)
   → Is it over-redundant / disordered? (disordered = Wood→Earth overdone)

4. Ask Metal (Structure):
   → Are tool boundaries clear? Over-rigid / over-loose? (over-rigid = Fire→Metal overdone / over-loose = Metal→Wood under-constraining)

5. Ask Water (Flow):
   → Upstream/downstream connected? Flow correct? (not connected = Metal→Water broken)
   → Is flow blocked / over-scattered? (blocked = Earth→Water overdone / scattered = Water→Wood under-generating)

Extension verification (every Skill must answer):
  □ Wood (Direction) defined? → No = Wood is dead, Skill dies once finalized
  □ What are Wood's extension directions? → Direction: ___ / ___ / ___
  □ What are the extension rules?
    → Light扩 (just fill Eight Dims) → Heavy扩 (back to Stack) → Architecture扩 (back to Balance)
  □ What are the extension gates?
    → New tools don't conflict / New tasks compatible / New output compatible with upstream/downstream
    → Extension gates: ___ / ___ / ___
```

**Verification pass criteria:**

```
Not "no floating tools" — that is a checklist.

Instead:
✓ Wood has direction, has extension presets
✓ Fire has basis, neither dead nor over-reactive
✓ Earth has output, neither excessive nor insufficient
✓ Metal has boundaries, neither rigid nor loose
✓ Water has flow, neither blocked nor scattered

Five Elements generate and restrain smoothly, forces balanced
→ Verification passes
```

---

## Step 6: Complete — Stop When Done

```
Derivation is complete when:

✓ Split: both Yin and Yang exist
✓ Stack: all Four Forces exist, tools/tasks/judgment/gate one-to-one
✓ Expand: at minimum Qian (Input), Kun (Output), Gen (Boundary) filled
✓ Balance: Metal→Wood→Fire→Water→Earth conduction chain intact
✓ Verify:
    Wood has direction, has extension presets ✓
    Fire has basis, neither dead nor over-reactive ✓
    Earth has output, neither excessive nor insufficient ✓
    Metal has boundaries, neither rigid nor loose ✓
    Water has flow, neither blocked nor scattered ✓
✓ Five Elements generate and restrain smoothly → Verify passes

Can fill or skip (depending on Skill complexity):
○ Remaining Eight Dimensions (Kan/Li/Dui/Zhen/Xun) — more complete = more robust
○ Five Elements mutual generation and restraint chains — more complete = clearer reasoning
○ More than 3 Yin rules — more = safer

Mark as pending (don't fill yet):
△ Upstream/downstream Skill doesn't exist yet → Xun/Dui marked "TBD"
△ Quantification unclear → Fire marked "needs business confirmation"
△ Extension direction uncertain → Wood marked "TBD"
△ Some Five Elements generation/restraint pair unclear → mark that pair "TBD"
```

---

## Full Derivation Example: Competitor Price Monitoring

### User says: "I want to monitor competitor prices"

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Step 0: Search (Search Existing Skills)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Search: "Claude video production skill" / "competitor monitoring workflow"
→ Found Claude Code's official ai-video-ad-workflow
→ Found some competitor monitoring scripts on GitHub

What was learned:
  Tools: KLING MiniMax / FFmpeg / diff tool (actually used)
  Flow: collect → compare → judge → report (verified)
  Pitfalls: dynamic page structure changes (already documented)
  Threshold: 10% change rate for alerts (industry convention)

→ Tool selection references KLING, not invented from scratch
→ Task order references actual flow, add "diff" step
→ Risk references pitfalls, add "page structure change" handling

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Step 1: Split (Yin/Yang)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

AI overdoing:
  AI might modify competitor price data
  AI might predict future price trends
  AI might scrape unrelated product categories
→ ✗ Do not modify raw price data
→ ✗ Do not predict price trends
→ ✗ Do not cross-category scraping

Scope:
  Raw prices belong to competitor websites; monitoring is read-only
→ ✗ Do not scrape content requiring login/payment

Human judgment:
  Whether prices are reasonable or trigger business decisions
→ ✗ Do not make business judgments on prices (record only, no buy/sell advice)

Yang:
  1. Periodically collect competitor prices
  2. Record changes (up/down/flat)
  3. Trigger alerts above threshold
  4. Generate daily report

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Step 2: Stack (Four Forces)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Sun (Tools):
  Collect prices → web scraping tool
  Record changes → diff comparison tool
  Trigger alerts → threshold judgment + notification tool
  Generate report → report generation tool
  = 4 tools

Young Yang (Task Order):
  Step 1: Trigger collection (scheduled)
  Step 2: Collect competitor prices
  Step 3: Compare with last record (diff)
  Step 4: Threshold judgment (alert or not)
  Step 5: Generate report

Young Yin (Judgments):
  Judgment 1: Did we collect it? → fields >= 5 (name/price/spec/promo/time)
  Judgment 2: Any changes? → any field differs from last record
  Judgment 3: Trigger alert? → change > 10%, or new product / discontinued

Dark (Gate):
  □ Daily prices recorded
  □ Changes have comparison data
  □ Alerts have basis

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Step 3: Expand (Eight Dimensions)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Qian (Input): competitor model list + last price record
Kun (Output): daily_price_report.json + price_alert.md
Zhen (Trigger): Step 1 trigger collection
Xun (Flow): flows to brand-strategy (price is strategic input)
Kan (Risk): rate limit→pause 10min switch source; page structure changed→log error
Li (Standard): daily records exist, changes have comparison, alerts have screenshots
Gen (Boundary): no modification, no prediction, no cross-category, no paid content
Dui (Handshake): report to agreed directory, brand strategy team reads

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Step 4: Balance (Five Elements)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Wood (Direction):
  Skill direction: monitor competitors → support brand strategy
  Water → Wood: brand strategy as upstream, sets direction ✓
  Fire sufficient? 10% alert threshold → judgment clear ✓
  Metal → Wood: tool precision (parsing dynamic pages) ✓

Fire (Judgment):
  Judgment from Wood: collect → compare → alert, direction clear ✓
  Fire → Earth: judgment produces daily_report + alert ✓
  Earth sufficient? Two outputs ✓
  Water → Fire: alert deduplication mechanism ✓

Earth (Deposit):
  Deposits: daily report + price alert
  Earth → Metal: deposits become standards → output format fixed ✓
  Metal sufficient? Tools standardized ✓
  Wood → Earth: new product detection = innovation ✓

Metal (Structure):
  Tool boundaries: no modification / no prediction / no cross-category / no paid content
  Metal → Water: standards defined, upstream/downstream connect ✓
  Water sufficient? Flow clear: alert → brand-strategy ✓
  Fire → Metal: threshold (10%) adjustable → structure not locked ✓

Water (Flow):
  Upstream: none (independent) → Downstream: brand-strategy
  Water → Wood: flow supports direction → monitoring informs strategy ✓
  Earth → Water: daily accumulation → historical comparison ✓
  Water sufficient? Direction clear, alert triggers downstream ✓

Five Elements pass, no breaks, no imbalance ✓

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Step 5: Verify
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Floating tools? → none ✓
□ Unowned tasks? → none ✓
□ Judgment thresholds quantified? → Yes, 10% ✓
□ Upstream/downstream connected? → upstream=none (independent), downstream=brand-strategy ✓
□ Wood (Direction) clear? → Extension presets: multi-category monitoring / API integration / historical trend analysis ✓
□ Fire (Judgment) has basis? → 10% threshold, judgment clear ✓
□ Earth (Deposit) has output? → Daily report + alert, output fixed ✓
□ Metal (Structure) has boundaries? → 5 Yin rules, boundaries clear ✓
□ Water (Flow) connected? → Flow clear, alert triggers downstream ✓

Five Elements generate and restrain smoothly, no breaks, no imbalance ✓
→ Derivation has no structural issues

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Step 6: Complete ✓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Split ✓  Stack ✓  Expand ✓  Balance ✓  Verify ✓

Eight Dimensions: 8/8 filled ✓
Yin rules: 5 (>3) ✓
Tools: 4 (in 3–10 range) ✓
Task steps: 5 ✓
Quantified judgments: 3 ✓
Extension presets: direction + rules + gates ✓

→ Derivation complete!
→ Five Elements generate and restrain smoothly ✓
```

---

## Seven Operations Overview

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Intent
  │
  ├─ Search → Search existing Skills (GitHub/HF/Coze etc.)
  │           ↓ Search found → learn tools/process/exceptions/thresholds
  │           ↓ No match → confirm gap, derive from scratch
  │
  ├─ Split  → Yin/Yang (what / what not)
  │           ↓
  ├─ Stack  → Four Forces (tools / tasks / judgment / gate)
  │           ↓
  ├─ Expand → Eight Dimensions (input / output / trigger / flow / risk / standard / boundary / handshake)
  │           ↓
  ├─ Balance→ Five Elements (Metal→Wood→Fire→Water→Earth) conduction chain
  │           ↓
  ├─ Verify → Find breaks, go back and fill
  │           ↓
  └─ Complete → Stop when done (all five forces balanced)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Meta-Cognition vs Rule Library

```
Rule library thinking:
  Encounter "collection" → use tool list A
  Encounter "analysis" → use tool list B
  Encounter "generation" → use tool list C
  → Always limited to what you pre-programmed

Meta-cognitive thinking:
  Encounter any intent → ask yourself seven questions
  Search: what's already out there? → learn from the real world
  Split: cut into Yin/Yang → know the boundaries
  Stack: stack into Four Forces → derive tools/tasks/judgment/gate
  Expand: expand into Eight Dimensions → complete the definition
  Balance: Five Elements dynamic reasoning → verify conduction chain
  Verify: fill gaps → fix what breaks
  Complete: stop when done → enough is enough

→ Any intent can be derived. Derivation power is not pre-limited.
→ Search makes derivation grounded in real-world experience, not invented in a vacuum
```

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| v5.3 | 2026-04-08 | Complete rewrite aligned with Chinese v5.3: Seven operations (not six), Step 0 added, same derivation example as Chinese (competitor price monitoring), no mixed pinyin, formal vocabulary throughout |
| v4.x | 2026-04-08 | Pre-v5.3 draft (outdated, do not reference) |

---

*This document is provided by skillforge — giving you meta-cognition, not a rule library*
