# Naitangsu Writing Style Guide

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Skill](https://img.shields.io/badge/Claude-Skill-purple)](https://claude.ai/code)

> A distilled writing craft guide from 43 volumes of web novel techniques —  
> from "how to make a single sentence clean" to "how to make a whole book complete."  
> **Clean language, powerful emotion.**

---

## Features

- **43 volumes** covering sentences, paragraphs, dialogue, scenes, plot, characters, spatial texture, sweet-pain rhythm, theme, endings, and more
- **3 built-in workflows** — draft, revise, and review — embedding the full technique library into your writing pipeline
- **Story memory system** — track characters, plot threads, and timeline across chapters
- **AI-tell diagnosis** — 7-symptom detection system with quick-fix SOPs
- **Quantitative DNA atlas** — 11-dimension style analysis from a 1M+ word corpus
- **Progressive disclosure** — load only the technique file you need, when you need it

---

## Quick Start

### 1. Clone the repository

```bash
git clone https://github.com/haoming-yang/naitangsu-write-skill.git
cd naitangsu-write-skill/skill
```

### 2. Install the skill

This repository contains Markdown instructions and reference files only. No Python packages are required, so there is no `requirements.txt` to install.

#### Claude Code (macOS / Linux)

```bash
mkdir -p ~/.claude/skills/naitangsu-write-skill
cp -R ./. ~/.claude/skills/naitangsu-write-skill/
```

#### Claude Code (Windows PowerShell)

```powershell
$dest = Join-Path $HOME ".claude\skills\naitangsu-write-skill"
New-Item -ItemType Directory -Force -Path $dest | Out-Null
Copy-Item -Path ".\*" -Destination $dest -Recurse -Force
```

#### Codex

```bash
mkdir -p ~/.agents/skills/naitangsu-write-skill
cp -R ./. ~/.agents/skills/naitangsu-write-skill/
```

### 3. Verify the installation

The installed directory must contain `SKILL.md` directly:

```text
~/.claude/skills/naitangsu-write-skill/SKILL.md
```

If `SKILL.md` is located at `.../naitangsu-write-skill/skill/SKILL.md`, you copied the repository root instead of the contents of the `skill/` directory.

### 4. Start using the skill

Once installed, the skill can be selected automatically for matching modern-romance writing tasks. You can also explicitly mention the skill or its methods. Try:

> "Help me revise this paragraph to be cleaner"  
> "How do I write this confession scene?"  
> "My dialogue feels flat, what do I change?"  
> "Check this chapter for AI-tell symptoms"

Or use the workflow commands:

| Trigger | Workflow |
|---------|----------|
| "Write a new chapter" | Drafting workflow |
| "Revise this passage" | Revision + diagnosis |
| "Review my draft" | Full dimensional review |

---

## Contents

| Section | Content | Core Value |
|---------|---------|------------|
| Vol 1–5 | Sentences · Paragraphs · Dialogue · Psychology · Senses | Foundation: clean language |
| Vol 6–15 | Narrative techniques · Punctuation · Function words · Characters · Scenes · Revision SOP | Craft precision |
| Vol 16–22 | POV iron law · Hook design · Emotional progression · Blanks · AI-tell diagnosis | Reader engagement |
| Vol 23–26 | Plot architecture · Story engines · Character building · Spatial texture | Structure & depth |
| Vol 27–29 | Sweet-pain rhythm · Theme · Ending art | Emotional impact |
| Vol 30–35 | Conflict · Reunion · Romantic tension · Info gap · Network · Bridging | Relationship dynamics |
| Vol 36–40 | Confession variants · Courage arcs · Restraint-breaking · Extra chapters · Universal model | Romance mastery |
| Vol 41–43 | Final checklist · Genre supplements · Character autonomy | Polish & edge cases |
| **Appendix** | **DNA atlas** | 11-dimension style quantification |

> ✨ See [`skill/quick-start.md`](skill/quick-start.md) for scene-by-scene navigation and suggested reading order.

---

## Usage Scenarios

| Scenario | How |
|----------|-----|
| **Revision** | Paste a passage; the skill analyzes sentence cleanliness, dialogue subtext, paragraph rhythm |
| **Writing romance** | Call on romantic tension escalation / confession ladder / sweet-pain ratio modules |
| **Plot design** | 3 story engine selection + 3-tier conflict + dual-thread interlocking |
| **Character building** | 3 anchors setup + unworthiness engine + arc verification |
| **Outline structure** | 5-act division + chapter bridging + suspense nesting |
| **Final chapter** | Style elevation + opening-closing image return + blank-leaving boundary |
| **AI-tell check** | Scan text for 7 AI-tell symptoms with structured SOP |

---

## About the Source Author

**Naitangsu (奶糖酥)** is a contracted author on Fanqie Novel (番茄小说) with multiple completed modern romance works spanning youth romance, high-official romance, suspense romance, and diplomatic romance — all exceeding one million Chinese characters in total.

| Work | Genre | Length | Status |
|------|-------|--------|--------|
| **Su Yu Xin Jian (溯雨信笺)** | Youth romance / mutual rescue / small-town literature | 373K words · 170 ch | ✅ Completed · Signed for print · EN translation ongoing |
| **Chao Xi Jie Xian (潮汐界限)** | High-ranking officials / age-gap / government setting | 347K words · 165 ch | ✅ Completed · Print edition published · Short drama adapted |
| **Tian Wu Chan Mian (甜雾缠绵)** | Modern romance / suspense crime | — | ✅ Completed · Print edition available |
| **Dai Shu You Li (待熟诱荔)** | Modern romance / diplomatic / mentor-student | — | ✅ Completed |
| **Wen Yang (吻漾)** | CEO romance / marriage first, love later | 259K words | ✅ Completed |
| **Er Shi Yi Feng Xin (二十一封信)** | Modern romance | — | 📝 Ongoing |

**Social media**: [@奶糖酥崽](https://weibo.com) on Weibo · [@奶糖酥崽](https://www.douyin.com/user/MS4wLjABAAAApzooXyXHcUKgI7zAsusGFVbe-uQ0gDSsR-sU6WvG-9IueWGUc_Hcyb3pNlfH6VY) on Douyin

> This skill is distilled from the author's publicly completed works through quantitative pattern analysis. All technique examples use neutral referents and generic scenarios.

---

## File Structure

```
naitangsu-write-skill/
├── README.md
├── LICENSE
├── docs/
│   └── distillation-notice.md
├── demos/
│   └── project-wenwan/              ← Usage demo
└── skill/                            ← distributable skill
    ├── SKILL.md                      ← Entry point + persona + nav
    ├── quick-start.md                ← 3-minute onboarding
    ├── story-memory.md               ← Character/plot/timeline tracking
    ├── novel-draft.md                ← Drafting workflow
    ├── novel-revise.md               ← Revision workflow
    ├── novel-review.md               ← Final review workflow
    └── references/                   ← 21 technique files
        ├── author-profile.md
        ├── before-after.md
        ├── dna-analysis.md / dna-atlas.md
        ├── sentences-paragraphs.md   ← Vol 1-3
        ├── dialogue.md               ← Vol 4
        ├── ... and 15 more
```

> The `skill/` folder is the only directory needed at runtime. Copy it in full — `references/` must sit next to `SKILL.md` for progressive disclosure to work.

---

## Design Philosophy

```
Clean language, powerful emotion.
Take it and write your own story — the joy and the ache in it are real.
```

---

## License

MIT License — see [LICENSE](LICENSE) for details.

## 免责声明

本技能是**对写作模式的观察总结**，来源于番茄签约作家奶糖酥公开作品的定量分析。本仓库**不包含、不复制、不重新分发**任何受版权保护的原文内容。

- 所有技法示例使用**中性指称**和**通用场景**
- 蒸馏的是**结构规律**（句子节奏、对话机制、叙事架构），而非创作内容
- 原理等同于风格指南或写作教科书——教的是"怎么写"，不是"写了什么"
- 原作者对其原创作品保留完整著作权

如您是奶糖酥本人或权利人，认为本仓库侵犯了您的权益，请提交 Issue 或联系仓库维护者。

---

*haoming-yang · 2026-08-05*
