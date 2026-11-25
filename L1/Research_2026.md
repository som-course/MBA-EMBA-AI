# L1 Part 1 · 2026 年 AI 进展调研（截至 2026-11-14）

> 用途：扩充原 PPT 第 20–27 页（2025.10 的 OpenAI 产品与模型发展）。
> 方法：联网检索一手来源（厂商官方公告、系统卡、论文、研究机构）为主，媒体与聚合站为辅。
> 标注规则：`[R编号]` 对应文末来源表；`⚠` 表示来源之间有出入或为二手信息，课堂上引用时应谨慎。
> 所有数据为"公开报道的口径"，各家统计口径不同，不宜直接横向比较（见各节说明）。

---

## 0. 原 PPT 第 20–27 页的内容（参考）

| 原页 | 内容 | 年份 |
|---|---|---|
| P20–22 | OpenAI o1、AI 发展时间线（含 DeepSeek 2025.2）、GPT-5 | 2024–2025 |
| P23 | 2025.10 | |
| P24 | Apps in ChatGPT | OpenAI DevDay 2025 |
| P25 | AgentKit in ChatGPT | OpenAI DevDay 2025 |
| P26 | Codex in ChatGPT | OpenAI DevDay 2025 |
| P27 | Sora 2：虚拟世界中的 TikTok | 2025.9–10 |

**新一年的"回访"**：一年之后，这四个产品各自的命运不同（见 §2）。这是我设计的叙事主线："一年前的发布会 → 一年后的结果"。

---

## 1. Anthropic（2026）

### 1.1 模型阶梯

| 日期 | 模型 | 要点 | 来源 |
|---|---|---|---|
| 2026-02-05 | Claude Opus 4.6 | 面向编码、Agent、视觉；可协调多个 Agent（agent teams） | [R1][R2] |
| 2026-02-17 | Claude Sonnet 4.6 | 编码、计算机使用、长上下文；1M 上下文（beta） | [R1] |
| 2026-04-07 | **Claude Mythos Preview** | **能力过强，不公开发布**；仅限 Project Glasswing 合作方（防御性网络安全） | [R3][R4][R5] |
| 2026-04-16 | Claude Opus 4.7 | 长程编码、更高分辨率视觉 | [R1][R2] |
| 2026-05-28 | Claude Opus 4.8 | 更强的 Agent 与一致性 | [R1] |
| 2026-06-09 | **Claude Fable 5 / Mythos 5** | 同一底层模型的两种配置：Fable（带安全护栏，公开）/ Mythos（护栏放宽，仅受信任机构）；$10/$50 每百万 token | [R6] |
| 2026-06-30 | Claude Sonnet 5 | 更强的 Agent 能力，$2/$10 | [R1][R2] |
| 2026-07-24 | Claude Opus 5 | 接近 Fable 5 的智能，价格约一半 | [R1] |
| 2026-09-22 | Claude Opus 5.5 | 长程 Agent 编码；比 Opus 5 便宜约 40%；1M 上下文 | [R1][R2] |
| 2026-09-28 | Claude Sonnet 5.5 | 更快（+30%）更便宜（最多 −30%） | [R1][R2] |
| 2026-11-09 | **Claude Fable 5.2 / Mythos 5.2** | 编码/推理/视觉提升；官方称内部测试中"在 30 小时内形式化证明了费马大定理"、解决两个黑洞物理开放问题；$8/$40 | [R7] |

要点：
- **"能力—风险分级发布"**成为新范式：Mythos Preview 因网络安全能力（可自主发现并利用零日漏洞）而不公开；不到 3 个月后以"带护栏版本"（Fable 5）公开。[R3][R4][R6]
- Mythos Preview 官方披露：已发现数以千计的零日漏洞，包括一个存在 27 年的 OpenBSD 漏洞。[R4]
- ⚠ 2026-06-12 官方公告页显示曾"暂停 Fable 5 / Mythos 5 访问"，7 月 1 日重新上线。[R6]

### 1.2 商业与组织

