# xuanji-decision

> A mystical fork-resolution skill for agent workflows.  
>
> 当理性分析只剩平局，玄机决负责落下最后一锤。  
> When rational analysis produces a draw, xuanji-decision delivers the final ruling.

---

## 中文介绍

**玄机决（xuanji-decision）** 是一个开源 Skill。  
一个**项目分叉点玄断插件**。

当 Agent 在真实项目推进过程中遇到 A / B 两条都成立、继续理性分析只会拖慢推进的分叉点时，玄机决会把这个问题视作**一局未定之象**，借命理四书的判断框架给出一个带玄意的裁断，帮助流程继续前进。

### 它解决什么问题

很多项目型 Agent 都会卡在这种时刻：

- 先做内容验证，还是先做 MVP
- 先卖服务，还是先做订阅工具
- 做单点产品，还是做平台型结构
- 先聚焦一类用户，还是先做泛用户
- 现在发版本，还是再打磨一周

这些问题常常不是信息不足，而是：

> **两边都成立，但必须先落一子。**

玄机决做的，就是在这种“理性平局”里，给出一个更像**断局**而不是**咨询**的拍板结果。

### 核心设计

玄机决以命理四书为思维骨架：

- **《滴天髓》**：观势
- **《穷通宝鉴》**：调候
- **《渊海子平》**：辨格局
- **《三命通会》**：察组合与时机

它不追求真正传统命理排盘，而是把这些命理体系里的判断习惯，转译成项目分叉决策语言：

- 势在何方
- 当前最缺什么
- 哪条路更成局
- 现在是不是其时

最后输出：

- 局名
- 断势
- 调候
- 辨格局
- 察时机
- 总断
- 行动令

### 适用场景

**最适合：**

- 产品方向分叉
- 商业模式分叉
- 执行节奏分叉
- 用户定位分叉
- 内容策略分叉

**弱适用：**

- 品牌调性
- 文案风格
- 视觉气质

**不适合：**

- 医疗、法律、生死、重大财务判断
- 明显存在客观最优解的问题
- 事实严重不足的问题

### 当前状态

当前版本已经：

- 完成 skill creator 标准化整理
- 通过校验与打包
- 具备可分发 `.skill` 产物
- 完成若干轮手工压测

但它仍然是一个会继续迭代的 v1：

- 词库还可以继续加厚
- 弱断 / 拒断策略还能继续细化
- 项目分叉点映射还可以继续扩展

### 安装

如果你的运行环境支持 OpenClaw Skill 包，可直接使用：

- `dist/xuanji-decision.skill`

如果你想阅读或修改 Skill 源文件，请查看：

- `skill/SKILL.md`
- `skill/references/*`

### 开源说明

本仓库公开的是：

- Skill 设计
- 引用词库
- 映射规则
- 打包产物

如果你基于它继续扩写、再训练、再包装，欢迎保留来源说明。

### 后续计划

- 增加更多标准测试样例
- 扩展品牌 / 调性分叉场景的弱断策略
- 加入更细的项目阶段映射
- 继续增强“更像真断局师”的语言风格

---

## English

**xuanji-decision** is an open-source skill for agent workflows.  
It is **not** a general fortune-telling tool. It is a **mystical fork-resolution plugin** for real project execution.

When an agent reaches a genuine project fork where option A and option B are both plausible, and further rational analysis would only stall progress, xuanji-decision treats the problem as an unresolved **局** and delivers a divination-style ruling using a framework inspired by four classic Chinese fate-analysis texts.

### What problem it solves

Project agents often get stuck on forks like these:

- content-first vs MVP-first
- service-first vs subscription-tool-first
- niche product vs platform structure
- focused audience vs broad audience
- ship now vs polish one more week

These are often not information problems. They are situations where:

> **both sides make sense, but one move still has to be made first.**

xuanji-decision exists to resolve that kind of rational stalemate with something that feels more like a **ruling** than a **consultation**.

### Core design

The skill uses a four-book metaphysical frame:

- **Di Tian Sui (滴天髓)** — read momentum and flow
- **Qiong Tong Bao Jian (穷通宝鉴)** — identify what the current situation lacks most
- **Yuan Hai Zi Ping (渊海子平)** — judge whether a path forms or breaks the project structure
- **San Ming Tong Hui (三命通会)** — judge timing, sequencing, and combinational fit

It does **not** attempt full traditional fate calculation.  
Instead, it translates the judgment habits of these systems into project-fork language:

- where the momentum lies
- what the project lacks right now
- which path better forms the current structure
- whether the time is ripe

The output typically includes:

- a situation name (局名)
- momentum ruling
- balance / adjustment ruling
- structure ruling
- timing ruling
- final judgment
- immediate action order

### Best-fit scenarios

**Best for:**

- product direction forks
- monetization and business-model choices
- execution pace choices
- audience targeting forks
- content-angle choices

**Weak fit:**

- brand tone
- copy style
- pure visual mood

**Not fit for:**

- medical, legal, life-and-death, or major financial decisions
- cases with an obvious objective winner
- cases with severely incomplete facts

### Current status

This repository already has:

- a skill-creator-aligned structure
- validated and packaged `.skill` output
- multiple rounds of manual pressure testing
- mapping files, lexicon files, rejection rules, and test cases

It is still a living v1 and will keep evolving.

### Install

If your environment supports OpenClaw skill packages, use:

- `dist/xuanji-decision.skill`

If you want to inspect or modify the source, see:

- `skill/SKILL.md`
- `skill/references/*`

### Open-source notes

This repository includes:

- the skill definition
- reference lexicons
- mapping rules
- packaged artifact

If you build upon it, attribution is appreciated.

---

## Repository structure

```text
xuanji-decision-open/
├── README.md
├── LICENSE
├── .gitignore
├── skill/
│   ├── SKILL.md
│   └── references/
│       ├── decision-point-mapping.md
│       ├── divination-lexicon.md
│       ├── four-books-mapping.md
│       ├── rejection-rules.md
│       ├── test-cases.md
│       ├── test-report-v1.md
│       └── workflow-and-prompt.md
└── dist/
    └── xuanji-decision.skill
```
