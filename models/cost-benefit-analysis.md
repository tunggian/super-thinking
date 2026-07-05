---
name: super-thinking/cost-benefit-analysis
description: |
  Upgrade a pro-con list by assigning dollar values to costs and benefits over time, then discount future values to today's dollars to compare options quantitatively.
source_book: "Super Thinking: The Big Book of Mental Models" by Gabriel Weinberg & Lauren McCann (2019)
source_chapter: Chapter 6 - Decisions, Decisions
tags: [decision-making, quantitative-analysis, finance, evaluation]
scenarios:
  - 你在纠结是否要读一个MBA学位，学费和时间投入巨大但毕业后薪资提升不确定，你需要量化比较一辈子时间尺度的净收益
  - 公司有两个技术方案可选：方案A初期投入低但维护成本高，方案B初期投入高但后续节省人力——你需要用折现率比较两者的净现值
  - 你在考虑是否卖掉现在的房子换一套更大的，需要把首付、月供、装修、税费和未来增值全部折算到今天来比较净收益
  - 你在评估一个企业级SaaS软件的采购决策，不仅要看许可费，还要算培训成本、迁移成本、员工学习曲线带来的隐性效率损耗
  - 团队在决定做不做技术债务偿还专项季度——不做的话维护成本逐年上升，做的话当前业务交付受影响，你需要量化两边的现金流
match_keywords: "成本效益|利弊|得失|划算|值得|投入产出|ROI|成本分析|权衡|性价比"
priority: 4
---

# Cost-Benefit Analysis

## R — 原文 (Reading)
> This powerful mental model helps you more systematically and quantitatively *analyze* the *benefits* (pros) and *costs* (cons) across an array of options. ... When writing down costs and benefits, you will find that some are intangible. ... you still want to assign dollar values to them.

## I — 方法论骨架 (Interpretation)
成本效益分析是利弊清单（pro-con list）的量化升级版。从给每个条目打分(−10到+10) 开始，逐步演进到赋金钱价值、按时间线排列、用折现率计算净现值。核心操作是：把每个选项在未来各年的成本和收益列出，用折现率将所有未来价值折算为"今天的美元"，然后加总得到净收益。正净收益意味着该选项优于现状。无形的成本（如焦虑、时间）和收益（如不用跟房东打交道）也要赋金钱值——虽然感觉随意，但比你隐式地判断要好。敏感性分析是关键伴侣工具，用来检验折现率等参数对结论的影响程度。

## A1 — 书中的应用 (Past Application)
- 买房决策：列出首付、月供、维修、税费等成本的时间线，以及出售时的预期收益，用折现率计算净现值来判断是否值得。
- 债券投资分析：$50,000投资，10年后回报$100,000，在6%折现率下净现值为$5,839，净收益为正。但如果折现率超过8%，净收益变为负数。

## A2 — 触发场景 (Future Trigger) ★
1. 评估是否应该换工作——比较新工作的收益流和当前工作加上转换成本
2. 决策是否回学校深造——学费和收入损失 vs 毕业后增加的终身收入
3. 选择不同的项目方案——将每个方案的预期成本和收益按年份排列，用折现率比较净现值

语言信号: "值不值得...", "长期来看...", "投入产出比...", "ROI..."

## E — 可执行步骤 (Execution)
1. **量化所有条目** - 将利弊清单的每一项赋予金钱价值（或从打分 −10到+10 的权重开始）
2. **按时间线排列** - 用电子表格列出每年（Year 0, 1, 2...）的成本和收益
3. **折现并求和** - 选择适当的折现率，用 NPV 公式将未来价值折算到今天，加总得到净收益；然后对折现率和关键无形价值做敏感性分析

## B — 边界 (Boundary) ★
- Garbage in, garbage out：如果输入的成本和收益估计严重不准确，分析结果同样不可靠
- 折现率的选择对结论影响巨大——折现率越高，远期收益越被低估，可能不公正地忽视对后代的影响（如气候变化政策）
- 比较不同时间跨度（如6年 vs 10年）的选项时，必须考虑再投资的机会
- 成本效益分析不适合理性评估人际关系的价值或不可量化的道德决策