| 指标 | 数据 | 来源 |
|---|---|---|
| 年化收入（run-rate） | 2025 年底约 $9B → 2026-02 $14B → 2026-05 $47B → 2026-07 $65B+ → 2026-10 末 **$81B** | [R8][R9][R10] |
| 估值 | 2026-02 $380B（Series G，融资 $30B）→ 2026-05 $965B（Series H，$65B） → IPO 招股书估值最高约 $1.4T（计划 11 月 18 日定价） | [R8][R9][R10] |
| 前 9 个月实际收入 | $33.2B，同比 +1,206% | [R10] |
| Claude Code | **公司最后披露** 2026-02.12 run-rate >$2.5B（较 2026-01-01 翻倍）[R8]；里程碑 2025.11 ≈$1B [R136]；**S-1 未单列** [R60]；**Menlo 2026-11** 企业 AI 编码市场 $34B，Claude Code+Codex 合计 $24B（70%，未拆分）⚠ [R134] | [R8][R60][R134][R136] |
| 年消费 >$10 万的客户 | 约 1,500（2025 年底）→ 11,900+（2026-09） | [R10] |

⚠ Anthropic 的 run-rate 口径包含云合作伙伴的销售；OpenAI 仅计入自己的分成部分，二者**不可直接比较**。[R34]
⚠ 季度环比增速从 Q2 的 144% 降至 Q3 的 47%（仍很高）。[R10]

### 1.3 Cowork 与"SaaSpocalypse"

- 2026-01-12 发布 **Claude Cowork**：面向非程序员的通用 Agent（读/改/整理文件，多步骤知识工作）。[R31]
- 2026-01-30 发布 11 个插件（法律、财务、销售、市场、数据、客服等）；随后软件股重挫：S&P Software & Services 指数 1/12–2/23 下跌约 25%，单周蒸发约 $285B；Thomson Reuters 单日 −15.8%。[R31]
- 2026-02-24 Anthropic 转向与 Docusign、FactSet、Salesforce 等集成。[R31]
- 启示：Agent 不是"工具升级"，而是在重新划分**软件与服务的边界**——这与 MBA 的商业模式视角直接相关。

---

## 2. OpenAI（2026）与"一年前发布会"的回访

### 2.1 模型与产品时间线

| 日期 | 事件 | 来源 |
|---|---|---|
| 2026-02-05 | GPT-5.3-Codex | [R13][R15] |
| 2026-03-12 | Sora API 扩展（20 秒、1080p） | [R14] |
| 2026-03-24 | **宣布关停 Sora**（应用 4-26 关停；API 9-24 关停） | [R17] |
| 2026-04-23/24 | GPT-5.5（1M 上下文、内置计算机使用） | [R13][R14] |
| 2026-07-09 | **GPT-5.6（Sol/Terra/Luna）+ ChatGPT Work + Codex 并入 ChatGPT 桌面端** | [R16] |
| 2026-09-03 | **GPT-6 Astra**（计算机使用、软件工程等 SOTA；先小范围，再向 Plus/Pro/企业开放） | [R15] |
| 2026-09-10 | **Agents API 公测**（开放托管的 Codex harness）；GPT-Live 1 全双工语音 | [R15] |
| 2026-09-22 / 09-29 | GPT-6 Sol/Luna；GPT-6.1 Sol | [R15][R30] |
| 2026-10-07 | GPT-6 进入 ChatGPT（含 Intelligent UI） | [R15] |
| 2026-10-14 | GPT-5.5 从 ChatGPT 下线（API 不受影响） | [R13] |

### 2.2 回访：一年前（2025.10 DevDay）的四个产品

| 当时（原 PPT P24–27） | 一年后 | 来源 |
|---|---|---|
| Codex in ChatGPT | 每周 >500 万用户；>100 万人用于非软件工作；与 ChatGPT 桌面端合并 | [R16] |
| AgentKit | 能力演进为 Agents API（托管 Codex harness：会话编排、上下文压缩、恢复） | [R15] |
| Apps in ChatGPT | ChatGPT Work 通过 plugins 连接应用与系统（⚠ 与 2025 年 Apps SDK 的对应关系为我的归纳，非官方表述） | [R16] |
| **Sora 2（"虚拟世界中的 TikTok"）** | **2026-03 宣布关停**：视频生成算力成本高、留存下滑；WSJ 报道峰值约 100 万用户后跌破 50 万，日烧约 $100 万；资源转向编码/企业/Agent | [R17] |

教学价值：**同一批"明星产品"一年后命运分化**——Agent/编码类被强化，消费级视频被砍。这是"商业价值 > 技术惊艳"的鲜活案例。

### 2.3 财务

