---
name: super-thinking/decision-tree
description: |
  When facing a decision with multiple uncertain outcomes, each with different probabilities—use a decision tree to map branches and calculate expected value.
source_book: "Super Thinking: The Big Book of Mental Models" by Gabriel Weinberg & Lauren McCann (2019)
source_chapter: Chapter 6 - Decisions, Decisions
tags: [decision-making, probability, risk-analysis, quantitative-analysis]
scenarios:
  - 你在几个外包供应商之间做选择，每个供应商的报价、交付周期和延期风险各不相同，你不知道该怎么选
  - 你在考虑是否换工作，新公司给出股权激励方案但估值不确定，你需要比较多个职业路径的预期收益和风险
  - 你的创业团队面临产品方向的抉择——A方向确定但天花板低，B方向不确定但可能爆发，你需要量化比较两条路径
  - 你在做健康保险方案选择，高免赔额低保费 vs 低免赔额高保费，取决于家庭成员的健康状况和不同医疗支出的概率分布
  - 公司有多个营销渠道可选，每个渠道的转化率、成本和风险差异很大，你需要找到预期ROI最优的渠道组合
match_keywords: "决策树|分支|概率|路径|选项|各种可能|结果|选择困难|多个方案|分支分析|量化决策|该不该|要不要|怎么办|怎么选|比较方案"
priority: 5
---

# Decision Tree

## R — 原文 (Reading)
> It's a diagram that looks like a *tree* (drawn on its side), and helps you analyze *decisions* with uncertain outcomes. The branches (often denoted by squares) are decision points and the leaves represent different possible outcomes.

## I — 方法论骨架 (Interpretation)
决策树是一种将复杂决策可视化的工具。你把每个选项画成一个分支（方框为决策点，圆圈为机会点），然后为每个可能的结果标注其概率和代价。在树的末端（叶子），列出该路径的最终成本或收益。将每条路径的概率乘以对应代价并求和，就得到了该选项的预期值。决策树迫使你把不确定性显式化，把模糊的"感觉"转化为可计算的结构。它特别适用于比较多个方案，即使其中某些方案有不确定的中间结果。当选项的成本和收益不清晰，或涉及概率性结果时，决策树比简单利弊清单要强大得多。

## A1 — 书中的应用 (Past Application)
- 作者用修泳池设备的例子：一个熟悉的承包商报价$2,500（确定结果），一个新承包商报价$2,000但有50%概率延期或超支（分别有25%/20%/5%的概率导致$250/$500/$1,000额外费用）。通过决策树计算预期值，新承包商的预期成本为$2,212.50，虽然最高可能达到$3,000，但预期值更低。
- 选择健康保险方案时，高免赔额低保费 vs 低免赔额高保费，取决于预期医疗需求和能否承担低概率的高额支出。

## A2 — 触发场景 (Future Trigger) ★
1. 需要在多个供应商/方案之间做选择，且每个方案都有不同的交付风险
2. 评估一个项目的多种执行路径，每条路径有不同的成功概率和资源消耗
3. 做个人职业选择时，不同方向有不同的收入概率、成长概率和满意度概率

语言信号: "如果顺利的话...但万一...", "有X%的把握", "最坏情况与最好情况差距很大"

## E — 可执行步骤 (Execution)
1. **列出所有选项** - 将每个可行的选择画为决策树的第一层分支（方框）
2. **为每个选项展开可能的结果** - 用圆圈表示机会点，列出每种结果的概率和代价/收益，确保每个机会点的概率之和为100%
3. **计算预期值并加入效用** - 将每条路径的代价×概率求和；如果涉及主观感受（如焦虑、时间机会成本），将无形因素转化为效用值加入叶子节点

## B — 边界 (Boundary) ★
- 当所有选项的结果都确定时，不需要决策树，直接比较即可
- 概率估计的准确性是关键——如果概率靠猜测，结果将不可靠（garbage in, garbage out）
- 只考虑预期值可能忽略极端风险的冲击——如果某个低概率结果会导致破产，应大幅提高其效用代价
- 不适用于选项之间有复杂互动反馈的系统性问题，需要先用系统思维建模
