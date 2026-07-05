---
name: super-thinking/expected-value
description: |
  When comparing probabilistic outcomes—multiply each possible payoff by its probability and sum them up to find the average expected result.
source_book: "Super Thinking: The Big Book of Mental Models" by Gabriel Weinberg & Lauren McCann (2019)
source_chapter: Chapter 6 - Decisions, Decisions
tags: [decision-making, probability, quantitative-analysis, risk]
scenarios:
  - 你在评估一个投资机会，有60%概率翻倍、40%概率亏损一半，你不确定这个"赌注"是否值得参与——需要计算预期值而非凭直觉判断
  - 你的团队在决定是否启动一个新项目，项目成功概率不高但回报巨大，你需要一个量化框架来辅助而非替代判断
  - 你在比较两种营销策略：A策略确定带来10万收入，B策略有30%概率带来50万收入但70%概率颗粒无收——直观判断不敢选B，但预期值可能指向相反结论
  - 你在做职业生涯规划，稳定的大厂岗位 vs 加入早期创业公司获得期权，你需要计算不同路径在多次"平行人生"中的平均回报
  - 你在设计游戏抽卡机制的奖励概率，需要确保玩家的预期获得在心理上既不会过于失望也不会过于容易
match_keywords: "期望值|预期|预期价值|概率计算|数学期望|平均结果|量化|期望收益|估值"
priority: 4
---

# Expected Value

## R — 原文 (Reading)
> You can now use your probability estimates to get an expected value for each contractor, by multiplying through each potential outcome's probability with its cost, and then summing them all up. This resulting summed *value* is what you would *expect* to pay on average.

## I — 方法论骨架 (Interpretation)
预期值是你面对不确定结果时的"平均化"思维工具。任何一个决策如果重复足够多次，你的平均收益（或成本）会趋近于预期值。计算方法简单：对每个可能的结果，用其概率乘以对应的价值，然后全部加起来。预期值不代表你会得到恰好那个数字——就像2015年美国母亲平均有2.4个孩子，但没有哪个母亲真有2.4个孩子。这里的关键洞见是：不要在单一结果上赌博，而要在多次决策中通过预期值优势持续获胜。当你不得不在高确定性和高预期值之间选择时，预期值往往指向更优的长期策略，前提是你能承受短期波动。

## A1 — 书中的应用 (Past Application)
- 泳池维修承包商选择：常规承包商确定成本$2,500；新承包商四种可能结果的预期值为$2,212.50，尽管存在$3,000的最坏情况，但预期成本更低，理性选择是新承包商。
- 作者用"多次运行"的思维解释：如果这个场景可以重复100次，选新承包商平均支付$2,212.50，一半时间只付$2,000，另一半时间更多，但整体平均更低。

## A2 — 触发场景 (Future Trigger) ★
1. 在投资决策中评估不同资产的风险与回报——预期收益率 vs 波动性
2. 选择营销策略时，需要权衡确定的小收益和不确定的大收益
3. 在做职业选择时，比较稳定收入的岗位与有期权潜力的创业机会

语言信号: "平均来看...", "长远而言...", "这个赌注值不值..."

## E — 可执行步骤 (Execution)
1. **列出所有可能的结果** - 穷举每个选项下可能发生的所有不同情形
2. **估计每种结果的概率和收益/成本** - 概率总和必须为100%，价值用统一的度量单位（金钱或效用）
3. **计算并比较** - 用 ∑(概率 × 价值) 计算每个选项的预期值，选择预期值最优的选项；同时用敏感性分析检查概率变化对结果的影响

## B — 边界 (Boundary) ★
- 预期值适用于可重复的决策场景（如投资组合管理），但不适用于"一生一次"的高风险决策
- 如果最坏结果会导致破产或不可逆损失，不能只看预期值——必须加入风险规避的效用调整
- 概率估计本身的质量决定了预期值的可靠性，需要警惕过度乐观偏差
- 在肥尾分布中（黑天鹅事件），极端结果的概率被低估，预期值会因此失真
