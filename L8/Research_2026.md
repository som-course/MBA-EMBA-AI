# L8 · Forbes AI 50（2026）调研（截至 2026-11-14）

> 用途：替换原 PPT 的 "2025 年第七届 AI 50" 逐家介绍（P2–P57），并更新 P58–P69 的几个佐证。
> 标注：`⚠` = 二手整理 / 来源口径冲突 / 未能回到一手来源核对。课堂引用前请核对。

## 0. 原 PPT（Lecture_8.pptx，69 页）的逻辑

| 页 | 内容 |
|---|---|
| P1–P3 | 封面；2025 年第七届 Forbes AI 50 的发布方（Forbes + Sequoia + Meritech）；两个趋势：从"模型规模/聊天界面"走向"落地工作流"，生成式应用爆发带来算力需求；AI 50 2024 Visualized 地图 |
| P4–P53 | 50 家公司逐页：官网 / 估值 / 产品 / 用途 |
| P54–P57 | 四层归类：数据与知识层 → 开发与基础算力层 → 基础模型与通用平台层 → 应用层（应用层再按 7 个行业域展开） |
| P58 | 中国 AI App 50（按 MAU，2025.9） |
| P59–P60 | OpenAI 已使用超 1 万亿 token 的 30 家客户（DevDay 2025） |
| P64–P65 | Lean AI Native Companies Leaderboard：通往"一人独角兽"之路 |
| P61–P68 | "新一轮 AI 产业到底在改变什么？"→ 认知改变：个人（与 AI 交互）/ 组织（边界模糊）/ 系统（自然语言处理人与系统关系）；Steve Jobs 引语 |
| P69 | 谢谢 |

**主线**：先看"谁在做"（50 家）→ 再看"在哪一层做"（四层）→ 再看"为什么重要"（认知改变：个人/组织/系统）。

## 1. 2026 榜单（Forbes 第八届，2026-04-16）

**事实（一手：Forbes）** [R1][R2][R3][R4]
- 2026-04-16 发布；Forbes 与 Sequoia、Meritech 合作；**不排名、按字母序**；全球非上市公司；无申请费。
- 方法：Sequoia 合伙人 Konstantine Buhler 的算法初筛 → 前 70 家交由评委（学界 + 投资人）→ Forbes 编辑定稿。
- 50 家合计融资 **$305.6B**，其中 OpenAI $182.6B；OpenAI + Anthropic 共 $242.6B，约 80%。
- **20 家新晋**、30 家留任；4 家女性创始/领导公司（EliseAI、Fireworks AI、Thinking Machines Lab、World Labs）；33 家总部在加州。
- 2025 名单中 3 家被收购/人才收购：Scale AI（CEO Alexandr Wang 加入 Meta）、xAI（并入 SpaceX）、Windsurf（Google $2.4B 聘走联创并授权技术，Cognition 收购其余部分）。
- 五大趋势：摆脱对 Big AI 的依赖；效率优于规模；行业专用 AI 增长；AI Agent 进入职场；算力获取是竞争优势。
- 新设 **AI 50 Brink List**：20 家种子/A 轮公司，合计融资 > $35 亿，平均成立约 24 个月 [R5]。

**2026 名单（50 家）**：Abridge、Anthropic、Applied Intuition、Baseten、Black Forest Labs、Chai Discovery、Clay、Cognition、Cohere、Crusoe、Cursor、Cyera、Databricks、Decagon、ElevenLabs、EliseAI、Fal、Fireworks AI、Gamma、Genspark、Glean、Harvey、HeyGen、Krea、Legora、Listen Labs、Lovable、Mercor、Midjourney、Mistral AI、Notion、OpenAI、OpenEvidence、Perplexity、Physical Intelligence、Reflection、Replit、Rogo、Runway、Safe Superintelligence、SambaNova、Sierra、Skild AI、Speak、Suno、Surge AI、Synthesia、Thinking Machines Lab、Together AI、World Labs。

