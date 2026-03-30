# Awesome 医疗 AI Skills 🏥🤖🇨🇳

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![最后更新](https://img.shields.io/badge/最后更新-2026--03--30-blue.svg)](#)
[![Skills 数量](https://img.shields.io/badge/Skills-80%2B-green.svg)](#)

> 🌍 **Looking for international skills?** See [awesome-medical-ai-skills](https://github.com/JuneYaooo/awesome-medical-ai-skills) — International Edition: Garmin, Fitbit, WHOOP, Epic FHIR, etc.

> 🏥 **找医疗 AI 项目（大模型、影像、临床系统）？** 请看 [awesome-medical-ai-cn](https://github.com/JuneYaooo/awesome-medical-ai-cn) — 国内医疗 AI 项目合集

> 精选**国内可用**的医疗 & 健康 AI Agent Skills、MCP 服务器合集。
> **仅收录可安装到 AI Agent 平台的技能**（Claude Code、OpenClaw、Cursor 等）。
> 重点关注：**网络可达性** · **中文支持** · **国内平台生态** · **国内法规合规**

---

## 为什么需要国内版？

国际版的许多 Skills 在国内使用时面临以下问题：

| 问题 | 说明 |
|------|------|
| 🚫 **网络不可达** | 部分 API 在国内无法直接访问（如 Google Scholar、某些 FHIR 端点） |
| 🈚 **中文支持差** | 很多 Skill 仅支持英文输入输出 |
| 📱 **平台不适用** | Fitbit/WHOOP/Oura 在国内用户少，华为/小米/OPPO 健康才是主流 |
| 📋 **法规不同** | 国内用 NMPA（国家药监局），不用 FDA |
| 🏥 **医疗体系不同** | 国内用 ICD-10 中文版、中医药标准、DRG/DIP 等 |

本仓库专注收录**国内用户真正能用的**医疗 AI 技能。

---

## 可用性标注

| 标记 | 含义 |
|------|------|
| ✅ **直接可用** | 国内网络直接可用，中文支持好 |
| ⚠️ **部分可用** | 可用但需要配置或有限制（如需 GitHub 访问） |
| 🔧 **需适配** | 需要自行修改或搭建才能在国内使用 |

---

## 目录

- [临床决策支持](#临床决策支持)
- [医疗 MCP 服务器](#医疗-mcp-服务器)
- [中医药 AI](#中医药-ai)
- [健康数据与可穿戴设备](#健康数据与可穿戴设备)
- [药物与药理](#药物与药理)
- [心理健康](#心理健康)
- [营养与饮食](#营养与饮食)
- [健身与训练](#健身与训练)
- [孕婴健康](#孕婴健康)
- [医疗器械合规](#医疗器械合规)
- [生物医学研究](#生物医学研究)
- [微信/企业微信集成](#微信企业微信集成)
- [技能合集与资源](#技能合集与资源)

---

## 临床决策支持

> 临床指南检索、患者报告生成、辅助诊断。

| 技能 | 平台 | 可用性 | Stars | 说明 |
|------|------|--------|-------|------|
| [medical-guidelines-suite](https://github.com/fshaan/medical-guidelines-suite) | Claude Code | ✅ 直接可用 | ![](https://img.shields.io/github/stars/fshaan/medical-guidelines-suite?style=flat-square) | 临床指南知识库构建 + 跨指南 RAG 检索 + 批量患者报告生成。**中文输出**。支持 NCCN、ESMO、CSCO 指南。生成 xlsx/docx/pptx 报告。 |
| [mediwise-health-suite](https://github.com/JuneYaooo/mediwise-health-suite) | OpenClaw | ✅ 直接可用 | ![](https://img.shields.io/github/stars/JuneYaooo/mediwise-health-suite?style=flat-square) | **家庭健康管理套件** — 健康档案、饮食追踪、体重管理、用药提醒、就医前摘要生成。支持多家庭成员隔离、图片识别化验单。本地 SQLite 存储，保护隐私。**中文原生**。 |
| [family-doctor](https://github.com/Yungho/family-doctor) | Claude Code / OpenClaw | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/Yungho/family-doctor?style=flat-square) | AI 家庭医生技能套件。25 个技能覆盖慢病管理、症状分诊、用药、睡眠、心理、家族史和预防保健；支持 Markdown+JSON 健康档案、自动关联分析与中文文档。 |
| [WellAlly-health](https://github.com/huifer/WellAlly-health) | Claude Code | ✅ 直接可用 | — | 个人健康档案管理。13 个专科咨询模拟、药物相互作用检测（A/B/C/D/X 五级）、辐射剂量追踪。**中英双语**。*(原名 Claude-Ally-Health)* |

**[→ 临床技能详情](categories/临床技能.md)**

---

## 医疗 MCP 服务器

> 可在国内使用或自部署的 MCP 服务器。

| 服务器 | 可用性 | Stars | 说明 |
|--------|--------|-------|------|
| [BioMCP](https://github.com/genomoncology/biomcp) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/genomoncology/biomcp?style=flat-square) | 15+ 生物医学 API（PubMed、ClinicalTrials.gov 等）。部分 API 国内可达，部分需代理。可自部署 HTTP 模式。 |
| [medical-mcp](https://github.com/JamesANZ/medical-mcp) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/JamesANZ/medical-mcp?style=flat-square) | FDA 药物、WHO 统计、PubMed 检索。Google Scholar 部分在国内不可用。本地部署无需 API 密钥。 |
| [OMOP MCP](https://github.com/OHNLP/omop_mcp) | ⚠️ 部分可用 | — | 临床术语到 OMOP 概念映射。需要 API Key。对接 LOINC、SNOMED 等国际标准。 |
| [mcp-simple-pubmed](https://github.com/andybrandt/mcp-simple-pubmed) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/andybrandt/mcp-simple-pubmed?style=flat-square) | PubMed 文献搜索。PubMed 在国内可直接访问。 |

---

## 中医药 AI

> 中医智能化相关项目和工具。

| 项目 | 可用性 | Stars | 说明 |
|------|--------|-------|------|
| *(暂无可用项目)* | | | 基于 Perplexity API 的中医健康视频制作等项目曾在 OpenClaw 上线，但目前链接已失效。 |

> 💡 **社区招募**：中医药 AI 是一个极具潜力但资源稀缺的方向。如果你有中医知识图谱、方剂数据库、辨证论治 Agent 等项目，欢迎提交 PR！

---

## 健康数据与可穿戴设备

### 国内主流设备

> 💡 **当前状态**：国内可穿戴设备（华为/小米/OPPO）的开放 API 较少，尚未发现专门的 Agent Skill。以下为已有的和国内可用的方案。

| 技能 | 平台 | 可用性 | 说明 |
|------|------|--------|------|
| [apple-health-skill](https://clawskills.sh/skills/nftechie-apple-health-skill) | OpenClaw | ✅ 直接可用 | Apple Health 数据查询（国内 iPhone 用户可用） |
| [apple-health-analyst](https://github.com/RuochenLyu/apple-health-analyst) | Claude Code / Multi | ✅ 直接可用 | ![](https://img.shields.io/github/stars/RuochenLyu/apple-health-analyst?style=flat-square) 本地解析 Apple Health 导出 ZIP，自动生成中英文健康报告，覆盖睡眠-恢复关联分析、行为模式识别与可解释评分。 |
| [healthkit-sync](https://clawskills.sh/skills/mneves75-healthkit-sync) | OpenClaw | ✅ 直接可用 | iOS HealthKit 数据同步 |
| [health-sync](https://clawskills.sh/skills/filipe-m-almeida-health-sync) | OpenClaw | ⚠️ 部分可用 | 多设备数据聚合（Oura/Withings/WHOOP 等，部分国内可用） |
| [health-summary](https://clawskills.sh/skills/yusaku-0426-health-summary) | OpenClaw | ✅ 直接可用 | 健康数据汇总报告生成 |

### Garmin（国内可用）

> Garmin 在国内有官方渠道，Connect 可用。

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [garmin-health](https://clawskills.sh/skills/eversonl-garmin-health-analysis) | ✅ 直接可用 | 自然语言查询 Garmin 数据 — 20+ 指标 |
| [garmin-cli](https://clawskills.sh/skills/voydz-garmin-cli) | ✅ 直接可用 | Garmin Connect CLI |

### 其他国际设备（国内部分可用）

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [fitbit](https://clawskills.sh/skills/mjrussell-fitbit) | ⚠️ 部分可用 | Fitbit 国内用户较少但可用 |
| [oura-analytics](https://clawskills.sh/skills/kesslerio-oura-analytics) | ⚠️ 部分可用 | Oura Ring 数据分析 |

---

## 药物与药理

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [maccabi-pharm-search](https://clawskills.sh/skills/alexpolonsky-maccabi-pharm-search) | 🔧 需适配 | 以色列药房库存查询（可参考开发国内版） |
| [admet-prediction](https://clawskills.sh/skills/huifer-admet-prediction) | ✅ 直接可用 | 药物 ADMET 预测（本地计算） |

> 💡 **缺口**：国内缺少 NMPA 药品数据查询、国家基本药物目录查询、医保目录查询等 Agent Skill。欢迎贡献！

---

## 心理健康

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [therapy-mode](https://clawskills.sh/skills/therapy-mode) | ⚠️ 部分可用 | CBT/ACT/DBT/MI 治疗框架。英文为主。*(链接可能失效)* |
| [anxiety-relief](https://clawskills.sh/skills/jhillin8-anxiety-relief) | ✅ 直接可用 | 焦虑缓解：接地练习和呼吸技巧 |
| [depression-support](https://clawskills.sh/skills/jhillin8-depression-support) | ✅ 直接可用 | 每日情绪追踪和抑郁支持 |
| [jungian-psychologist](https://clawskills.sh/skills/jungian-psychologist) | ⚠️ 部分可用 | 荣格心理学：阴影工作、原型分析、梦境解读。*(链接可能失效)* |
| [adhd-assistant](https://clawskills.sh/skills/thinktankmachine-adhd-assistant) | ✅ 直接可用 | ADHD 友好的生活管理助手 |
| [social-media-detox](https://clawskills.sh/skills/social-media-detox) | ✅ 直接可用 | 社交媒体戒瘾 + 数字健康。*(链接可能失效)* |

---

## 营养与饮食

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [calorie-counter](https://clawskills.sh/skills/cnqso-calorie-counter) | ✅ 直接可用 | 卡路里和蛋白质追踪 |
| [diet-tracker](https://clawskills.sh/skills/yonghaozhao722-diet-tracker) | ✅ 直接可用 | 每日饮食记录与营养计算 |
| [fasting-tracker](https://clawskills.sh/skills/jhillin8-fasting-tracker) | ✅ 直接可用 | 间歇性断食追踪 |
| [feast](https://clawskills.sh/skills/smadgerano-feast) | ⚠️ 部分可用 | 餐饮规划（含多文化主题） |
| [opencal](https://clawskills.sh/skills/neikfu-opencal) | ✅ 直接可用 | 通过 AI 语音记录饮食和管理卡路里 |

---

## 健身与训练

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [endurance-coach](https://clawskills.sh/skills/shiv19-endurance-coach) | ✅ 直接可用 | 个性化铁人三项/马拉松训练计划 |
| [muscle-gain](https://clawskills.sh/skills/jhillin8-muscle-gain) | ✅ 直接可用 | 肌肉增长追踪 |
| [hevy](https://clawskills.sh/skills/mjrussell-hevy) | ✅ 直接可用 | 健身数据查询（Hevy App） |
| [strava-cycling-coach](https://clawskills.sh/skills/strava-cycling-coach) | ⚠️ 部分可用 | Strava 骑行分析（国内 Strava 可用但用户较少）。*(链接可能失效)* |

---

## 孕婴健康

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [pregnancy-tracker](https://clawskills.sh/skills/pregnancy-tracker) | ✅ 直接可用 | 孕期追踪：每周更新、症状记录、里程碑倒计时。*(链接可能失效)* |
| [huckleberry](https://clawskills.sh/skills/jayhickey-huckleberry) | ⚠️ 部分可用 | 婴儿睡眠/喂养/成长追踪（需 Huckleberry App） |

---

## 医疗器械合规

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [capa-officer](https://clawskills.sh/skills/alirezarezvani-capa-officer) | ⚠️ 部分可用 | CAPA 系统管理（面向 FDA/ISO 体系，NMPA 需适配） |

> 💡 **缺口**：急需 NMPA 注册申报、国内 GMP 合规、医疗器械注册人制度相关的 Agent Skill。

---

## 生物医学研究

| 项目 | 可用性 | Stars | 说明 |
|------|--------|-------|------|
| [claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/K-Dense-AI/claude-scientific-skills?style=flat-square) | 170+ 科学技能文档（SKILL.md 格式），需通过 Claude Code / Cursor 等平台安装使用。生物信息学、化学信息学部分技能国内可用（本地计算为主）。 |
| [OpenBioMed Skills](https://github.com/PharMolix/OpenBioMed) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/PharMolix/OpenBioMed?style=flat-square) | PharMolix 与清华 AIR 联合发布的生物医药 Agent 平台，含 45 个可安装技能，覆盖药物发现、蛋白工程、单细胞组学。仓库自带 `skills/` 目录和工作流，但部分模型/依赖需自行准备环境。 |
| [M4](https://github.com/hannesill/m4) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/hannesill/m4?style=flat-square) | 面向 MIMIC-IV、eICU 等临床研究数据的 AI 基础设施。提供 MCP / Python 工具接口、测试和文档，适合本地或自托管科研分析。 |
| [med-stats-skills](https://github.com/chenhaodev/med-stats-skills) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/chenhaodev/med-stats-skills?style=flat-square) | 中国开发者维护的 OpenCode 医学统计与临床试验方法技能集。覆盖预测模型、验证、试验质量评估、临床数据管理，附模板、清单和 R/Python 示例。 |
| [MedgeClaw](https://github.com/xjtulyc/MedgeClaw) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/xjtulyc/MedgeClaw?style=flat-square) | 西安交大 — 生物医学 AI **研究编排助手**（非大模型本身）。通过对话调用 RNA-seq、药物发现、临床分析等 140+ K-Dense 科学技能。基于 Claude Code 构建。 |
| [ScienceClaw](https://github.com/AgentTeam-TaichuAI/ScienceClaw) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/AgentTeam-TaichuAI/ScienceClaw?style=flat-square) | 太初团队维护的科研智能体平台，内置 1900+ 科学工具与 Skills，覆盖 PubMed 检索、药物发现、生信分析和多格式内容生成。提供前后端、任务调度与沙箱，支持本地/自托管部署。 |
| [automedsci](https://github.com/Jay-Chen79/automedsci) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/Jay-Chen79/automedsci?style=flat-square) | 中文/英文双语的医学科研论文 AI 流水线。157 条实战规则 + 12 个技能工作流，覆盖选题、方案、分析、写作、交叉审稿和投稿检查；纯 Markdown、零依赖。 |
| [Bioclaw Skills Hub](https://github.com/zongtingwei/Bioclaw_Skills_Hub) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/zongtingwei/Bioclaw_Skills_Hub?style=flat-square) | 面向生物信息学与组学工作流的官方技能库。仓库包含 `skills/` 目录、分类目录和中英文文档，便于在 BioClaw 或通用 AI Agent 中复用。 |
| [AI_Bioinformatic](https://github.com/Jack123-Wang/AI_Bioinformatic) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/Jack123-Wang/AI_Bioinformatic?style=flat-square) | 面向 Claude 的生物信息学 Agent Skill 合集。已提供 GEO/TCGA/CGGA 多数据库检索和 scRNA-seq 细胞注释工作流，输出 Excel 报告与 R 可视化代码。 |
| [dna-claude-analysis](https://github.com/shmlkv/dna-claude-analysis) | ⚠️ 部分可用 | — | 个人基因组分析。支持 23andMe/AncestryDNA（国内可用微基因、23魔方等替代）。 |

---

## 微信/企业微信集成

以下技能支持通过微信或企业微信与 AI Agent 交互：

| 技能 | 平台 | 说明 |
|------|------|------|
| [wechat-mcp](https://clawskills.sh/skills/wechat-mcp) | OpenClaw | Windows 微信桌面端 MCP 集成 — 消息监控、搜索联系人、发送消息。*(链接可能失效)* |
| [wecom](https://clawskills.sh/skills/wecom) | OpenClaw | 通过 Webhook 向企业微信发送消息。*(链接可能失效)* |

---

## 技能合集与资源

| 资源 | Stars | 说明 |
|------|-------|------|
| [awesome-openclaw-skills-zh](https://github.com/clawdbot-ai/awesome-openclaw-skills-zh) | ![](https://img.shields.io/github/stars/clawdbot-ai/awesome-openclaw-skills-zh?style=flat-square) | OpenClaw **中文官方技能库**。按场景分类，支持中文调用。 |
| [OpenClaw-Medical-Skills](https://github.com/FreedomIntelligence/OpenClaw-Medical-Skills) | ![](https://img.shields.io/github/stars/FreedomIntelligence/OpenClaw-Medical-Skills?style=flat-square) | 869 个医疗技能（港中文深圳团队） |
| [Awesome-MCP-ZH](https://github.com/yzfly/Awesome-MCP-ZH) | ![](https://img.shields.io/github/stars/yzfly/Awesome-MCP-ZH?style=flat-square) | MCP 中文资源精选，含部分医疗相关 MCP 服务器索引。 |

---

## 姊妹仓库

| 仓库 | 说明 |
|------|------|
| [awesome-medical-ai-skills](https://github.com/JuneYaooo/awesome-medical-ai-skills) | 🌍 医疗 AI Skills（国际版） |
| [awesome-medical-ai](https://github.com/JuneYaooo/awesome-medical-ai) | 🌍 医疗 AI 项目合集（国际版） |
| [awesome-medical-ai-cn](https://github.com/JuneYaooo/awesome-medical-ai-cn) | 🇨🇳 国内医疗 AI 项目合集（大模型、影像、HIS 等） |

---

## ⚠️ 免责声明

> 本列表中的所有技能仅供**信息参考和研究目的**。它们**不是**经过验证的临床工具，**不应**用于实际的医疗诊断或治疗决策。请始终咨询合格的医疗专业人员获取医疗建议。AI 生成的医疗信息可能不准确甚至有害。

---

## 参与贡献

欢迎贡献！特别欢迎以下类型的提交：

### 💡 用过好用的医疗 Skill？推荐给大家！

如果你在实际工作中用过某个医疗 AI 技能，觉得**真的好用**，欢迎推荐！真实使用反馈是这个列表最有价值的信号。

**推荐方式：**
1. [提交 Issue](../../issues/new?title=推荐:+技能名称) 标题写 `推荐: <技能名称>`
2. 告诉我们：**你用它做了什么**、**哪些方面好用**、**有什么坑**
3. 我们会给该技能加上 `👍 社区推荐` 标记

> 经过真实用户验证的技能，比 Star 数更有参考价值。你的使用经验能帮助更多人做出更好的选择。

### 欢迎提交的内容

1. **国内可用的医疗 AI 技能**（标注可用性）
2. **中文医疗大模型**（已开源或可接入）
3. **国内健康平台集成**（华为/小米/微信健康等）
4. **国内法规合规工具**（NMPA/DRG/DIP 等）
5. **中医药 AI 项目**

### 提交格式

```markdown
| [项目名](链接) | 平台 | ✅/⚠️/🔧 | Stars | 一句话说明 |
```

---

## 许可证

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

本列表以 [CC0 1.0 通用](LICENSE) 发布。