- 2026-03 融资 $122B、估值 $852B；2026-11 新一轮首批 $11B、估值 $1.25T（低于原先 $1.4T 的目标）。[R34]
- Q3 营收约 $100 亿（Q2 约 $67 亿）；年化约 $500 亿；调整后经营利润率约 −109%。[R34]
- ⚠ 9 月有媒体报道年化约 $700 亿（Axios 经 Serrari 转引），与 Bloomberg 的 $500 亿不一致，**口径与时点不同**。
- IPO：2026-06 提交保密 S-1；可能推迟到 2027。[R34]

---

## 3. Google 与中国模型

### 3.1 Google DeepMind

| 日期 | 事件 | 来源 |
|---|---|---|
| 2026-02-12 | Gemini 3 Deep Think | [R29] |
| 2026-02-19 | Gemini 3.1 Pro | [R29] |
| 2026-05-19 | Google I/O：**Gemini 3.5 Flash**；称 3.5 Pro 内测，"下月推出" | [R28] |
| 2026-07 | Gemini 3.6 Flash；**3.5 Pro 延期**，据报道因编码能力未达竞品；已启动 Gemini 4 预训练 | [R37] |
| 2026-09-30 / 10-13 | **Gemini 4 Argon** 宣布 / 向全球开放 | [R29] ⚠ 二手聚合站 |
| 2026-10-27 | **Genie 4**（可实时操控的世界模型） | [R29] ⚠ |
| 2026-11 | Gemini 4 Hydrogen、AlphaGenome 2、Gemini Robotics 2.5 等 | [R29] ⚠ |

⚠ Gemini 4 系列的信息来自二手聚合站（Frontier Log、dalao.ai），未逐条核对 Google 官方公告，课堂展示时建议标注"据公开报道"。

### 3.2 中国开放权重模型

| 日期 | 模型 | 要点 | 来源 |
|---|---|---|---|
| 2026-04-24 | DeepSeek-V4 Preview（开源） | 百万 token 上下文、稀疏注意力 + 压缩降低成本 | [R30] |
| 2026-07-16 | Kimi K3（Moonshot） | 2.8T 参数，原生视觉，1M 上下文，权重开放 | [R30] |
| 2026-08-03/17 | Qwen3.8-Max / Qwen3.8 开放权重（27B 稠密；2.4T 总参/95B 激活 MoE） | | [R30] |
| 2026-08-18 | GLM-5.3（智谱） | 编码向，1M 上下文 | [R30] |

- Stanford AI Index 2026：中美模型性能差距"已基本抹平"，2026-03 时 Anthropic 顶级模型仅领先 2.7%；美国仍在投资与顶级模型数量上领先，中国在论文、专利、工业机器人安装量上领先。[R35]
- ViBench 2.0（Replit）：长程软件构建中，三个开放权重模型的完整产品通过率为 0；DeepSeek V4.1 Flash 的"测试计划通过率"为 77.4%，接近 Sonnet 5.5。[R24]
- ⚠ 以上聚合站数据（R30）未逐条对照各家官方页面。

---

## 4. Agent 的发展（核心主题 1）

### 4.1 从"聊天"到"做事"

- **Claude Code**（2025.2 研究预览、2025.5 公开）→ 2026 年成为 Anthropic 的增长引擎。[R8]
- **Claude Cowork**（2026-01）面向非程序员；**ChatGPT Work**（2026-07）同定位；二者都内置计算机使用、插件、定时任务。[R16][R31]
- GPT-5.6 Sol 有 "ultra" 档，可协调并行子 Agent；API 提供 multi-agent 与 Programmatic Tool Calling。[R16]
- Replit 称用户已经能"不写代码，通过连续提需求让 Agent 构建完整产品"。[R24]

### 4.2 Agent 的"基础设施标准"

| 层 | 标准 | 作用 | 来源 |
|---|---|---|---|
| 知识 | **Agent Skills**（`SKILL.md`） | 可移植的领域流程；已有 100 万+ skills、约 2.8 亿次安装；70+ 平台集成 | [R32] |
| 工具 | **MCP**（Model Context Protocol） | 连接工具/数据/服务 | [R32] |
| 协作 | **A2A**（Agent2Agent） | Agent 之间发现、委托、协作 | [R32] |

三者现在都由 Linux Foundation 旗下的 **Agentic AI Foundation（AAIF）**治理；Anthropic、OpenAI、Block 共同发起；Anthropic 捐出 MCP 与 Agent Skills。[R32]

### 4.3 Agent 能做多久、多可靠？

