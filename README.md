# teaching-helper-team

**教学帮帮团** · v1.1.2 · `team`

> Nine teaching experts and 18 skills covering course building, case writing, thesis mentoring, slides, minutes, voice synthesis and grant proposals — with de-AI-flavor and citation-fidelity gates on every deliverable.

Part of the [Lucewalk Lumen](https://github.com/Lucewalk-Lumen/about-me) collection — expert teams, agents and skills for the WorkBuddy AI assistant platform.

## What it does

A full teaching-production bench for higher-education teachers, organized as a **three-layer architecture** rather than a bag of prompts:

- **Agent layer (8 domain experts + orchestrator)** — course building, case writing, thesis mentoring, grant writing, slide making, minutes organizing, text-to-speech, plus the lead (教学编排总监 · 齐帮办) who routes and assembles.
- **Foundation layer (5 skills, mounted on the lead, injected on demand)** — shared capabilities like material extraction, content summarization and the knowledge wiki that every workflow can draw on.
- **Quality-gate layer (2 skills, applied to all text output)** — `citation-integrity` and `deai-rules`: references must be real, and prose must not read like machine-generated filler. These gates run on the final deliverable, not on intermediate steps.

On top of that sits a **material-tool boundary table** (which extractor/crawler/summarizer owns which input type) to prevent ambiguous double-triggering.

## Preloaded workflows

Six scenario workflows ship ready-to-run — you describe the situation, the lead picks the workflow:

- **Workflow A — material prep / collection**: crawler + extractor → downstream teams
- **Workflow B — minutes & review synthesis** (minutes-organizer)
- **Workflow C — university case writing** (case-writer)
- **Workflow D — thesis mentoring** (thesis-mentor)
- **Workflow E — agent skill production** (architect — build a new expert/skill package)
- **Workflow F — knowledge-base consolidation** (knowledge-wiki)

## Hard gates (by design)

- **Init / Step 0** — a mandatory initialization pass on the first message of every session (version broadcast + capability alignment);
- **Input routing gate** — every submitted input passes a routing check before any member is engaged;
- **Web-crawler confirmation gate** — crawling only runs after you explicitly confirm the targets.

## Agent roster

| Agent | Role |
|---|---|
| `teaching-helper-team-lead` | Orchestrator — teaching orchestration director |
| `architect` | Builds new agent/skill packages (also powers Workflow E) |
| `case-writer` | University teaching-case writing |
| `course-builder` | Course architecture & materials |
| `grant-writer` | Education grant proposals (edu-grant-writer skill) |
| `minutes-organizer` | Meeting minutes & review synthesis |
| `ppt-maker` | Slide decks for teaching |
| `text-to-speech` | Voice synthesis for course audio |
| `thesis-mentor` | Thesis supervision support |

## Skills (18)

`architect` · `case-writer` · `citation-integrity`(quality gate) · `content-summary` · `course-builder` · `crawler` · `deai-rules`(quality gate) · `edu-grant-writer` · `knowledge-wiki` · `literature-distiller` · `long-manuscript-core` · `material-extractor` · `minutes-organizer` · `ppt-maker` · `setup`(init) · `text-to-speech` · `textbook-chapter-expansion` · `thesis-mentor` · `_shared`

## Install

1. Download the package zip from [Releases](https://github.com/Lucewalk-Lumen/teaching-helper-team/releases) or clone this repo;
2. Unzip keeping the `.codebuddy-plugin/` manifest structure intact;
3. Import/register in WorkBuddy (custom connector → trust & enable). Step 0 initialization runs automatically on first use.

## Version

Current release: **v1.1.2**. See the package manifest and in-package `CHANGELOG.md` for details.

## License

MIT — see [LICENSE](LICENSE).


---

<details>
<summary><strong>📖 中文说明(Chinese README)</strong></summary>

# 教学帮帮团

**教学帮帮团:九专家十八技能,三层架构,六大预设工作流**

- 版本:v1.1.2 · 类型:team
- 版本真源:包内 `.codebuddy-plugin/plugin.json` 的 `version` 字段
- 所属合集:[Lucewalk Experts 门户](https://github.com/Lucewalk-Lumen/about-me)(全部产品目录与品牌说明)

## 安装

1. 从本仓库 [Releases](https://github.com/Lucewalk-Lumen/teaching-helper-team/releases) 页下载该包 zip(或直接克隆仓库);
2. 解压后**保持内部清单结构不变**(`.codebuddy-plugin/` 目录);
3. 在 WorkBuddy 中导入/注册(自定义连接器入口 → 信任并启用)。

能力详解见上方英文文档;品牌与全部产品目录见门户仓库。

## 许可

MIT——详见 [LICENSE](LICENSE)。

</details>