**与 2025 名单（原 PPT）对比**（本课自行比对）
- 留任 30：Abridge、Anthropic、Baseten、Clay、Cohere、Crusoe、Cursor、Databricks、Decagon、ElevenLabs、Fireworks、Glean、Harvey、Mercor、Midjourney、Mistral、Notion、OpenAI、OpenEvidence、Perplexity、Runway、SambaNova、Sierra、Skild、Speak、Suno、Synthesia、Thinking Machines、Together、World Labs。
- 退出 20：Captions、Coactive、DeepL、Figure、Hebbia、Hugging Face、Lambda、LangChain、Luminance、Photoroom、Pika、Sakana、Scale AI、Snorkel、StackBlitz、Vannevar Labs、VAST Data、Windsurf、Writer、xAI。（仅 3 家有"被收购"一手说明；其余只是**未入选**，原因不详，不应解读为失败。）
- 新晋 20 与 Forbes 新闻稿一致（Applied Intuition、Black Forest Labs、Chai Discovery、Cognition、Cyera、EliseAI、Fal、Gamma、Genspark、HeyGen、Krea、Legora、Listen Labs、Lovable、Physical Intelligence、Reflection、Replit、Rogo、Surge AI、SSI）。

**逐家融资/估值（二手整理 ⚠）** [R6][R7]：融资额以 Forbes 为口径，经 foundevo、Shota Sawada（note.com）汇总；估值为 2026-04 前后公开报道。本课用这两份表复算：融资总和与 Forbes 的 $305.6B 一致（见 `src/slides/00-data.html` 内的 `CO` 数据，页面上标 ⚠）。
- 中位数融资约 $735M（⚠ 二手计算）；成立于 2022 年及之后的 28 家（⚠，据 foundevo 的成立年份计数）；旧金山 25 家（⚠ 二手）。
- Midjourney、Surge AI 在 Forbes 口径下融资为 $0（未接受外部融资）。

## 2. 发榜之后的七个月（2026-04 → 2026-11）

| 事件 | 数据 | 来源 |
|---|---|---|
| Anthropic | 2026-05 融资 $65B，投后估值 $965B；**2026-11-10 启动 IPO 路演**，拟发 8.25 亿股、$70–78，计划 11-18 定价、11-19 在 Nasdaq 以 ANT 交易；估值区间报道不一：CNBC/Yahoo 称完全稀释后约 $1.3–1.45T，NBC/Reuters 另有"最高约 $1.02T"的表述 ⚠（口径不同） | [R8] |
| OpenAI | 2026-03/04 融资 $122B、$852B；2026-11 新一轮已入账 $11B、估值 $1.25T（Bloomberg，原计划 $30B 未达）；IPO 推迟到 2027 | [R9] |
| Cursor | 2026-02/03 年化收入 > $20 亿；2026-04 传 $500 亿估值融资；**2026-06 SpaceX 宣布 $600 亿收购，8 月完成** | [R10][R11] |
| Databricks | 2026-08 融资 $50 亿、估值 $1,900 亿；年化收入 > $70 亿，Q2 同比增长 > 80%；调整后现金流为正 | [R12] |
| Cognition | 2026-09 融资 > $20 亿、估值 $480 亿（年化收入由 5 月 $4.92 亿升至近 $9 亿） | [R13] |
| Harvey | 2026-09 融资 $5.5 亿、估值 $155 亿 | [R14] |
| Mistral | 2026-09 Series D €30 亿，投后 > €210 亿 | [R15] |
| 其他 | Cohere Series E（C$357 亿，Cohere 口径 ⚠）、SSI 本季融资 $50 亿、TML 洽谈 ≥ $400 亿（⚠ 洽谈中）；OpenRouter（Brink List 公司）被 Stripe 以 > $70 亿收购（⚠ 据知情人士） | [R16][R17][R18] |
| 资本市场 | Crunchbase：2026 Q3 全球风险投资 $159B，AI 公司 $102B（64%）；27 家公司融资 ≥ $10 亿（纪录）；Q1–Q3 累计 $679B | [R17] |
| 估值倍数 ⚠ | BlockWest：Anthropic 约 14.8× 年化收入（私募最后一轮），OpenAI 约 35.5×，Mistral 约 61×，Cohere 约 85×（二手，仅示意量级） | [R16] |

