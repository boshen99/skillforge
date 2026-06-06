# SkillForge

> **Turn any intent into a complete, executable AI Skill.**

Give SkillForge an idea — *I want to monitor competitor prices* — and it walks you through 7 questions to derive a complete Skill with tools, tasks, judgments, and quality gates.

```yaml
Input:  One sentence of intent
Output: A complete, runnable Skill
Time:   15-30 minutes
```

---

## 30 Seconds: The Problem & The Solution

**The problem** — You have an idea for an AI Skill. You're not sure:
- Which tools you need
- What order to run them in
- Where this Skill sits in your pipeline
- What it should *never* do
- How to know it's working

**The solution** — Answer 7 questions. Get a complete Skill with:
- **3-10 tools** it needs
- **5-10 ordered task steps** to follow
- **2-5 quantified judgments** (with thresholds, not vibes)
- **3-5 quality gates** to know it's done
- **3+ forbidden actions** so it doesn't go off the rails
- **3+ extension directions** so it grows when you need

---

## 30 Minutes: The Seven Questions

```
                    ┌─────────────────────────────────┐
                    │           YOUR INTENT            │
                    │  "I want to monitor competitor  │
                    │   prices" / "triage GitHub       │
                    │   Issues" / "build a CRM"        │
                    └──────────────┬──────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  0. SEARCH  — What's already out there?  │
              │  GitHub / HuggingFace / Coze / Dify      │
              │  Learn: tools · flow · pitfalls · thresholds│
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  1. SPLIT  — Yin / Yang                  │
              │  (What to DO / What to NEVER do)         │
              │  Do: periodic collect / record / alert   │
              │  Don't: modify data / predict / cross-collect│
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  2. STACK  — Four Forces                  │
              │  Sun (Tools) · Young Yang (Tasks)         │
              │  Young Yin (Judgments) · Dark (Gates)     │
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  3. EXPAND  — Eight Dimensions            │
              │  Qian (Input) · Kun (Output)              │
              │  Zhen (Start) · Xun (Next)                │
              │  Kan (Errors) · Li (Success)              │
              │  Gen (Boundaries) · Dui (Handoff)         │
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  4. BALANCE  — Five Elements              │
              │  Wood (Direction) → Fire (Judgment)       │
              │  → Earth (Output) → Metal (Structure)    │
              │  → Water (Flow)                           │
              │  Check: chain intact? any weak link?      │
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  5. VERIFY  — Find the breaks             │
              │  Over-scattered direction? Over-rigid      │
              │  judgment? Output blocking flow?          │
              │  Go back to Step 2 / 3 / 4 and fix it     │
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  6. COMPLETE  — Done when                 │
              │  All five forces balanced                 │
              │  Extension directions defined             │
              │  No floating tools or orphan tasks        │
              └──────────────────────────────────────────┘
```

**Result: a complete, executable Skill** — specific to your intent, not a generic template.

> Don't know what the Chinese terms mean? See [The Terms in Plain English](#the-terms-in-plain-english) below.

---

## Real Examples (Built With This Framework)

| Intent | Skill Output | Walkthrough |
|--------|--------------|-------------|
| Monitor competitor prices | 4 tools · 5 steps · 3 judgments | See [PRINCIPLES.md](PRINCIPLES.md) § "完整走一遍" |
| **Auto-triage GitHub Issues** | 4 tools · 6 steps · 5 judgments · 8 forbidden | [examples/01-github-issue-auto-triage.md](examples/01-github-issue-auto-triage.md) |

**Each example walks the full 7-step process** — search, split, stack, expand, balance, verify, complete — and ends with a copy-paste-ready `SKILL.md`.

---

## Five Elements: Not Labels, Forces

The Five Elements are a **dynamic reasoning system** — not a checklist. They ask: *what forces are at play, and which one is weak or overdone?*

```
Mutual Generation — where power comes FROM:
  Wood → Fire    Direction gives judgment its purpose
  Fire → Earth   Judgment produces outputs
  Earth → Metal  Outputs shape structure
  Metal → Water  Structure enables flow
  Water → Wood   Flow creates new direction

Mutual Restraint — where power constrains:
  Metal → Wood   Structure prunes over-scattered direction
  Wood → Earth   Innovation breaks over-stable output
  Earth → Water  Accumulation blocks flow
  Water → Fire   Flow balances over-heated judgment
  Fire → Metal   Decision reshapes rigid structure
```

**Wrong way**: *"Check: are tools sufficient? Are tasks ordered?"*
**Right way**: *"Is direction over-scattered? Is judgment over-rigid? Is output accumulating and blocking flow?"*

