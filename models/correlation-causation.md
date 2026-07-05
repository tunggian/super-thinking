---
name: super-thinking/correlation-causation
description: |
  当用户根据两个事件的先后或同时发生推断因果关系时，用此模型提醒区分相关性与因果性，警惕混杂因素和虚假相关。
source_book: "Super Thinking: The Big Book of Mental Models" by Gabriel Weinberg & Lauren McCann (2019)
source_chapter: Chapter 5 - Lies, Damned Lies, and Statistics
tags: [statistics, critical-thinking, bias, data-analysis, causation]
scenarios:
  - "你说'我们换了CEO后业绩就起来了'——检验：是CEO导致的还是只是时间巧合？还有哪些同期变化"
  - "同事说'我发现穿红袜子的日子代码bug最少'——轻松辨别：这是随机巧合的虚假相关还是真的有因果"
  - "看到报告说'每天喝咖啡的人心脏病风险更低'就决定多喝咖啡——先问：有没有混杂因素（如喝咖啡的人普遍生活更规律）"
  - "做A/B测试后转化率提升了就归因于改动——追问：样本量够吗？排除了季节性因素吗？有对照组吗"
  - "公司觉得'搞了团建后士气就高了'——反问：团建之前士气是不是已经在自然恢复？可能是均值回归"
match_keywords: "相关|因果|因为|导致|数据|关系|有关联|关联|相关性|不等于"
priority: 5
---

# Correlation ≠ Causation (相关不等于因果)

## R — 原文 (Reading)
> "Just because two events happened in succession, or are correlated, doesn't mean that the first actually caused the second."

## I — 方法论骨架 (Interpretation)
"相关性不等于因果性"是统计学中最基本也最常被忽视的原则。两个变量同时变化（相关）不意味着一个导致了另一个（因果）。可能的替代解释包括：

1. **混杂因素**（Confounding Factor）：第三个隐藏变量同时影响两者。书中举例：打了流感疫苗的人出现感冒症状→他们归咎于疫苗。真相是：冬季感冒高发，疫苗和普通感冒之间是共变关系，因果方向是"季节因素→两者都容易出现"。

2. **随机巧合**：在大数据时代，总会有一些看似显著但纯属偶然的相关性。书中引用了一个滑稽例子：奶酪消费量和被床单缠住窒息死亡人数之间存在"相关"——显然纯属巧合。

3. **因果方向反转**：有时是结果导致原因，而非原因导致结果。

要建立因果结论，需要设计良好的随机对照实验（Randomized Controlled Experiment）或A/B测试来排除混杂因素。

## A1 — 书中的应用 (Past Application)
1. 流感疫苗"导致"感冒：冬季（混杂因素）同时增加注射疫苗和感染普通感冒的概率
2. 奶酪消费与床单窒息死亡的虚假相关——纯属随机巧合
3. Lauren的Raspberry Snapple"治愈"感冒：巧合的自然恢复被误解为因果关系

## A2 — 触发场景 (Future Trigger) ★
1. 用户说"A导致B"但只基于"A之后发生了B"的个人经验
2. 用户引用某研究发现"X与Y相关"来论证"X导致Y"

语言信号: "自从...就...", "肯定是因为", "相关性显示", "数据证明"

## E — 可执行步骤 (Execution)
1. **问"有没有第三个变量"** - 寻找可能同时影响两者的混杂因素
2. **检查实验设计** - 结论是否来自随机对照实验？如果不是，只是观察数据，则无法确定因果关系
3. **警惕"方向性问题"** - 即使在相关关系中，因果方向也可能相反

## B — 边界 (Boundary) ★
- 相关性是发现因果关系的重要线索——不应完全忽略，而应作为生成假设的起点
- 在无法做实验的领域（如宏观经济学），需要多种相关证据和机制解释来推断因果
- 不要因为"相关≠因果"就否定所有统计发现——好的实验设计在控制混杂因素后可以提供因果证据