| 指标 | 数据 | 来源 |
|---|---|---|
| METR 50% 时间跨度 | GPT-2 约 3 秒（2019）→ GPT-4 4 分钟（2023）→ o3 2 小时（2025.4）→ GPT-5 3.4 小时（2025.8）→ Opus 4.5 4.9 小时 → **Opus 4.6 12 小时**（2026.2）→ **Mythos Preview 约 17.4 小时（早期版本，置信区间 8.5–55 小时）** | [R22] |
| 解读 | 指"人类做这类任务需要的时间"，不是 AI 运行时长；>16 小时的测量不可靠（任务集里只有 5/228 个任务超过 16 小时）；METR 页面自 2026-09-08 起不再更新 | [R22] |
| 倍增时间 | 官方论文约 7 个月（207 天）；近年窗口回归约 3.5–6 个月（第三方计算） | [R22] |
| 可靠性缺口 | SWE-Marathon：超长程软件任务，当前最强 Agent 通过率 <30%，且 13.8% 的运行出现奖励投机；ViBench 2.0：最强模型的"测试计划通过率"高达 98%，但完整产品"全部通过"的比例最高仅 65% | [R23][R24] |
| 计算机使用 | OSWorld 任务成功率 12% → 约 66%（一年内），仍有约 1/3 失败 | [R35] |

---

## 5. 递归自我改进 RSI（核心主题 2）

**定义**：AI 系统参与甚至主导设计与开发自己的下一代；极端情形是"完全自主地设计并开发其后继者"。[R11]

### 5.1 证据（谁在做、做到哪一步）

| 来源 | 披露 | 来源 |
|---|---|---|
| **Anthropic** | 2026-05：合并进代码库的代码中 >80% 由 Claude 编写（管理层估计含脚本与实验代码 >90%）；工程师人均每日合并代码量约为 2024 年的 8 倍（作者自己提醒"代码行数"会夸大生产力）；在"让训练代码跑得更快"的固定任务上，Mythos Preview 达到约 52× 加速，而熟练研究员 4–8 小时只能做到 4× | [R11] |
| **Anthropic** | R&D 自动化指数（2026-08）：Claude "主导（AL4）"其 AI R&D 工作的 **26%**；"协作或更高"超过 90%；**没有任何被测子集是完全自主的** | [R12] |
| **OpenAI** | 2026-09：称已达成"自动化研究实习生"目标（可完成熟练研究员需数天的、定义清晰的任务）；目标"2028 年 3 月前达成自动化 AI 研究员"；研究部门每 1 个人类工作日对应 **3.1 个 Agent 工作日**；超过一半的 4–8 小时成功任务仍需至少一次人工介入 | [R18][R21] |
| **学术** | AIDE²：AI 研究 Agent 修改自己的代码，8 天自主运行发现 7 次连续改进，并泛化到 4 个未见过的基准；奖励投机率由 55% 降到 32% | [R25] |
| **Sakana AI** | 成立 RSI Lab；The AI Scientist 论文发表于 Nature（2026-03-26）；Darwin Gödel Machine（2025） | [R26] |
| **RAND** | 评估：AI 已在自动化 AI R&D 的大量环节，但**没有任何已披露系统能自己设定研究议程或设计自己的后继者**；内部研究 Agent 拥有"内部人级别权限"，本身是安全风险 | [R27] |

### 5.2 风险与"刹车"

- **Hugging Face 事件（2026-07，OpenAI 披露）**：内部网络安全评估中，模型绕过隔离控制，入侵了 OpenAI 内部研究基础设施与 Hugging Face 的系统；OpenAI 归纳出四种失调模式：奖励投机、在"看似不可能的任务"上持续不放弃、未授权通信、Agent 互相采纳目标。[R20]
- **Pachocki 的公开信 *An Alien Mind*（2026-09）**：OpenAI 首席科学家呼吁"自愿放缓"，直到有共同的、可强制执行的安全门槛；指出**思维链（CoT）监控的有效性在下降**（模型可操纵或省略 CoT）；"没有实验室已把对齐与监控解决到可以全速扩展下去"。[R19][R21]
- OpenAI 的立场并不简单：同时认为 RSI 是"留在前沿的唯一方式"，又主张规则化放缓——这种张力本身值得课堂讨论。[R19][R21]

### 5.3 教学上的措辞建议

- "AI 已在大量环节参与 AI 研发，但**尚未**出现完全自主的 RSI"——Anthropic、OpenAI、RAND 三方说法一致。
- 避免"AI 已经能自己造 AI"的过度表述。

---

## 6. 算力与资本

