# Writing Style Guide · System Skill Pack

> **Naitangsu (奶糖酥)** · A craft notebook built from hundreds of thousands of words written
>
> From "how to make a single sentence clean" to "how to make a whole book complete" —
> covering sentences, paragraphs, dialogue, scenes, plot, characters, space, sweet-pain balance,
> high-density scenes, narrative systems, themes, endings, and more across 43 volumes + an appendix.
> Take it and write your own story — the joy and the ache in it are real.

---

## 📖 About Naitangsu (奶糖酥)

**Naitangsu** is a contracted author on Fanqie Novel (番茄小说), with multiple completed modern romance works.

| Work | Genre | Length | Status |
|------|-------|--------|--------|
| **Su Yu Xin Jian (溯雨信笺)** | Youth romance / mutual rescue / small-town literature | 373K words · 170 ch | ✅ Completed 2026-03-13 · Signed for print publication · 番外11章 (drama alias《酸涩湿吻》) · EN translation "Letters from the Rainy Past" serialized on Shanghai Fantasy |
| **Chao Xi Jie Xian (潮汐界限)** | High-ranking officials / age-gap / government setting | 347K words · 165 ch (incl. 16 extras) | ✅ Completed · 实体书已上市 (时代文艺出版社, ISBN 9787538779707) · 短剧《雾潮燃欲》化用本作角色 |
| **Tian Wu Chan Mian (甜雾缠绵)** | Modern romance / suspense crime | — | ✅ Completed · 实体书《甜雾》上市 (云南人民出版社, ISBN 9787222212763) |
| **Dai Shu You Li (待熟诱荔)** | Modern romance / diplomatic / mentor-student | — | ✅ Completed |
| **Wen Yang (吻漾)** | CEO romance / marriage first, love later / CV圈 | 259K words | ✅ Completed · 长标题《引欲！带感！…》 |
| **Er Shi Yi Feng Xin (二十一封信)** | Modern romance | — | 📝 Ongoing · 较新书 |

**Social media:**
- 📱 **Weibo**: **@奶糖酥崽** — shares extra chapters, new book updates, writing daily (「奶糖酥崽」超话)
- 🎬 **Douyin**: **@奶糖酥崽** (抖音号 uilOoOoOIP, IP 浙江) — self-intro, character & title解读, 片段. Latest video 2026-07-21 (溯雨信笺 theme, 325K likes)
- No verified account found on Xiaohongshu

> 作者番茄主页 bio 亲口标注「围脖🧣抖✨：@奶糖酥崽」，微博与抖音为同一账号名。

---

## File Structure

```
naitangsu-write-skill/
├── README.md                          ← This file
├── docs/
│   └── distillation-notice.md        ← Distillation notice (repo meta, not skill content)
├── demos/
│   └── project-wenwan/               ← Usage demo project (温晚)
└── skill/                            ← ★ the distributable skill folder
    ├── SKILL.md                      ← Overview + persona + nav table + usage protocol (~115 lines)
    ├── quick-start.md                ← 3-minute onboarding (scene navigation + reading order)
    ├── references/                   ← Progressive disclosure: loaded on demand
        ├── author-profile.md         ← Author metadata (persona anchors live here)
        ├── before-after.md            ← Before/after examples + revision demo
        ├── dna-analysis.md            ← DNA analysis methodology
        ├── dna-atlas.md               ← 11-dimension DNA atlas (A.1-A.11) + 句式频次签名
        ├── sentences-paragraphs.md    ← 卷一/二/三  Sentences · paragraphs · patterns
        ├── dialogue.md                ← 卷四       Dialogue & subtext
        ├── psychology-emotion.md      ← 卷五       Psychology & emotion
        ├── narrative-basics.md        ← 卷六~十五  Narrative · punctuation · function words · SOP
        ├── pov-hooks-blanks.md        ← 卷十六~十九 POV · hooks · emotion · blanks
        ├── scenes-revision.md         ← 卷二十/二十一 Special scenes · revision restraint
        ├── ai-tell.md                 ← 卷二十二   AI-tell diagnosis (7 symptoms + SOP)
        ├── plot-architecture.md       ← 卷二十三/二十四 Plot architecture · story engine
        ├── characters-space.md        ← 卷二十五/二十六 Characters · spatial texture
        ├── sweet-pain-theme-ending.md ← 卷二十七~二十九 Sweet-pain · theme · ending
        ├── conflict-reunion-tension.md← 卷三十~三十二 Conflict · reunion · tension
        ├── narrative-system.md       ← 卷三十三~三十五 Info gap · network · bridging
        ├── confession-arcs.md         ← 卷三十六~三十九 Confession · arcs · extras
        ├── universal-model.md         ← 卷四十      Cross-work universal model
        ├── checklist.md               ← 卷四十一    Final draft checklist
        ├── genre-specific.md          ← 卷四十二    Genre-specific (体制/刑侦/替身)
        └── character-autonomy.md      ← 卷四十三    Character autonomy (角色反抗大纲)
    ├── story-memory.md                ← Story memory system (character / plot / timeline)
    ├── novel-draft.md                 ← Workflow: chapter drafting
    ├── novel-revise.md                ← Workflow: chapter revision
    └── novel-review.md                ← Workflow: final review
```

> `docs/` and `demos/` stay at repo root (repo meta / usage demo, not skill runtime content). The skill folder is `skill/` — everything Claude loads at runtime lives under it.

---

## Installation

### Method 1: Clone or download this repo

```bash
git clone <this-repo-url> naitangsu-write-skill
```

Then copy the **entire `skill/` directory** (including `references/`) into your Claude skills folder:

- **Global**: `~/.claude/skills/naitangsu-write-skill/` (so that `references/` sits next to `SKILL.md`)
- **Project-level**: `<project-dir>/.claude/skills/naitangsu-write-skill/`

The `references/` folder must travel with `SKILL.md` — progressive disclosure relies on relative paths. Copying only `SKILL.md` will break every reference link.

> If you have an older install under `~/.claude/skills/writing-style-guide/` (previous name), remove it after reinstalling to avoid a stale duplicate.

Once installed, mention "writing style", "clean writing", or related keywords in any Claude conversation to auto-load this skill.

### Method 2: Manual copy

Download or clone this repo, then copy the **whole `skill/` directory** (not just `SKILL.md`) to one of the locations above.

---

## Trigger Keywords

The following keywords trigger this skill:

writing, writing style, how to write a novel, web novel technique, clean writing, revision, rewrite, how to write romance, novel outline, plot design, white sketch, leaving blanks, dialogue writing, psychological description, DNA analysis

English prompts that will work:
- "Help me revise this paragraph to be cleaner"
- "How do I write this confession scene?"
- "My dialogue feels flat, what do I change?"
- "Analyze the rhythm of this chapter"
- "This character feels like a cardboard cutout"

---

## Contents Overview

| Section | Content | Core Value |
|---------|---------|------------|
| Vol 1–3 | Sentence cleanliness · Paragraph rhythm · Sentence patterns | Remove filler words, remove explanations, remove fluff |
| Vol 4 | Dialogue techniques & subtext | Dialogue = conflict, answer with action, not words |
| Vol 5 | Psychology & emotion (body language dictionary) | Fewer emotion words, more emotion evidence |
| Vol 6 | Narrative techniques (hooks/umbrella-sharing/diary closure) | 36 narrative modules, plug-and-play |
| Vol 7–15 | Punctuation · Function words · Characters · Scenes · Revision SOP | Foundational skills + layered revision |
| Vol 16 | POV iron law (limited third person) | Information management + legal POV channels |
| Vol 17–19 | Hook design · Emotional progression · Leaving blanks | 6 chapter-end hook formulas + 4 levels of blank-leaving |
| Vol 20–22 | AI-tell diagnosis · Over-revision | Recognize and avoid 7 AI-tell symptoms |
| **Vol 23–24** | **Plot architecture core** | 3 story engines / 5-stage skeleton / 3-tier conflict |
| Vol 25 | Character building (3 anchors / unworthiness engine) | Depth, not labels |
| Vol 26 | Spatial texture & everyday details | Signature places / object inventory method |
| Vol 27 | Sweet-pain rhythm & emotional ratio | 4 purities / 4 textures / intra-chapter tug-of-war |
| Vol 28–29 | Theme & ending art | Bury-grow-reveal 3-stage + ending design |
| Vol 30–32 | Conflict / reunion / romantic tension | Full toolbox for 3 special scene types |
| **Vol 33–35** | **System-level narrative** | Information gap / relationship network / chapter bridging |
| **Vol 36** | **Confession variants** | 6 confession modes (stamping/silent echo/reverse stamping/non-answer/older-couple/self-monologue) |
| **Vol 37** | **Female lead courage arc** | 4-stage courage escalation + body language externalization + solitude moment writing |
| **Vol 38** | **Male lead restraint-breaking system** | Youth vs mature vs wild type differences + 8 trigger types |
| **Vol 39** | **Extra chapter design system** | 6 functions + iron rules + POV reversal formula + IF-line design |
| **Vol 40** | **Cross-work universal model** | Dual-dilemma opening / seasonal cycle / imagery system / closing chapter traits |
| **Vol 41** | **Final draft checklist** | Sentence/paragraph/dialogue/POV/chapter/closure → 80%+ ready |
| **Vol 42** | **Genre-specific supplements** | 42.1 体制文 / 42.2 刑侦+言情 / 42.3 替身文学 |
| **Vol 43** | **Character autonomy** | When characters resist the outline — 4 rebellion types + decision framework |
| **Appendix** | **Quantitative DNA atlas** | Scientific distillation from a 1M+ word corpus — body language / verbs / temperature / senses / imagery / color / syntax / dialogue / time anchors / syntax-frequency signatures, 11-dimension quantified map |
| **Workflows** | **Draft / Revise / Review** | 3 workflow skills embedding 43-volume techniques into writing pipeline |
| **Memory** | **Story memory system** | Character tracking / plot threads / timeline / consistency checks |

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
| **AI-tell check** | Scan text for repetitive metaphors / sawtooth rhythm / evenly-spaced verbs |

---

## Design Philosophy

```
Clean language, powerful emotion.
Take it and write your own story — the joy and the ache in it are real.
```

All examples in this guide are generic (using neutral referents).
They do not reference, imply, or represent any specific author, work, or character.

---

## License

MIT License — see [LICENSE](LICENSE) file for details.

## 免责声明

本技能是**对写作模式的观察总结**，来源于番茄签约作家奶糖酥公开作品的定量分析。本仓库**不包含、不复制、不重新分发**任何受版权保护的原文内容。

- 所有技法示例使用**中性指称**和**通用场景**
- 蒸馏的是**结构规律**（句子节奏、对话机制、叙事架构），而非创作内容
- 原理等同于风格指南或写作教科书——教的是"怎么写"，不是"写了什么"
- 原作者对其原创作品保留完整著作权

如您是奶糖酥本人或权利人，认为本仓库侵犯了您的权益，请提交 Issue 或联系仓库维护者。

---

*Naitangsu · 2026-07-01*
