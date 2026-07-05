# Super Thinking — 思维模型工具箱 🧠

> **97 个核心思维模型，为 AI 注入结构化思考能力。**
>
> 灵感源自 Charlie Munger（穷查理宝典）的多元思维模型理念，内容基于 Gabriel Weinberg 和 Lauren McCann 的《Super Thinking: The Big Book of Mental Models》（2019）。

## 📖 背景

读《穷查理宝典》收获最大的是两件事：

1. **思维模型** — Munger 说，如果你只有一把锤子，你看什么都像钉子。要解决复杂问题，你需要**跨学科的多元思维模型**（Lollapalooza 效应）。
2. **偏见与误区** — 人类认知天然存在系统性偏差，识别它们就是战胜它们的第一步。

于是我想到：**如果 AI 也能拥有一个"思维模型工具箱"——遇到问题时自动匹配最合适的模型来分析——会怎样？**

于是用 `book-to-skill-master` 这个技能将《Super Thinking》全书的 97 个模型提炼成了这套 AI 可读的技能文件。每个模型包含：

- **R** — 原文精要
- **I** — 方法论骨架
- **A1/A2** — 历史应用 + 未来的触发场景
- **E** — 可执行的操作步骤
- **B** — 边界与限制

## ✨ 功能

当你在 Claude Code 或其他兼容 AI Agent 中遇到需要深度思考的问题时，调用 `/super-thinking`，AI 将：

1. 理解你的问题/困境
2. 从 **97 个模型 × 400+ 场景** 中找到最匹配的 **3 个模型**
3. 用 E（执行）步骤给出结构化、可操作的思路

覆盖的问题域：

| 领域 | 模型数 | 适合做什么 |
|---|---|---|
| 🧠 认知与清晰思考 | 18 | 克服偏见、更清晰地思考 |
| ⚖️ 决策与选择 | 18 | 做重大决策、权衡利弊 |
| 🔧 系统思维与冲突 | 25 | 分析组织问题、处理博弈 |
| 👥 人际与领导力 | 12 | 管理团队、激励他人 |
| 🏢 战略与市场 | 10 | 创业方向、竞争策略 |
| 📊 统计素养 | 4 | 数据解读、避免统计陷阱 |
| 🌿 自然与系统 | 6 | 理解增长、惰性、临界点 |
| ⏱ 生产力 | 4 | 时间管理、深度工作 |

## 🚀 安装

### 前提

- 安装 Claude Code 或其他兼容的 AI Agent 工具
- 确保你的 skills 目录已配置（如 `.agents/skills`、`~/.claude/skills` 或对应工具的 skills 文件夹）

### 方法一：直接安装

```bash
git clone https://github.com/tunggian/super-thinking.git
cp -r super-thinking ~/.agents/skills/
```

### 方法二：符号链接（便于更新）

```bash
git clone https://github.com/tunggian/super-thinking.git ~/super-thinking
ln -s ~/super-thinking ~/.agents/skills/super-thinking
```

### 方法三：直接从 GitHub 安装

```bash
cd ~/.agents/skills
git clone https://github.com/tunggian/super-thinking.git
```

### 验证安装

重启 Claude Code，输入 `/super-thinking`，应该看到 skill 被加载的提示。

## 💡 使用方法

### 快速启动

```
/super-thinking
```

### 提问范例

直接描述你遇到的问题即可。AI 会自动匹配合适的模型：

| 你的问题 | 匹配的模型 |
|---|---|
| "有几个工作机会在衡量，各有优劣，不知道选哪个" | decision-tree, opportunity-cost, de-risking |
| "团队做了个功能没人用，但舍不得砍" | sunk-cost, opportunity-cost |
| "每次开会大家都不说话，但我知道有人有意见" | groupthink, devils-advocate |
| "对手打价格战，跟不跟？" | game-theory, war-of-attrition |
| "每天都在忙，但重要的事一直没推进" | eisenhower-matrix, pareto, deep-work |

### 回答格式示例

```
你的问题属于[领域]，我找到 3 个最相关的思维模型：

**模型 1: [名称]** — 匹配场景: "[引用具体场景]"
- 核心逻辑: ...
- 怎么做: ...

**模型 2: [名称]** — 匹配场景: "[引用具体场景]"
...

**模型 3: [名称]** — 匹配场景: "[引用具体场景]"
...

**综合建议**: ...
```

