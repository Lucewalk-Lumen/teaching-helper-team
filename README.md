# teaching-helper-team

**教学帮帮团** · v1.1.2 · `team`

> Nine teaching experts and 18 skills covering course building, case writing, thesis mentoring, slides, minutes, voice synthesis and grant proposals, with de-AI and citation-fidelity gates.


Part of the [WorkBuddy Experts](https://github.com/Lucewalk/WorkBuddy-Experts) collection — expert teams, agents and skills for the WorkBuddy AI assistant platform.


## What it does

- **deai-rules** — "去AI味四层规则库：英文通用层（24 类英文 AI 高频模式）+ 中文通用层（AI 高频词表/四类高频病灶/标点硬约束）+ 文体专用层（案例 L1/L2 门禁、纪要 TEEL）+ 量化诊断层（统计信号/三级词汇/交付门槛）。用于所有交付文档的自然化改写门禁。"
- **citation-integrity** — 引用保真校验清单。规定一条引用怎么算核过、AI 编造引用有哪些特征、核不出来怎么标注处置、整篇论文的参考文献怎么批量走一遍。thesis-mentor 与 case-writer 交付前必读。
- **crawler** — >
- **material-extractor** — >
- **content-summary** — "总结 URL、本地文件、PDF、图片、音频与 YouTube 内容（多模型 CLI）。用于素材准备阶段的快速总结与要点提取，产出喂给纪要整理专家/案例写作专家/论文辅导专家。"
- **knowledge-wiki** — "用 LLM 构建并维护个人知识库（wiki）：将原始资料增量编译为持久、互链的 Markdown 知识库。适用于用户想创建知识库、搭建个人 wiki、整理研究笔记、导入文档或维护长期演化的知识库。"
- **long-manuscript-core** — 将大纲、访谈、笔记、部分草稿与成稿推进为长文档。用于产出首个可用价值的稿件片段、对限定范围章节做续写或修订，或将草稿收尾交付。覆盖资料激活、限定范围续写/修订、成稿收尾三大场景。
- **architect** — 通用 Agent / Skill 生产级制作、校验与交付工作流（平台无关，已对齐 WorkBuddy）。交互式收集需求，设计职责边界、上下文、结构化动作、人类介入与错误恢复；按生产级规范生成并校验技能（SKILL.md）/ agent，复用本宿主原生能力（find-skills 
- **case-writer** — "高校教学案例、课程思政案例与工商管理案例写作（四路径：教学案例/课程思政/融入思政/工商管理案例）。案例写作专家陈叙真的主技能包，含八要素深度标准、思政元素映射、引用保真四铁律、deai-rules 去AI味门禁与 md_to_docx 转换。"
- **thesis-mentor** — |
- **course-builder** — >
- **edu-grant-writer** — |
- **literature-distiller** — 论文文献速览与蒸馏助手。支持用户上传的 PDF 文件，通过 4+2 深度蒸馏模型快速提取元数据、逻辑骨架、核心发现及批判性洞察，生成结构化 Markdown 报告，并可沉淀到本地知识库（knowledge-wiki）。适用于个人文献管理、快速浏览、知识收集等场景。
- **textbook-chapter-expansion** — "教材/书籍/长文档薄弱章节的批量补齐：三路并行差距扫描 → 多 Agent 并行扩充 → 锚点注入正文 → 素材分层回填 → 一致性验证 → docx 导出。适用于教材编写、书稿修订、长文档加厚等大规模内容补齐任务。触发词：教材补齐、章节扩充、加厚章节、章节太薄、素材回填、批量
- **ppt-maker** — >
- **minutes-organizer** — 学术会议纪要与综述报告智能生成。扫描本地会议文件夹（转录稿/PPT照片/议程PDF），完成 OCR 与内容归类，产出两类文档：1.按主题-汇报人复述的会议纪要；2.按议题重组、三层评述的学术综述报告。遵循 deai-rules 去AI味门禁与 TEEL 段落逻辑，先出 .md 供
- **text-to-speech** — "免费语音合成：微软 Edge TTS（40+ 语言 300+ 声音），支持 rate/pitch/volume 精细控制，输出 MP3+SRT 字幕。零成本做课程/汇报/答辩音频。"
- **setup** — "教学帮帮团一键初始化技能：装包后/首次会话/用户说『初始化/装依赖/配置环境/开箱即用』时触发，统一安装全部运行时依赖（Python 托管 venv + Node docx）、检测 crawler 的 bsk CLI、为 content-summary 生成 `.env` 凭证

## Agent roster

| Agent | Role |
|---|---|
| `architect` | 智能体架构专家 - 安志远 |
| `case-writer` | 案例写作专家 - 陈叙真 |
| `course-builder` | 课程建设专家 - 柯明纲 |
| `grant-writer` | 教育课题申报专家 - 项承文 |
| `minutes-organizer` | 纪要整理专家 - 闻纪清 |
| `ppt-maker` | 课件制作专家 - 裴演 |
| `teaching-helper-team-lead` | 教学编排总监 - 齐帮办 |
| `text-to-speech` | 语音合成专家 - 声入微 |
| `thesis-mentor` | 论文辅导专家 - 周慎导 |

## Install

1. Download the package zip from [Releases](https://github.com/Lucewalk/teaching-helper-team/releases) or clone this repo;
2. Unzip keeping the internal manifest structure intact;
3. Import/register in WorkBuddy (custom connector → trust & enable).

## Version

Current release: **v1.1.2** — see [CHANGELOG.md](CHANGELOG.md) if present, or the package manifest.

## License

MIT — see [LICENSE](LICENSE).
