# Skill Factory

> **From any intent to a complete Skill in seven steps**

A meta-cognitive framework for deriving AI agent skills from first principles. Not a rule library — you bring the intent, it guides the thinking.

**Seven Meta-Cognitive Operations**: Search → Split → Stack → Expand → Balance → Verify → Complete

---

## What is this?

Skill Factory solves a specific problem: you have an intent ("I want to do X with an AI agent"), and you need a complete, executable Skill — with tools, task steps, judgment criteria, quality gates, and extension presets.

It does not give you a template. It gives you seven operations that force you to think through every dimension of a Skill. The output is always specific to your intent, never generic.

## Quick Start

```
Intent: "I want to monitor competitor prices"

Step 0: Search
  Search "competitor monitoring Claude Skill" / "AI workflow"
  → Learn tools, flow, pitfalls, thresholds from existing work

Step 1: Split (Yin/Yang)
  AI overdoes: modify data, predict trends, over-collect
  → Yin: no modification, no prediction, no cross-category
  Yang: periodic collect, record changes, trigger alerts, daily report

Step 2: Stack (Four Forces)
  Sun (Tools): scraper, diff tool, alert threshold, report generator
  Young Yang: Step1 trigger → Step2 collect → Step3 diff → Step4 judge → Step5 report
  Young Yin: collected? (fields >= 5), changed? (any diff), alert? (>10% or new/discontinued)
  Dark: □ daily record □ diff data □ alert evidence

Step 3: Expand (Eight Dimensions)
  Qian (Input): competitor model list + last price record
  Kun (Output): daily_price_report.json + price_alert.md
  Xun (Flow): → brand-strategy
  Gen (Boundary): no modification / no prediction / no cross-category / no paid content

Step 4: Balance (Five Elements)
  Wood (Direction): monitor → support brand strategy ✓
  Fire (Judgment): 10% threshold, judgment clear ✓
  Earth (Deposit): daily report + alert ✓
  Metal (Structure): tool boundaries clear ✓
  Water (Flow): flow clear, alert → downstream ✓

Step 5: Verify
  → No floating tools, no vague thresholds, upstream/downstream connected ✓
  → Extension presets defined: multi-category / API / historical trend ✓

Step 6: Complete ✓
  Tools: 4  |  Task steps: 5  |  Judgments: 3 quantified  |  Yin rules: 5
```

**Done.** That's a complete Skill — not a template, a derivation.

---

## Seven Operations

| Step | Operation | Asks | Outputs |
|------|-----------|------|---------|
| 0 | **Search** | What already exists? | Tools / flow / pitfalls / thresholds |
| 1 | **Split** | What to do vs. not do? | Yin (forbidden) + Yang (do) |
| 2 | **Stack** | What forces are needed? | Tools / Tasks / Judgment / Gate |
| 3 | **Expand** | Where does it sit? | Eight Dimensions (Qian/Kun/Zhen/Xun/Kan/Li/Gen/Dui) |
| 4 | **Balance** | Is the chain intact? | Five Elements (Metal/Wood/Fire/Water/Earth) |
| 5 | **Verify** | Where does it break? | Fill gaps, back to Step 2/3/4 |
| 6 | **Complete** | Is it done? | Full Skill ✓ |

---

## Five Entry Points

| Entry | When to Use |
|-------|-------------|
| **Chain Node** | Your Skill is a node in a pipeline (collect/clean/analyze/insight) |
| **Independent Domain** | Your Skill has its own upstream/downstream, not in a chain |
| **Strategy Chain** | Your Skill is in L1 (understand) / L2 (change) / L3 (hold) |
| **Analytics & Insight** | Your Skill has a statistics layer + an insight layer |
| **5-Minute Quick Start** | Under 10 tools, under 5 steps, independent use |

See [RECIPES.md](RECIPES.md) for the full entry point guides.

---

## Five Elements (Metal/Wood/Fire/Water/Earth)

The Five Elements are not labels — they are five forces with generation and restraint relationships:

**Mutual Generation** (where power comes from):
- Wood → Fire: Direction gives judgment its purpose
- Fire → Earth: Judgment produces outputs
- Earth → Metal: Outputs shape structure
- Metal → Water: Structure enables flow
- Water → Wood: Flow creates new direction

**Mutual Restraint** (where power constrains):
- Metal → Wood: Structure prunes over-scattered direction
- Wood → Earth: Innovation breaks over-stable outputs
- Earth → Water: Accumulation blocks flow
- Water → Fire: Flow balances over-heated judgment
- Fire → Metal: Decision reshapes rigid structure

Use these to ask dynamic questions, not to check boxes. See [PRINCIPLES.md](PRINCIPLES.md) for the full reasoning framework.

---

## Files

```
skill-factory/
├── README.md              ← You are here (English)
├── SKILL.md               ← Entry point with seven-step table + quality checklist
├── PRINCIPLES.md          ← Full meta-cognitive operations (Chinese)
├── PRINCIPLES_en.md       ← Full meta-cognitive operations (English)
├── RECIPES.md             ← Five entry points (Chinese)
├── RECIPES_en.md          ← Five entry points (English)
├── LICENSE                ← MIT License
├── CONTRIBUTING.md        ← Contribution guide
└── .github/               ← Issue templates
```

---

## Example Skills Built with This Framework

| Skill | Description |
|-------|-------------|
| [wechat-publisher](https://github.com/anthropics/claude-code/tree/main/.claude/skills/wechat-publisher) | Auto-generate WeChat articles with AI images |

---

## License

MIT License — use freely, modify freely, contribute freely.

---

*This framework gives you meta-cognition, not a rule library.*