## 3. 其他板块的更新

- **中国 AI App**（原 P58，非凡产研 2025-09）→ QuestMobile 2026-09（AI 原生 App 月活）：豆包 4.19 亿（同比 +143.6%）、千问 1.58 亿（同比 +5076.6%，低基数）、DeepSeek 1.23 亿（同比 −15.2%）、元宝 3,733 万、蚂蚁阿福 3,479 万。办公 Agent 榜：腾讯 WorkBuddy 3,235 万居首。**两榜口径不同**（原榜含百度搜索等 AI 搜索，QuestMobile 是"AI 原生 App"），不能直接比较 [R19]。
- **OpenAI 万亿 token 客户**（原 P59–P60，DevDay 2025 的 30 家）→ 2026：OpenAI 称 API 每分钟处理超 150 亿 token（DevDay 2025 为 60 亿/分钟），企业收入占比 > 40%，预计 2026 年底与消费者持平 [R20]；另据其企业报告，约 200 家组织累计处理超 1 万亿 token（⚠ 二手转述）[R21]。
- **Lean AI Native Leaderboard**（原 P64–P65）：原 PPT 截图为 2025 年快照（总收入 $37.8 亿、人均 $249 万、平均 27 人）。2026 的实时数据网页为动态加载，**未能核对**，本课只用截图与 Forbes 的案例（Gamma 50 人年化收入 > $1 亿；Midjourney 零融资）[R22][R3]。

## 4. 来源表

- R1 Forbes, *Forbes 2026 AI 50 List*, 2026-04-16 — forbes.com/lists/ai50
- R2 Forbes, *Forbes Unveils 2026 AI 50, Marking Shift From AI Dominance To AI Independence*, 2026-04-16
- R3 E. Brier, *Forbes 2026 AI 50 List*（Forbes Middle East 转载），2026-04-17
- R4 E. Brier, *How Forbes Compiled The 2026 AI 50 List*, 2026-04-16
- R5 S. Chierchio, R. Shrivastava, *The AI 50 Brink List*, Forbes, 2026-04-16
- R6 foundevo, *Forbes AI 50 List 2026*（二手 ⚠），2026-04-29
- R7 Shota Sawada, *I researched all 50 companies on the Forbes AI 50*（二手 ⚠），note.com，2026-08-01
- R8 Anthropic, *Roadshow launch*, 2026-11-10；CNBC 2026-11-10；Yahoo Finance 2026-11-13；NBC/Reuters 2026-11-10
- R9 The Verge / Bloomberg, *OpenAI valued at $1.25 trillion*, 2026-11；Reuters 2026-10-19
- R10 Forbes, *SpaceX Will Buy AI Coding Firm Cursor For $60 Billion*, 2026-06-16；stockanalysis.com（8 月完成 ⚠ 二手）
- R11 TechCrunch, 2026-03-02、2026-04-17
- R12 Reuters, *Databricks valued at $190 billion*, 2026-08-13
- R13 Bloomberg, *Cognition raises $2 billion at a $48 billion value*, 2026-09-08
- R14 Harvey, *Harvey raises $550M at $15.5B*, 2026-09-09
- R15 TapToMarket, *AI funding week Sep 8–14, 2026*
- R16 BlockWest Research, *AI lab funding tracker, October 2026*（二手 ⚠）
- R17 Crunchbase News, *Q3 2026 global startup funding*, 2026-10-05
- R18 Fortune, *Stripe clinches over $7 billion deal to buy OpenRouter*, 2026-08-16
- R19 QuestMobile（经 199IT、快科技、虎嗅转载），2026-10-20
- R20 OpenAI, *The next phase of enterprise AI*, 2026
- R21 shuaiguan.io, *OpenAI Statistics*（二手 ⚠）
- R22 leanaileaderboard.com（H. Shi），原 PPT 截图
- R23 Forbes, *AI 50 2025*（Forbes Middle East 转载）
- R24 原 PPT Materials/Lecture_8.pptx（P1–P69）