---

## The Terms in Plain English

SkillForge borrows imagery from Chinese cosmology — 八八八 (bagua) and 五行 (wuxing). These are not mystical; they're compact labels for reasoning patterns. Here's what they actually mean:

| Chinese | Literal | Plain English |
|---------|---------|---------------|
| **太极** (Taiji) | Supreme ultimate | The seed intent you start with |
| **阴阳** (Yin-Yang) | Dark-Light | **What to do / What never to do** |
| **四象** (Sixiang) | Four Images | **Tools / Tasks / Judgments / Quality gates** |
| **乾 Qian** (Heaven) | Creative | **Input** — what data the Skill receives |
| **坤 Kun** (Earth) | Receptive | **Output** — what files/messages it produces |
| **震 Zhen** (Thunder) | Arousing | **Starting task** — the first step |
| **巽 Xun** (Wind) | Gentle | **Flow** — where output goes next |
| **坎 Kan** (Water) | Abyss | **Errors** — what to do when things break |
| **离 Li** (Fire) | Clinging | **Success criteria** — how to know it's done |
| **艮 Gen** (Mountain) | Stillness | **Boundaries** — what it must never do |
| **兑 Dui** (Lake) | Joyous | **Handoff** — protocol for the next Skill |
| **木 Wood** | — | **Direction** — where this Skill is heading |
| **火 Fire** | — | **Judgment** — the decision-making power |
| **土 Earth** | — | **Output** — what gets produced |
| **金 Metal** | — | **Structure** — the tools and boundaries |
| **水 Water** | — | **Flow** — how Skills connect |

If you only remember two things:

> **Eight Dimensions** = where the Skill lives in the world (input/output/flow/errors/etc.)
> **Five Elements** = the forces at play inside the Skill (direction/judgment/output/structure/flow)

---

## Seven Operations at a Glance

| # | Operation | Asks | Output |
|---|-----------|------|--------|
| 0 | **Search** | What already exists? | Tool candidates · flow references · pitfalls · thresholds |
| 1 | **Split** | What to do vs. not do? | Yin (forbidden) + Yang (do) |
| 2 | **Stack** | What forces are needed? | Tools / Tasks / Judgment / Gate |
| 3 | **Expand** | Where does it sit? | Eight Dimensions (Input/Output/Flow/Errors/...) |
| 4 | **Balance** | Is the chain intact? | Five Elements reasoning (Direction/Judgment/Output/Structure/Flow) |
| 5 | **Verify** | Where does it break? | Go back to Step 2 / 3 / 4, fill the gap |
| 6 | **Complete** | Is it done? | Full Skill with extension presets |

---

## Five Entry Points

Pick the entry that fits your scenario:

| Entry | When to Use |
|-------|-------------|
| **Chain Node** | Your Skill is a node in a pipeline (collect → clean → analyze → insight) |
| **Independent Domain** | Your Skill has its own upstream/downstream, not part of any chain |
| **Strategy Chain** | Your Skill operates in L1 (understand) / L2 (change) / L3 (hold) |
| **Analytics & Insight** | Your Skill has a statistics layer + an insight layer (what + why) |
| **5-Minute Quick Start** | Under 10 tools, under 5 steps, independent use, just want it to work |

See [RECIPES.md](RECIPES.md) for full entry point guides with specific questions for each step.

---

## File Structure

```
skillforge/
├── README.md              ← You are here
├── SKILL.md               ← Entry point (7-step table + quality checklist)
├── PRINCIPLES.md          ← Full framework (Chinese)
├── PRINCIPLES_en.md       ← Full framework (English)
├── RECIPES.md             ← Five entry points (Chinese)
├── RECIPES_en.md          ← Five entry points (English)
├── examples/              ← End-to-end walkthroughs
│   └── 01-github-issue-auto-triage.md
├── diagram.svg            ← Visual seven-step flow + five forces
├── LICENSE                ← MIT
├── CONTRIBUTING.md        ← Contribution guide
└── .github/
    └── ISSUE_TEMPLATE/    ← Bug report + feature request templates
```

---

## Who Built Skills With This

| Skill | Description |
|-------|-------------|
| [wechat-publisher](https://github.com/anthropics/claude-code/tree/main/.claude/skills/wechat-publisher) | Auto-generate WeChat articles with AI-generated images |

*Have a Skill you built with this framework? Open a PR to add it here.*

---

## License

MIT — use freely, modify freely, contribute freely.

---

*SkillForge — giving you meta-cognition, not a rule library.*
