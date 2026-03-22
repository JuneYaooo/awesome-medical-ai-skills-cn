# Awesome 医疗 AI Skills 🏥🤖🇨🇳

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![最后更新](https://img.shields.io/badge/最后更新-2026--03--22-blue.svg)](#)
[![Skills 数量](https://img.shields.io/badge/Skills-80%2B-green.svg)](#)

> 🌍 **Looking for international skills?** See [awesome-medical-ai-skills](https://github.com/yyj/awesome-medical-ai-skills) — International Edition: Garmin, Fitbit, WHOOP, Epic FHIR, etc.

> 精选**国内可用**的医疗 & 健康 AI Agent Skills、MCP 服务器和工具合集。
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
- [中文医疗大模型](#中文医疗大模型)
- [医疗 MCP 服务器](#医疗-mcp-服务器)
- [中医药 AI](#中医药-ai)
- [医学影像 AI](#医学影像-ai)
- [电子病历与临床系统](#电子病历与临床系统)
- [健康数据与可穿戴设备](#健康数据与可穿戴设备)
- [药物与药理](#药物与药理)
- [心理健康](#心理健康)
- [营养与饮食](#营养与饮食)
- [健身与训练](#健身与训练)
- [孕婴健康](#孕婴健康)
- [医疗器械合规](#医疗器械合规)
- [生物医学研究](#生物医学研究)
- [多智能体医疗系统](#多智能体医疗系统)
- [技能合集与资源](#技能合集与资源)

---

## 临床决策支持

> 临床指南检索、患者报告生成、辅助诊断。

| 技能 | 平台 | 可用性 | Stars | 说明 |
|------|------|--------|-------|------|
| [medical-guidelines-suite](https://github.com/fshaan/medical-guidelines-suite) | Claude Code | ✅ 直接可用 | ![](https://img.shields.io/github/stars/fshaan/medical-guidelines-suite?style=flat-square) | 临床指南知识库构建 + 跨指南 RAG 检索 + 批量患者报告生成。**中文输出**。支持 NCCN、ESMO、CSCO 指南。生成 xlsx/docx/pptx 报告。 |
| [Claude-Ally-Health](https://github.com/huifer/Claude-Ally-Health) | Claude Code | ✅ 直接可用 | — | 个人健康档案管理。13 个专科咨询模拟、药物相互作用检测（A/B/C/D/X 五级）、辐射剂量追踪。**中英双语**。 |
| [cyber-doctor（赛博华佗）](https://github.com/Warma10032/cyber-doctor) | 独立项目 | ✅ 直接可用 | ![](https://img.shields.io/github/stars/Warma10032/cyber-doctor?style=flat-square) | 基于多模态大模型的多功能智能体。接入医疗知识图谱后可进行疾病初诊、病历分析、专业知识问答。一键搭建本地多模态大模型。 |

**[→ 临床技能详情](categories/临床技能.md)**

---

## 中文医疗大模型

> 国内团队开发的医疗领域大模型，可作为 Agent 的底座或工具。

| 项目 | Stars | 团队 | 说明 |
|------|-------|------|------|
| [HuatuoGPT](https://github.com/FreedomIntelligence/HuatuoGPT) | ![](https://img.shields.io/github/stars/FreedomIntelligence/HuatuoGPT?style=flat-square) | 港中文深圳 | 华佗 GPT — 面向医疗场景的开源中文医疗大模型。支持问诊对话、医学知识问答。 |
| [HuatuoGPT-o1](https://github.com/FreedomIntelligence/HuatuoGPT-o1) | ![](https://img.shields.io/github/stars/FreedomIntelligence/HuatuoGPT-o1?style=flat-square) | 港中文深圳 | 医疗领域复杂推理能力，Medical o1 思路。 |
| [DISC-MedLLM](https://github.com/FudanDISC/DISC-MedLLM) | ![](https://img.shields.io/github/stars/FudanDISC/DISC-MedLLM?style=flat-square) | 复旦 DISC | 面向医疗健康对话的大语言模型。智能问诊、医疗知识问答、病历结构化。 |
| [MedgeClaw](https://github.com/xjtulyc/MedgeClaw) | ![](https://img.shields.io/github/stars/xjtulyc/MedgeClaw?style=flat-square) | 西安交大 | 生物医学 AI 研究助手 — 通过对话运行 RNA-seq、药物发现、临床分析等。基于 Claude Code 构建，140+ K-Dense 科学技能。 |
| [OpenClaw-Medical-Skills](https://github.com/FreedomIntelligence/OpenClaw-Medical-Skills) | ![](https://img.shields.io/github/stars/FreedomIntelligence/OpenClaw-Medical-Skills?style=flat-square) | 港中文深圳 | 869 个医疗 AI Agent 技能：临床工作流、基因组学、药物发现、法规合规。OpenClaw 平台。 |
| [Chinese-clinical-NER](https://github.com/MenglinLu/Chinese-clinical-NER) | ![](https://img.shields.io/github/stars/MenglinLu/Chinese-clinical-NER?style=flat-square) | — | CCKS2019 中文命名实体识别：从医疗文本中识别疾病、解剖部位、影像检查、实验室检验、手术和药物 6 种实体。 |

---

## 医疗 MCP 服务器

> 可在国内使用或自部署的 MCP 服务器。

| 服务器 | 可用性 | Stars | 说明 |
|--------|--------|-------|------|
| [BioMCP](https://github.com/genomoncology/biomcp) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/genomoncology/biomcp?style=flat-square) | 15+ 生物医学 API（PubMed、ClinicalTrials.gov 等）。部分 API 国内可达，部分需代理。可自部署 HTTP 模式。 |
| [medical-mcp](https://github.com/JamesANZ/medical-mcp) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/JamesANZ/medical-mcp?style=flat-square) | FDA 药物、WHO 统计、PubMed 检索。Google Scholar 部分在国内不可用。本地部署无需 API 密钥。 |
| [OMOP MCP](https://github.com/OHNLP/omop_mcp) | ⚠️ 部分可用 | — | 临床术语到 OMOP 概念映射。需要 API Key。对接 LOINC、SNOMED 等国际标准。 |
| [mcp-simple-pubmed](https://github.com/andybrandt/mcp-simple-pubmed) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/andybrandt/mcp-simple-pubmed?style=flat-square) | PubMed 文献搜索。PubMed 在国内可直接访问。 |
| [Awesome-MCP-ZH](https://github.com/yzfly/Awesome-MCP-ZH) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/yzfly/Awesome-MCP-ZH?style=flat-square) | MCP 中文资源精选，含部分医疗相关 MCP 服务器索引。 |

---

## 中医药 AI

> 中医智能化相关项目和工具。

| 项目 | 可用性 | Stars | 说明 |
|------|--------|-------|------|
| [tcm-video-factory](https://clawskills.sh/skills/tcm-video-factory) | ⚠️ 部分可用 | — | 基于 Perplexity API 的中医健康视频自动化制作（选题研究 → 脚本 → 角色 → 图像/视频提示）。OpenClaw 技能。 |

> 💡 **社区招募**：中医药 AI 是一个极具潜力但资源稀缺的方向。如果你有中医知识图谱、方剂数据库、辨证论治 Agent 等项目，欢迎提交 PR！

---

## 医学影像 AI

| 项目 | 可用性 | Stars | 说明 |
|------|--------|-------|------|
| [MedRAX](https://github.com/bowang-lab/MedRAX) | 🔧 需适配 | ![](https://img.shields.io/github/stars/bowang-lab/MedRAX?style=flat-square) | **ICML 2025**。胸部 X 光 AI 解读。需 GPU + 模型下载。依赖 GPT-4o（需代理）。 |
| [EasyLung](https://github.com/TommyZihao/EasyLung) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/TommyZihao/EasyLung?style=flat-square) | 从 X 光胸片中 AI 识别肺炎及病原体种类。包含网页、**微信小程序**、APP。 |
| [liver_cancer_classify](https://github.com/wuwusky/liver_cancer_classify) | ✅ 直接可用 | — | 肝癌影像 AI 诊断（3D-Conv 深度学习）。 |
| [Lambar_Spine_Slicer](https://github.com/Keyon-2580/Lambar_Spine_Slicer) | ✅ 直接可用 | — | 腰椎影像智能分割可视化系统。Vue+Django+3DUNet。 |
| [paddle-fl-gui](https://github.com/yyyanbj/paddle-fl-gui) | ✅ 直接可用 | — | 基于 PaddleFL 的联邦学习医疗影像识别 GUI。百度飞桨框架。 |

---

## 电子病历与临床系统

| 项目 | 可用性 | Stars | 说明 |
|------|--------|-------|------|
| [SoDiaoEditor](https://github.com/tlzzu/SoDiaoEditor) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/tlzzu/SoDiaoEditor?style=flat-square) | 电子病历编辑器。**已在多家三甲医院上线**，持续维护中。 |
| [HIS（ZainZhao）](https://github.com/ZainZhao/HIS) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/ZainZhao/HIS?style=flat-square) | 医院信息系统。门诊/药房/财务/患者管理工作站。Spring Boot。 |
| [HIS（TANGKUO）](https://github.com/TANGKUO/HIS) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/TANGKUO/HIS?style=flat-square) | 医院信息系统。临床诊疗、药品管理、财务管理、患者管理。 |
| [云医疗管理系统](https://github.com/Rain-Ricky/cloud) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/Rain-Ricky/cloud?style=flat-square) | 网上挂号、在线问诊、诊断报告查询、费用缴纳。Spring Boot + 前后端分离。 |

---

## 健康数据与可穿戴设备

### 国内主流设备

> 💡 **当前状态**：国内可穿戴设备（华为/小米/OPPO）的开放 API 较少，尚未发现专门的 Agent Skill。以下为已有的和国内可用的方案。

| 技能 | 平台 | 可用性 | 说明 |
|------|------|--------|------|
| [apple-health-skill](https://clawskills.sh/skills/nftechie-apple-health-skill) | OpenClaw | ✅ 直接可用 | Apple Health 数据查询（国内 iPhone 用户可用） |
| [healthkit-sync](https://clawskills.sh/skills/mneves75-healthkit-sync) | OpenClaw | ✅ 直接可用 | iOS HealthKit 数据同步 |
| [health-sync](https://clawskills.sh/skills/filipe-m-almeida-health-sync) | OpenClaw | ⚠️ 部分可用 | 多设备数据聚合（Oura/Withings/WHOOP 等，部分国内可用） |
| [health-summary](https://clawskills.sh/skills/yusaku-0426-health-summary) | OpenClaw | ✅ 直接可用 | 健康数据汇总报告生成 |

### Garmin（国内可用）

> Garmin 在国内有官方渠道，Connect 可用。

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [garmin-health](https://clawskills.sh/skills/eversonl-garmin-health-analysis) | ✅ 直接可用 | 自然语言查询 Garmin 数据 — 20+ 指标 |
| [garmin-cli](https://clawskills.sh/skills/voydz-garmin-cli) | ✅ 直接可用 | Garmin Connect CLI |
| [garmin-connect](https://clawskills.sh/skills/garmin-connect) | ✅ 直接可用 | 每 5 分钟自动同步 |

### 其他国际设备（国内部分可用）

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [fitbit](https://clawskills.sh/skills/mjrussell-fitbit) | ⚠️ 部分可用 | Fitbit 国内用户较少但可用 |
| [oura-analytics](https://clawskills.sh/skills/kesslerio-oura-analytics) | ⚠️ 部分可用 | Oura Ring 数据分析 |
| [withings-health](https://clawskills.sh/skills/withings-health) | ⚠️ 部分可用 | Withings 体重/体脂/活动/睡眠 |

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
| [therapy-mode](https://clawskills.sh/skills/therapy-mode) | ⚠️ 部分可用 | CBT/ACT/DBT/MI 治疗框架。英文为主。 |
| [anxiety-relief](https://clawskills.sh/skills/jhillin8-anxiety-relief) | ✅ 直接可用 | 焦虑缓解：接地练习和呼吸技巧 |
| [depression-support](https://clawskills.sh/skills/jhillin8-depression-support) | ✅ 直接可用 | 每日情绪追踪和抑郁支持 |
| [jungian-psychologist](https://clawskills.sh/skills/jungian-psychologist) | ⚠️ 部分可用 | 荣格心理学：阴影工作、原型分析、梦境解读 |
| [adhd-assistant](https://clawskills.sh/skills/thinktankmachine-adhd-assistant) | ✅ 直接可用 | ADHD 友好的生活管理助手 |
| [social-media-detox](https://clawskills.sh/skills/social-media-detox) | ✅ 直接可用 | 社交媒体戒瘾 + 数字健康 |

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
| [strava-cycling-coach](https://clawskills.sh/skills/strava-cycling-coach) | ⚠️ 部分可用 | Strava 骑行分析（国内 Strava 可用但用户较少） |

---

## 孕婴健康

| 技能 | 可用性 | 说明 |
|------|--------|------|
| [pregnancy-tracker](https://clawskills.sh/skills/pregnancy-tracker) | ✅ 直接可用 | 孕期追踪：每周更新、症状记录、里程碑倒计时 |
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
| [claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) | ⚠️ 部分可用 | ![](https://img.shields.io/github/stars/K-Dense-AI/claude-scientific-skills?style=flat-square) | 170+ 科学技能。生物信息学、化学信息学部分技能国内可用（本地计算为主）。 |
| [MedgeClaw](https://github.com/xjtulyc/MedgeClaw) | ✅ 直接可用 | ![](https://img.shields.io/github/stars/xjtulyc/MedgeClaw?style=flat-square) | 西安交大 — 生物医学 AI 研究助手。RNA-seq、药物发现、临床分析。基于 Claude Code。 |
| [dna-claude-analysis](https://github.com/shmlkv/dna-claude-analysis) | ⚠️ 部分可用 | — | 个人基因组分析。支持 23andMe/AncestryDNA（国内可用微基因、23魔方等替代）。 |

---

## 多智能体医疗系统

| 项目 | 可用性 | Stars | 说明 |
|------|--------|-------|------|
| [Multi-Agent-Medical-Assistant](https://github.com/souvikmajumder26/Multi-Agent-Medical-Assistant) | 🔧 需适配 | ![](https://img.shields.io/github/stars/souvikmajumder26/Multi-Agent-Medical-Assistant?style=flat-square) | 多智能体诊断和医疗研究聊天机器人 |
| [medgraph-ai](https://github.com/asanmateu/medgraph-ai) | 🔧 需适配 | — | Neo4j 知识图谱 + RAG 的医疗问答 |
| [SOLVE-Med](https://github.com/PRAISELab-PicusLab/SOLVE-Med) | ✅ 直接可用 | — | 面向隐私的多智能体医疗问答，可离线运行。 |

---

## 技能合集与资源

| 资源 | Stars | 说明 |
|------|-------|------|
| [awesome-openclaw-skills-zh](https://github.com/clawdbot-ai/awesome-openclaw-skills-zh) | ![](https://img.shields.io/github/stars/clawdbot-ai/awesome-openclaw-skills-zh?style=flat-square) | OpenClaw **中文官方技能库**。按场景分类，支持中文调用。 |
| [Awesome-MCP-ZH](https://github.com/yzfly/Awesome-MCP-ZH) | ![](https://img.shields.io/github/stars/yzfly/Awesome-MCP-ZH?style=flat-square) | MCP 中文资源精选合集 |
| [OpenClaw-Medical-Skills](https://github.com/FreedomIntelligence/OpenClaw-Medical-Skills) | ![](https://img.shields.io/github/stars/FreedomIntelligence/OpenClaw-Medical-Skills?style=flat-square) | 869 个医疗技能（港中文深圳团队） |
| [ai-guide（鱼皮）](https://github.com/liyupi/ai-guide) | ![](https://img.shields.io/github/stars/liyupi/ai-guide?style=flat-square) | AI 资源大全 + 教程。含 OpenClaw/Claude Code 教程、Skills 使用指南。 |

---

## 🔴 国内急需但尚缺的方向

以下方向在国内有强烈需求，但目前开源社区中尚无成熟的 Agent Skill：

| 方向 | 需求场景 | 难度 |
|------|---------|------|
| 🏥 **NMPA 药品/器械查询** | 查询国家药监局药品注册信息、器械注册状态 | ⭐⭐ |
| 💊 **国家基本药物目录** | 查询基药目录、医保目录、集采药品信息 | ⭐⭐ |
| 📋 **DRG/DIP 分组辅助** | 辅助 DRG/DIP 编码分组和费用预测 | ⭐⭐⭐ |
| 🏥 **互联网医院接口** | 对接微医、好大夫、丁香园等平台 API | ⭐⭐⭐ |
| 📱 **华为/小米健康数据** | 华为运动健康、小米健康 API 数据读取 | ⭐⭐⭐ |
| 🌿 **中医辨证论治 Agent** | 基于中医理论的智能辨证和方剂推荐 | ⭐⭐⭐⭐ |
| 🧬 **国内基因检测数据** | 对接微基因、23魔方等国内基因检测数据 | ⭐⭐⭐ |
| 📊 **卫健委数据接口** | 查询全国卫生统计、传染病疫情等公开数据 | ⭐⭐ |

**欢迎社区贡献！** 如果你正在开发以上方向的项目，请提交 PR。

---

## 微信/企业微信集成

以下技能支持通过微信或企业微信与 AI Agent 交互：

| 技能 | 平台 | 说明 |
|------|------|------|
| [wechat-mcp](https://clawskills.sh/skills/wechat-mcp) | OpenClaw | Windows 微信桌面端 MCP 集成 — 消息监控、搜索联系人、发送消息 |
| [wecom](https://clawskills.sh/skills/wecom) | OpenClaw | 通过 Webhook 向企业微信发送消息 |

---

## ⚠️ 免责声明

> 本列表中的所有技能仅供**信息参考和研究目的**。它们**不是**经过验证的临床工具，**不应**用于实际的医疗诊断或治疗决策。请始终咨询合格的医疗专业人员获取医疗建议。AI 生成的医疗信息可能不准确甚至有害。

---

## 参与贡献

欢迎贡献！特别欢迎以下类型的提交：

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