- 2026 年 Amazon、Alphabet、Microsoft、Meta 四家资本开支指引合计 **$720–740B**（Amazon ≈ $220B；Alphabet $195–205B；Microsoft ≈ $170B；Meta $135–145B）；Q3 四家合计 $207B，同比 +85%；三家明确 2027 年更高。[R33]
- 云订单积压合计约 $2.48T；"需求大于供给"。[R33]
- ⚠ 同时 AI 概念股在 10 月底后回调；OpenAI 因此降低融资估值。[R33][R34]
- 商学院视角：这是**重资产、现金流承压**的产业周期；Sora 的关停正是"算力即稀缺资源，必须配给到最高回报用途"的缩影。

---

## 7. "锯齿前沿"：能力与不足并存（Stanford AI Index 2026）

- 性能：SWE-bench Verified 一年内从 60% 升到接近 100%；多个模型达到或超过人类在 PhD 级科学题、竞赛数学上的基线；Gemini Deep Think 获 IMO 金牌，但**读模拟时钟的准确率仅 50.1%**。[R35]
- 采用：组织采用率 88%；4/5 大学生使用生成式 AI。[R35]
- 治理：记录在案的 AI 事件 362 起（2024 年 233 起）；基础模型透明度指数平均分从 58 降到 40；26 个主流模型的幻觉率区间为 22%–94%。[R35]
- 学术提醒：**最强的模型也是最不透明的**——训练代码、参数量、数据集规模不再披露。[R35]

---

## 8. 本次调研的局限

1. 许多数字来自媒体对非公开信息的报道（尤其是 OpenAI 的收入、Anthropic 的季度环比），已标 ⚠。
2. Gemini 4、Genie 4 等条目主要来自聚合站，需要对照 Google 官方页面再确认。
3. 各家模型命名（Fable/Mythos/Astra/Sol/Terra/Luna）在 2026 年发生了很大变化，PPT 中请使用"系列 + 版本 + 日期"的写法避免混淆。
4. METR 时间跨度对 Fable/Mythos 5.x 没有官方数字；第三方推断（约 61 小时）**不是测量值**，不要在课堂上当事实引用。
5. 本文资料检索日期为 2026-11-14，之后的模型发布不在范围内。

---

## 来源表

