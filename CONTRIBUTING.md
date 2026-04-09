# Contributing to Skill Factory

Thank you for your interest in contributing.

## How to Contribute

### Report Issues

Use GitHub Issues to report:
- Bugs in the seven-step derivation logic
- Gaps in the Five Elements reasoning framework
- Unclear definitions or ambiguous language
- Missing entry points for common Skill types

Please include:
- Which file and section the issue is in
- What you expected vs. what you found
- A concrete example when possible

### Propose Changes

#### Minor Changes (typos, clarity improvements)
- Submit a PR directly with the fix
- Description: what changed and why

#### Meaningful Changes (new steps, new frameworks, structural rewrites)
- Open an Issue first to discuss the change
- Wait for consensus before submitting a PR
- PR should include the Chinese version and English version

### Style Guide

**Language**: Write in clear, unambiguous English (or Chinese for Chinese-language files)

**Avoid**:
- Colloquial question forms ("Is it good enough?", "Are tools sufficient?")
- Anthropomorphization of forces ("Does Fire want to produce?")
- Vague quantifiers ("appropriate", "sufficient", "reasonable") without definition

**Use**:
- Formal, declarative statements ("Judgment threshold: 10%")
- Force labels with parentheses: Fire (Judgment), Metal (Structure)
- Specific thresholds and conditions

### File Structure

```
PRINCIPLES_en.md    ← English version of core principles
PRINCIPLES.md       ← Chinese version (同步更新)
RECIPES_en.md       ← English version of entry points
RECIPES.md          ← Chinese version (同步更新)
SKILL.md            ← Bilingual entry, do not separate
```

When modifying core principles, always update both language versions in the same PR.
