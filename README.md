# SkillForge

> **Give it any intent. Get back a complete, executable Skill.**

A meta-cognitive framework for deriving AI agent Skills — not a template library, not a rule set. You bring the intent, it guides the thinking. From a one-line idea to a full Skill with tools, task steps, judgment criteria, quality gates, and extension presets.

---

## The Seven Steps

```
                    ┌─────────────────────────────────┐
                    │           YOUR INTENT            │
                    │  "I want to monitor competitor  │
                    │   prices" / "build a CRM" /   │
                    │   "automate report generation"  │
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
              │  What must this Skill DO?                  │
              │  What must it NEVER do?                    │
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  2. STACK  — Four Forces                  │
              │  Sun (Tools) · Young Yang (Tasks)          │
              │  Young Yin (Judgments) · Dark (Gates)      │
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  3. EXPAND  — Eight Dimensions            │
              │  Qian · Kun · Zhen · Xun                   │
              │  Kan · Li · Gen · Dui                      │
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  4. BALANCE  — Five Elements              │
              │  Metal → Wood → Fire → Water → Earth       │
              │  Mutual generation & mutual restraint       │
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  5. VERIFY  — Find the breaks            │
              │  Which force is weak / overdone?          │
              │  Go back to Step 2 / 3 / 4 and fix it     │
              └──────────────────┬───────────────────────┘
                                   ▼
              ┌──────────────────────────────────────────┐
              │  6. COMPLETE  — Done when                │
              │  All forces balanced · Extension presets   │
              │  defined · Five elements generate &        │
              │  restrain smoothly                         │
              └──────────────────────────────────────────┘
```

**Result: a complete, executable Skill** — specific to your intent, not a generic template.

---

## Quick Example

Given the intent: *"I want to monitor competitor prices"*

| Step | Output |
|------|--------|
| **Search** | Found: similar skills use scraper + diff + alert threshold |
| **Split** | Do: periodic collect / record changes / trigger alerts / daily report. Don't: modify data / predict / cross-collect |
| **Stack** | 4 tools · 5 task steps · 3 quantified judgments · 5 Yin rules |
| **Expand** | Input: competitor list + last record. Output: `daily_report.json` + `price_alert.md`. Flow: → brand-strategy |
| **Balance** | Wood (direction) → Fire (10% threshold) → Earth (report + alert) → Metal (boundaries) → Water (flow) — all connected |
| **Verify** | No floating tools · Thresholds quantified · Extension presets defined |
| **Complete** | **4 tools · 5 steps · 3 quantified judgments** |

Done in ~15 minutes, not hours.

---

## Five Elements: Not Labels, Forces

The Five Elements are a dynamic reasoning system — not a checklist:

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

**Wrong**: "Check: are tools sufficient? Are tasks ordered?"
**Right**: "Is direction over-scattered? Is judgment over-rigid? Is output accumulating and blocking flow?"

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

## Seven Operations at a Glance

| # | Operation | Asks | Output |
|---|-----------|------|--------|
| 0 | **Search** | What already exists? | Tool candidates · flow references · pitfalls · thresholds |
| 1 | **Split** | What to do vs. not do? | Yin (forbidden) + Yang (do) |
| 2 | **Stack** | What forces are needed? | Tools / Tasks / Judgment / Gate |
| 3 | **Expand** | Where does it sit? | Eight Dimensions (Qian/Kun/Zhen/Xun/Kan/Li/Gen/Dui) |
| 4 | **Balance** | Is the chain intact? | Five Elements reasoning (Metal/Wood/Fire/Water/Earth) |
| 5 | **Verify** | Where does it break? | Go back to Step 2 / 3 / 4, fill the gap |
| 6 | **Complete** | Is it done? | Full Skill with extension presets |

---

## File Structure

```
skillforge/
├── README.md              ← You are here
├── SKILL.md               ← Entry point (bilingual, 7-step table + quality checklist)
├── PRINCIPLES.md          ← Full framework in Chinese
├── PRINCIPLES_en.md       ← Full framework in English
├── RECIPES.md            ← Five entry points in Chinese
├── RECIPES_en.md         ← Five entry points in English
├── LICENSE               ← MIT License
├── CONTRIBUTING.md       ← Contribution guide
└── .github/
    └── ISSUE_TEMPLATE/   ← Bug report + feature request templates
```

---

## Example Skills Built with This Framework

| Skill | Description |
|-------|-------------|
| [wechat-publisher](https://github.com/anthropics/claude-code/tree/main/.claude/skills/wechat-publisher) | Auto-generate WeChat articles with AI-generated images |

---

## License

MIT License — use freely, modify freely, contribute freely.

---

*SkillForge — giving you meta-cognition, not a rule library.*