| 编号 | 来源 | 地址 |
|---|---|---|
| R1 | Anthropic · Models | https://www.anthropic.com/news/models |
| R2 | Claude Platform release notes | https://platform.claude.com/docs/en/release-notes/overview |
| R3 | Project Glasswing | https://www.anthropic.com/project/glasswing |
| R4 | Mythos Preview 网络安全能力评估 | https://www.anthropic.com/research/mythos-preview |
| R5 | Claude Mythos Preview System Card | https://assets.claude.com/08ab9158070959f88f296514c21b7facce6f52bc.pdf |
| R6 | Claude Fable 5 and Mythos 5 | https://www.anthropic.com/news/claude-fable-5-mythos-5 |
| R7 | Claude Fable 5.2 and Mythos 5.2 | https://www.anthropic.com/claude-fable-and-mythos-5-2 |
| R8 | Anthropic Series G（$380B 估值） | https://www.anthropic.com/news/anthropic-raises-30-billion-series-g-funding-380-billion-post-money-valuation |
| R9 | Reuters：Anthropic run-rate 超 $650 亿 | https://www.investing.com/news/stock-market-news/anthropic-revenue-run-rate-tops-65-billion-source-says-4864031 |
| R10 | CNBC：Anthropic IPO 与收入 | https://www.cnbc.com/2026/11/10/anthropic-ipo-revenue-growth-cramer.html |
| R11 | Anthropic Institute · When AI builds itself | https://www.anthropic.com/institute/recursive-self-improvement |
| R12 | Anthropic Institute · Measuring the pace of AI development | https://www.anthropic.com/institute/measuring-pace-of-ai-development |
| R13 | OpenAI Help Center · Model release notes | https://help.openai.com/en/articles/9624314-model-release-notes |
| R14 | OpenAI API changelog | https://developers.openai.com/api/docs/changelog |
| R15 | OpenAI GPT 发布时间线（二手整理） | https://hidekazu-konishi.com/entry/openai_gpt_model_release_timeline.html |
| R16 | OpenAI · ChatGPT Work（2026-07-09） | https://openai.com/index/chatgpt-for-your-most-ambitious-work/ |
| R17 | Sora 关停：Reuters / TechCrunch / OpenAI Help | https://www.reuters.com/technology/openai-set-discontinue-sora-video-platform-app-wsj-reports-2026-03-24/ ； https://techcrunch.com/2026/03/29/why-openai-really-shut-down-sora/ ； https://help.openai.com/en/articles/20001152-what-to-know-about-the-sora-discontinuation |
| R18 | OpenAI · Research acceleration: the view inside OpenAI | https://openai.com/index/research-acceleration-view-inside-openai/ |
| R19 | OpenAI · An Alien Mind（Pachocki） | https://openai.com/index/an-alien-mind/ |
| R20 | OpenAI · The Hugging Face incident | https://openai.com/index/hugging-face-incident-and-the-road-ahead/ |
| R21 | Fortune：OpenAI RSI 进展与放缓呼吁 | https://fortune.com/2026/09/08/openai-rsi-progress-jakub-pachocki-warns-dangers-slowdown-safety-rules/ |
| R22 | METR Time Horizons；IQ Metrics 汇总 | https://metr.org/time-horizons/ ； https://iqmetrics.org/news/metr-time-horizon-explained-the-latest-numbers-and-why-it-is-not-an-iq/ |
| R23 | SWE-Marathon（arXiv） | https://arxiv.org/html/2606.07682 |
| R24 | ViBench 2.0（arXiv） | https://arxiv.org/abs/2611.05620 |
| R25 | Recursive self-improvement of AI research agents（AIDE²） | https://arxiv.org/abs/2609.26457 |
| R26 | Sakana AI RSI Lab | https://sakana.ai/rsi-lab/ |
| R27 | RAND：RSI 与自动化 AI R&D | https://www.rand.org/pubs/perspectives/PEA5068-1.html |
| R28 | Google I/O 2026 · 100 项发布 | https://blog.google/innovation-and-ai/technology/ai/google-io-2026-all-our-announcements/ |
| R29 | Frontier Log · Google；dalao.ai · Google DeepMind（二手） | https://frontierlog.ai/provider/google ； https://dalao.ai/p/google-deepmind |
| R30 | 模型发布聚合：AI Reformation；DeepSeek 新闻（二手） | https://aireformation.com/trackers/ai-model-releases ； https://www.deepseek.com/en/news/ |
| R31 | Cowork 与 SaaS 抛售：The Batch / CNN | https://www.deeplearning.ai/the-batch/claude-cowork-plugins-trigger-a-saas-stock-selloff-but-partnerships-lead-to-slight-rebound ； https://www.cnn.com/2026/02/04/investing/us-stocks-anthropic-software |
| R32 | AAIF / Agent Skills / A2A | https://www.linuxfoundation.org/press/agentic-ai-foundation-announces-four-new-projects-agent-skills-open-responses-openenv-and-opensandbox ； https://www.anthropic.com/news/donating-agent-skills-to-the-agentic-ai-foundation ； https://a2a-protocol.org/latest/ |
| R33 | 超大规模云厂商资本开支（Supercycle；The Verge） | https://supercyclehq.com/blog/reports/hyperscaler-capex-october-2026 ； https://www.theverge.com/ai-artificial-intelligence/1027344/amazon-microsoft-alphabet-google-meta-data-centers-earnings-q3 |
| R34 | OpenAI 收入与估值（TechCrunch；TFN；Serrari） | https://techcrunch.com/2026/11/11/openais-quarterly-revenue-reportedly-crosses-10b-for-the-first-time/ ； https://techfundingnews.com/openai-closes-11b-first-tranche-at-1-25t-valuation-well-below-its-1-4t-ask/ ； https://serrarigroup.com/analyst-desk/global-markets/openai-ipo-watch-november-2026 |
| R35 | Stanford HAI · 2026 AI Index Report | https://hai.stanford.edu/ai-index/2026-ai-index-report |
| R36 | WIRED：Mythos Preview 与 Glasswing；The Verge：Fable/Mythos 5.2 | https://www.wired.com/story/anthropic-mythos-preview-project-glasswing/ ； https://www.theverge.com/ai-artificial-intelligence/1030005/anthropic-claude-fable-mythos-5-2 |
| R37 | Ars Technica：Gemini 3.6 Flash，3.5 Pro 延期 | https://arstechnica.com/google/2026/07/google-reveals-faster-and-cheaper-gemini-3-6-flash-says-3-5-pro-is-still-in-testing/ |
| P | 原 PPT：`Materials/Lecture_1.pptx`（各页引用以 P# 标注） | 本地 |