### 与 Thinking Clearly 结合使用

本仓库还有一个配套技能 [**Thinking Clearly**](https://github.com/tunggian/thinking-clearly)，聚焦于认知偏见和思维误区的自我觉察。两者搭配：

- `/super-thinking` → 找思维模型来解决问题
- `/thinking-clearly` → 识别自己是否陷入了某种认知偏见

## 📁 目录结构

```
super-thinking/
├── README.md              # 本文件
├── SKILL.md               # 技能定义（核心工作流 + 触发规则）
├── INDEX.md               # 问题域索引（400+ 场景 → 模型映射）
├── models/                # 97 个思维模型文件
│   ├── first-principles.md
│   ├── inversion.md
│   ├── ockhams-razor.md
│   ├── confirmation-bias.md
│   ├── thinking-gray.md
│   ├── ... (共 97 个)
└── LICENSE                # MIT
```

## 🗺 完整模型清单

### A. 认知与清晰思考（18）

| # | 模型 | 一句话 |
|---|---|---|
| 1 | First Principles（第一性原理） | 抛开假设，从基础事实重建 |
| 2 | Inversion（逆思考） | 反过来想，避开最坏结果 |
| 3 | Occam's Razor（奥卡姆剃刀） | 最简单的往往最正确 |
| 4 | Confirmation Bias（确认偏误） | 你只看到支持自己观点的证据 |
| 5 | Thinking Gray（灰色思维） | 非黑即白是思考的偷懒 |
| 6 | Hanlon's Razor（汉隆剃刀） | 能用愚蠢解释的，别归因于恶意 |
| 7 | Third Story（第三故事） | 跳出自己的视角看冲突 |
| 8 | MRI（最善意的解释） | 给别人一个善意的解释 |
| 9 | Framing（框架效应） | 说法不同，判断完全不同 |
| 10 | Anchoring（锚定效应） | 第一个数字决定一切 |
| 11 | Availability Bias（可得性偏误） | 最近的新闻扭曲了你的判断 |
| 12 | Paradigm Shift（范式转移） | 旧方法失效了 |
| 13 | Maslow's Hammer（马斯洛锤） | 有了锤子看什么都像钉子 |
| 14 | Cognitive Dissonance（认知失调） | 做错事后拼命找理由 |
| 15 | Fundamental Attribution Error（基本归因偏误） | 自己是环境，别人是本质 |
| 16 | Hindsight Bias（事后诸葛偏误） | 我早就知道会这样（其实你并不知道） |
| 17 | Murphy's Law（墨菲定律） | 可能出错的一定会出错 |
| 18 | Root Cause / Five Whys（根因分析 / 5W法） | 连问 5 个为什么 |

### B. 决策与选择（18）

| # | 模型 | 一句话 |
|---|---|---|
| 19 | De-risking（去风险化） | 先验证风险最大的假设 |
| 20 | MVP（最小可行产品） | 用最小代价验证想法 |
| 21 | Perfect is Enemy of Good（完美是好的敌人） | 追求完美等于永远完不成 |
| 22 | Decision Tree（决策树） | 画出所有可能路径 |
| 23 | Expected Value（期望值） | 收益 × 概率 = 真实价值 |
| 24 | Cost-Benefit Analysis（成本收益分析） | 全面衡量，而不是感觉 |
| 25 | Opportunity Cost（机会成本） | 选了 A 的代价是放弃了 B |
| 26 | Sunk Cost（沉没成本） | 已经投入的不应影响未来决策 |
| 27 | Loss Aversion（损失厌恶） | 失去的痛苦大于获得的快乐 |
| 28 | Reversible Decisions（可逆决策） | 这扇门关上还能打开吗？ |
| 29 | Scenario Analysis（情景分析） | 未来有好几种可能 |
| 30 | Systems Thinking（系统思维） | 改一个地方，哪些地方会受影响 |
| 31 | Black Swan（黑天鹅） | 低概率、高冲击的极端事件 |
| 32 | Groupthink（群体思维） | 会上没人反对，但大家未必真的同意 |
| 33 | Devil's Advocate（魔鬼代言人） | 主动找一个反对派 |
| 34 | Local vs Global Optimum（局部最优 vs 全局最优） | 你被困在山顶还是半山腰？ |
| 35 | Hicks Law（希克定律） | 选项越多，决策越慢 |
| 36 | Paradox of Choice（选择的悖论） | 选择越多越焦虑 |

### C. 系统思维与冲突（25）

| # | 模型 | 一句话 |
|---|---|---|
| 37 | Tragedy of the Commons（公地悲剧） | 公共资源被每个人消耗殆尽 |
| 38 | Free Rider（搭便车） | 有人不出力却享受成果 |
| 39 | Externalities（外部性） | 你的决定影响到了不相关的人 |
| 40 | Goodhart's Law（古德哈特定律） | 指标变成目标后就不再有效 |
| 41 | Cobra Effect（眼镜蛇效应） | 好心办了坏事 |
| 42 | Perverse Incentives（扭曲激励） | 激励制度导致行为跑偏 |
| 43 | Boiling Frog（温水煮青蛙） | 变化慢到没人察觉 |
| 44 | Path Dependence（路径依赖） | 过去的小决定锁死了未来的选择 |
| 45 | Short-termism（短期主义） | 眼前的利益 > 长远的未来 |
| 46 | Technical Debt（技术债务） | 赶进度的代价是未来的崩溃 |
| 47 | Preserving Optionality（保留选择权） | 别让今天的决定锁死明天的可能 |
| 48 | Principal-Agent（委托代理问题） | 委托人 vs 代理人，利益不一致 |
| 49 | Moral Hazard（道德风险） | 反正不是我承担后果 |
| 50 | Asymmetric Info（信息不对称） | 你知道的比对方多或少 |
| 51 | Game Theory（博弈论） | 你的最优策略取决于对手怎么动 |
| 52 | Prisoner's Dilemma（囚徒困境） | 各自选最有利的，结果双输 |
| 53 | Nash Equilibrium（纳什均衡） | 谁都不敢先动的僵局 |
| 54 | Tit for Tat（以牙还牙） | 你怎么对我，我就怎么对你 |
| 55 | Red Line（红线） | 告诉对方，越界必有后果 |
| 56 | Deterrence（威慑） | 让对方因为害怕而不敢行动 |
| 57 | MAD（相互确保摧毁） | 双方都有毁灭对方的能力 |
| 58 | OODA Loop（OODA循环） | 比对手更快地观察→定位→决策→行动 |
| 59 | War of Attrition（消耗战） | 看谁先撑不住的持久战 |
| 60 | Guerrilla Warfare（游击战） | 小打小闹，打不过就跑 |
| 61 | Beachhead（滩头阵地） | 先占领一个小市场站稳脚跟 |

### D. 人际与领导力（12）

| # | 模型 | 一句话 |
|---|---|---|
| 62 | Deliberate Practice（刻意练习） | 不是练得多，而是练得对 |
| 63 | Growth Mindset（成长心态） | 能力是可以培养的，不是天生的 |
| 64 | Pygmalion Effect（皮格马利翁效应） | 你对一个人的期望影响了他的表现 |
| 65 | Peter Principle（彼得原理） | 每个人最终被提拔到不胜任的位置 |
| 66 | Dunning-Kruger（邓宁-克鲁格效应） | 越不懂的人越自信 |
| 67 | Impostor Syndrome（冒名顶替综合征） | 明明很好却觉得自己配不上 |
| 68 | DRI（直接责任人） | 问题一定要有最终负责人 |
| 69 | Radical Candor（彻底坦诚） | 关心他人 + 直接挑战 |
| 70 | Maslow's Hierarchy（马斯洛需求层次） | 人最底层的需求是什么？ |
| 71 | Dunbar's Number（邓巴数） | 一个人最多维持 150 个社交关系 |
| 72 | Joy's Law（乔伊定律） | 最优秀的人才不在你公司 |
| 73 | Maker vs Manager（创造者 vs 管理者） | 大块时间 vs 碎片时间 |

### E. 战略与市场（10）

| # | 模型 | 一句话 |
|---|---|---|
| 74 | Moat（护城河） | 你的优势别人多久能复制？ |
| 75 | Product-Market Fit（产品市场契合） | 你的产品是不是用户真正想要的？ |
| 76 | Secrets（秘密） | 你知道但大多数人不知道的真相 |
| 77 | First Mover（先发优势） | 第一个进入市场就一定赢吗？ |
| 78 | Disruptive Innovation（颠覆性创新） | 巨头看不上的小市场可能是未来 |
| 79 | Crossing the Chasm（跨越鸿沟） | 早期用户到主流用户的致命裂缝 |
| 80 | Jobs to Be Done（待办任务） | 用户"雇佣"你的产品完成什么任务？ |
| 81 | S-Curve（S型曲线） | 增长总有平台期 |
| 82 | Network Effects（网络效应） | 每个新用户让产品更好 |
| 83 | Pivot / Exit Strategy（转型 / 退出策略） | 知道什么时候该走 |

### F. 统计素养（4）

| # | 模型 | 一句话 |
|---|---|---|
| 84 | Correlation ≠ Causation（相关≠因果） | A 和 B 相关，不意味着 A 导致 B |
| 85 | Survivorship Bias（幸存者偏差） | 你看到的成功故事都是活下来的 |
| 86 | Bayes' Theorem（贝叶斯定理） | 根据新信息更新你的判断 |
| 87 | Regression to Mean（均值回归） | 极端表现之后必然回归正常 |

### G. 自然与系统（6）

| # | 模型 | 一句话 |
|---|---|---|
| 88 | Inertia（惯性） | 系统抗拒变化 |
| 89 | Flywheel（飞轮） | 每转一圈都在为下一圈蓄力 |
| 90 | Critical Mass（临界质量） | 过了这个点，自持续增长开始 |
| 91 | Tipping Point（引爆点） | 一个小变化引发连锁反应 |
| 92 | Entropy（熵增） | 不维护，一切都会走向混乱 |
| 93 | Antifragile（反脆弱） | 在混乱中变得更强的能力 |

### H. 生产力（4）

| # | 模型 | 一句话 |
|---|---|---|
| 94 | Activation Energy（活化能） | 开始一件事比坚持更难 |
| 95 | Eisenhower Matrix（艾森豪威尔矩阵） | 紧急 vs 重要，四象限 |
| 96 | Pareto Principle（帕累托法则） | 80% 的成果来自 20% 的投入 |
| 97 | Deep Work（深度工作） | 进入心流之前，先移除干扰 |

## 🧩 技术细节

- 每个模型文件使用标准化的 **R-I-A-E-B** 结构
- 通过 **情景语义匹配** 路由：用户描述问题 → 在 400+ 场景中匹配最相似的 3 个模型
- `INDEX.md` 包含 8 个问题域和 400+ 具体场景的语义映射
- 每个模型文件都有 `scenarios` 和 `match_keywords` 用于匹配

## 🧠 姊妹项目：Thinking Clearly

**[Thinking Clearly](https://github.com/tunggian/thinking-clearly)** — 99 个认知偏误避坑工具箱。

基于 Rolf Dobelli 的《The Art of Thinking Clearly》（清醒思考的艺术），与 Super Thinking 形成完美互补：

| | Super Thinking | Thinking Clearly |
|---|---|---|
| 侧重 | **给工具** — 用思维模型分析问题 | **避坑** — 识别认知偏误 |
| 来源 | 《Super Thinking》Gabriel Weinberg | 《The Art of Thinking Clearly》Rolf Dobelli |
| 数量 | 97 个思维模型 | 99 个认知偏误 |
| 回答 | "你应该这样思考" | "你正在犯这个错，这样避免" |

**建议工作流**：
1. `/thinking-clearly` — 先检查自己有没有陷入认知偏误
2. `/super-thinking` — 再找合适的思维模型分析问题

```bash
git clone https://github.com/tunggian/thinking-clearly.git
```

## 📜 许可

MIT License — 你可以自由使用、修改、分享。

## 🙏 致谢

- **Charlie Munger** — 多元思维模型的倡导者
- **Gabriel Weinberg & Lauren McCann** —《Super Thinking》的作者，系统地整理了 97 个思维模型
- **Rolf Dobelli** —《The Art of Thinking Clearly》作者，姊妹项目的思想来源
- **[book-to-skill](https://github.com/apple-ouyang/book-to-skill)** — 将书籍转化为 AI Agent 可执行 Skill 的开源项目