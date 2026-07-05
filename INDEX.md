# Super Thinking — 问题·情景驱动路由

> 来源: 《Super Thinking: The Big Book of Mental Models》(2019)
> 路由方式: **情景语义匹配** — 将用户的问题/情景与 97 个思维模型的 400+ 个具体问题场景匹配
> 模型总数: 97

---

## 路由算法 (MUST FOLLOW)

```
1. 阅读用户描述的问题或困境
2. 查阅下方的「问题域索引」找到用户问题所属的领域
3. 在该领域内，用语义理解匹配用户情景与模型 scenarios 中的具体场景
4. 选出情景最匹配的 3 个思维模型
   每个模型必须能引用一个匹配到的具体场景
```

**关键原则:**
- 恰好 3 个模型，覆盖不同角度（分析现状 + 评估风险 + 指导行动）
- 必须引用匹配到的具体场景说明为什么选这个模型

---

## 问题域索引

### 我该怎么做这个决定？

| 你面临的处境 | 最适合的思维模型 |
|---|---|
| 有几个选项，各有不同的风险和收益，不知道该怎么比较 | decision-tree, expected-value, cost-benefit-analysis |
| 这个决定后果太严重，做错了就回不来了 | de-risking, reversible-decisions, preserving-optionality |
| 太多选择了，选得头疼 | hicks-law, paradox-of-choice, decision-fatigue |
| 做了一个决定后总后悔，觉得另一个更好 | sunk-cost, loss-aversion, hindsight-bias |
| 明明知道现在的情况不对，但就是走不出来 | sunk-cost, opportunity-cost, boiling-frog |
| 做决策时总是被最近的新闻或经历影响 | availability-bias, anchoring, framing |
| 团队做决策，每次开会都一致通过但心里觉得不对劲 | groupthink, devils-advocate, dri |
| 要考虑未来不确定性的重大决策 | scenario-analysis, black-swan, bayes-theorem |
| 不知道该不该放弃现在的，去尝试新的 | opportunity-cost, reversible-decisions, mvp |
| 总是追求最优方案，结果一直没法开始 | perfect-is-enemy-of-good, local-global-optimum, mvp |

### 我的思考方式出问题了吗？

| 你面临的处境 | 最适合的思维模型 |
|---|---|
| 总是用老办法解决新问题，效果不好 | maslows-hammer, first-principles, paradigm-shift |
| 看问题容易走极端，非黑即白 | thinking-gray, inversion, third-story |
| 看到的信息让我觉得世界很糟糕 | availability-bias, framing, news-illusion |
| 别人做了一件对我不利的事，我立刻觉得他故意的 | hanlons-razor, fundamental-attribution-error, mri |
| 事后觉得"我早就知道会这样" | hindsight-bias, counterfactual |
| 很多问题找不到真正的原因 | root-cause, five-whys, proximate-root |
| 观点和别人冲突，不知道谁对 | confirmation-bias, cognitive-dissonance, ockhams-razor |
| 被数据/统计忽悠了但说不出哪里不对 | correlation-causation, survivorship-bias, regression-to-mean |

### 系统/组织/政策出了问题

| 你面临的处境 | 最适合的思维模型 |
|---|---|
| 设计了一个考核制度，结果大家钻空子 | goodharts-law, perverse-incentives, cobra-effect |
| 公共资源（代码质量、预算、时间）被不断消耗 | tragedy-of-commons, free-rider, externalities |
| 改了一个地方，其他地方突然崩了 | systems-thinking, cascading-failure |
| 事情正在慢慢变糟，但没人注意到 | boiling-frog, tyranny-small-decisions, short-termism |
| 组织陷入了一个不好的模式走不出来 | path-dependence, inertia, entropy |
| 好心办坏事，原本的好政策产生了反面效果 | cobra-effect, perverse-incentives, moral-hazard |
| 委托别人做的事总是和预期不一样 | principal-agent, asymmetric-info, moral-hazard |
| 只想快速解决眼前问题，顾不上长远的 | short-termism, technical-debt, preserving-optionality |

### 竞争/谈判/冲突

| 你面临的处境 | 最适合的思维模型 |
|---|---|
| 和竞争对手/合作伙伴陷入了互相消耗的局面 | prisoners-dilemma, game-theory, nash-equilibrium |
| 对方不断得寸进尺，不知道该怎么回应 | tit-for-tat, deterrence, red-line |
| 想要说服别人接受我的方案 | influence-principles, framing, reciprocity |
| 对方信息比我多，处于劣势 | asymmetric-info, game-theory |
| 双方都不敢先行动，僵在那里 | mad, nash-equilibrium, deterrence |
| 如何快速应对变化的环境 | ooda-loop, scenario-analysis |
| 要不要打价格战/军备竞赛 | game-theory, prisoners-dilemma, war-of-attrition |

### 团队/人才/管理

| 你面临的处境 | 最适合的思维模型 |
|---|---|
| 好员工被提拔后反而做不好了 | peter-principle, dunning-kruger |
| 团队有人觉得自己不配这个位置 | impostor-syndrome, pygmalion-effect, growth-mindset |
| 培训/学习效果总是不好 | deliberate-practice, growth-mindset, spacing-effect |
| 项目出了问题没人认领责任 | dri, bystander-effect, power-vacuum |
| 给反馈总是让对方不舒服或者没效果 | radical-candor, pygmalion-effect |
| 重要人才想离职/招不到对的人 | joys-law, maslows-hierarchy, dunbars-number |
| 会议太多，没时间真正做事 | maker-manager, deep-work, eisenhower-matrix |
| 团队越来越大后效率反而下降 | dunbars-number, social-loafing |

### 创业/产品/市场

| 你面临的处境 | 最适合的思维模型 |
|---|---|
| 有一个想法，不确定是否该全力投入 | product-market-fit, mvp, customer-development |
| 产品做出来了但没人用 | jobs-to-be-done, product-market-fit, crossing-the-chasm |
| 做了一个功能没人用，但又不舍得砍 | sunk-cost, opportunity-cost |
| 和巨头竞争，各方面都不如对方 | disruptive-innovation, guerrilla-warfare, secrets |
| 想建立长期竞争壁垒 | moat, network-effects, lock-in |
| 早期用户很喜欢但始终长不大 | crossing-the-chasm, s-curve, critical-mass |
| 要不要率先进入一个市场 | first-mover, beachhead, ooda-loop |
| 用户增长突然停滞了 | s-curve, tipping-point, critical-mass |
| 该不该转型/退出 | pivot, exit-strategy, opportunity-cost |
| 看到别人的产品火了，想抄一个 | survivorship-bias, first-principles, secrets |

### 时间/效率/习惯

| 你面临的处境 | 最适合的思维模型 |
|---|---|
| 每天忙得要死但重要的事一直没推进 | eisenhower-matrix, pareto, deep-work |
| 事情永远做不完，越来越多 | leverage, pareto, opportunity-cost |
| 总是高估自己能完成的事 | planning-fallacy, parkinsons-law |
| 想养成一个好习惯但总是三天打鱼 | activation-energy, flywheel, commitment-device |
| 做一件事总是迟迟无法开始 | activation-energy, perfect-is-enemy-of-good |
| 想做一件事但"万事开头难" | activation-energy, mvp, de-risking |
| 投入了很多时间精力但产出不多 | leverage, pareto, opportunity-cost |

### 变革/增长/自然规律

| 你面临的处境 | 最适合的思维模型 |
|---|---|
| 推动组织变革，阻力巨大 | inertia, activation-energy, paradigm-shift |
| 想建立一个自我驱动的增长循环 | flywheel, critical-mass, network-effects |
| 势头很好，突然就停滞了 | s-curve, tipping-point, entropy |
| 一个趋势什么时候会爆发/结束 | tipping-point, critical-mass, s-curve |
| 事情已经不可逆地走向糟糕的方向 | entropy, path-dependence, boiling-frog |
| 怎么能从混乱中获益 | antifragile, ooda-loop |

---

## 完整模型列表（带典型问题场景）

| # | 模型 | 典型问题场景 |
|---|---|---|
| 1 | first-principles | "一直都是这么做的"——你想从零重新思考但不知从何开始 |
| 2 | inversion | 正着想不出答案，试试反过来——不做哪些事能避免最坏结果？ |
| 3 | ockhams-razor | 面对一堆互相矛盾的解释，最简单的往往最可能是对的 |
| 4 | confirmation-bias | 你发现自己在选择性收集证据支持已有结论 |
| 5 | thinking-gray | 你或团队陷入了"全对"或"全错"的二元对立 |
| 6 | hanlons-razor | 别人做了对你不利的事，你的第一反应是对方故意的 |
| 7 | third-story | 你和某人产生了分歧，需要跳出自己的立场理解问题 |
| 8 | mri | 沟通出现误解，你需要给对方的言行一个最善意的解释 |
| 9 | framing | 同样的信息换一种说法就让你做出完全不同的判断 |
| 10 | anchoring | 谈判或估价时被第一个出现的数字牢牢套住 |
| 11 | availability-bias | 最近的新闻/事件让你高估了某些风险、低估了其他 |
| 12 | paradigm-shift | 旧的方法论在新的环境下完全失效了 |
| 13 | maslows-hammer | 你发现自己或团队永远只用一种方法解决所有问题 |
| 14 | cognitive-dissonance | 做了一个决定后开始不断找理由说服自己是对的 |
| 15 | fundamental-attribution-error | 别人失败是能力问题，自己失败是环境不好 |
| 16 | hindsight-bias | "我早就知道会这样"——但当时其实你没有 |
| 17 | murphys-law | 你觉得"应该不会出问题吧"，结果真的出了问题 |
| 18 | root-cause | 反复解决同一个问题的"症状"但从没找到病根 |
| 19 | five-whys | 想知道一个问题的根本原因，不是表面原因 |
| 20 | de-risking | 一个重大决定让你害怕，想在投入全部资源前先验证 |
| 21 | mvp | 有一个想法但不想花太多时间精力去验证 |
| 22 | perfect-is-enemy-of-good | 因为一直在追求完美，三个月后还没有可以交付的东西 |
| 23 | decision-tree | 有多个方案各有概率性结果，需要系统比较 |
| 24 | expected-value | 做决策时只看可能的收益，没考虑每种结果的发生概率 |
| 25 | cost-benefit-analysis | 在两个选项之间反复比较但始终没法下决心 |
| 26 | opportunity-cost | 选了A就得放弃B，但B似乎也很好，怎么选？ |
| 27 | sunk-cost | 明知某件事继续下去没有意义，但不舍得已经投入的 |
| 28 | loss-aversion | 面对可能的损失时变得过于保守，错过了机会 |
| 29 | reversible-decisions | 不确定这个决定做错了还能不能回头 |
| 30 | scenario-analysis | 未来有好几种可能的发展方向，每种都要准备 |
| 31 | systems-thinking | 改了一个地方却发现其他地方连锁出了问题 |
| 32 | black-swan | 大家都在说"不可能"，但万一发生了就是灾难 |
| 33 | groupthink | 会上没人反对，但你知道不是所有人都真正同意 |
| 34 | devils-advocate | 大家很快就达成了一致，你需要有人来挑战一下 |
| 35 | local-global-optimum | 你是不是被困在了一个"还行"但不是最好的方案里？ |
| 36 | hicks-law | 选项太多了导致迟迟做不了决定 |
| 37 | paradox-of-choice | 选项越多反而越焦虑，选完还后悔 |
| 38 | tragedy-of-commons | 公共的东西大家都在用，没人维护 |
| 39 | free-rider | 小组里有人什么都没做但享受了集体成果 |
| 40 | externalities | 你的决策影响到了不相干的第三方 |
| 41 | goodharts-law | 一旦指标变成了考核目标，它就不再是好的衡量标准 |
| 42 | cobra-effect | 本想用奖励解决问题，结果让问题更严重了 |
| 43 | perverse-incentives | 激励制度设计出来后人们的行为完全偏离了初衷 |
| 44 | boiling-frog | 事情正在慢慢变糟，但因为变化太慢没人拉警报 |
| 45 | path-dependence | 今天的困境是一系列过去的小决定累积锁死的 |
| 46 | short-termism | 为了眼前的利益牺牲了长远的未来 |
| 47 | technical-debt | 为了赶进度做了很多临时方案，现在系统快撑不住了 |
| 48 | preserving-optionality | 你现在做的一个决定可能会锁死未来的很多可能性 |
| 49 | principal-agent | 你委托别人做的事，对方的利益和你不一致 |
| 50 | moral-hazard | 反正不是你承担后果，所以你没有动力控制风险 |
| 51 | asymmetric-info | 交易/合作中对方掌握了你不知道的关键信息 |
| 52 | game-theory | 你的最佳策略取决于对手怎么行动 |
| 53 | prisoners-dilemma | 每个人选对自己最有利的，结果大家的情况都更差 |
| 54 | nash-equilibrium | 竞争或博弈到了一个彼此都不敢先动的僵局 |
| 55 | tit-for-tat | 对方怎么对你，你就怎么对他——但这样对吗？ |
| 56 | influence-principles | 你需要说服一个很难被说服的人 |
| 57 | deterrence | 你需要让对方因为害怕后果而不敢做某件事 |
| 58 | mad | 对抗双方都有能力摧毁对方，谁也不敢轻举妄动 |
| 59 | ooda-loop | 环境变化太快，你每慢一步就落后一步 |
| 60 | deliberate-practice | 花了很多时间练习/学习但进步不大 |
| 61 | growth-mindset | 你或你的团队成员觉得"我就是做不好这个" |
| 62 | pygmalion-effect | 你对某个下属/孩子的期望影响了他的实际表现 |
| 63 | peter-principle | 最好的员工被提拔后反而表现不佳 |
| 64 | dunning-kruger | 刚学了一点就觉得自己很懂，或者学了很多反而觉得自己不够 |
| 65 | impostor-syndrome | 明明做得很好却总觉得自己配不上、怕被拆穿 |
| 66 | dri | 出了问题大家都觉得"不关我的事" |
| 67 | radical-candor | 有话想直说又怕伤了关系，不说出来又憋着难受 |
| 68 | maslows-hierarchy | 你想激励他人，但不知道他们当前最需要的是什么 |
| 69 | dunbars-number | 团队超过一定规模后沟通效率急剧下降 |
| 70 | joys-law | 最优秀的人才大都不在你的公司 |
| 71 | maker-manager | 你一整天被会议填满，真正需要专注的工作只能晚上做 |
| 72 | moat | 你的产品/个人优势很容易被竞争对手复制 |
| 73 | product-market-fit | 产品做出来了但没人用，或者用了就不来了 |
| 74 | secrets | 你想找到一个被大多数人忽略的重要洞察 |
| 75 | first-mover | 你不知道该不该第一个进入一个新兴市场 |
| 76 | disruptive-innovation | 行业巨头看不上你的小市场，但这里可能是未来 |
| 77 | crossing-the-chasm | 早期用户很喜欢你的产品，但没办法扩展到主流用户 |
| 78 | jobs-to-be-done | 用户说想要的功能做出来他们却不用 |
| 79 | s-curve | 增长/学习到了一个平台期，不知道下一步什么时候来 |
| 80 | network-effects | 想建立一个用户越多产品越好的正向循环 |
| 81 | exit-strategy | 你已经在一个局面里太久，需要一个体面的退场方案 |
| 82 | correlation-causation | 数据显示A和B高度相关，你就断定A导致了B |
| 83 | survivorship-bias | 你参考的"成功经验"都是幸存者写的 |
| 84 | bayes-theorem | 获得了新信息，需要用它来更新原来的判断 |
| 85 | regression-to-mean | 一次极端的好/坏表现后必然回归正常 |
| 86 | inertia | 想推动变革但感觉整个系统都在反对你 |
| 87 | flywheel | 想设计一个每转一圈就自动加速的增长引擎 |
| 88 | critical-mass | 在到达某个关键规模之前一切投入都看不到回报 |
| 89 | tipping-point | 想知道一个小变化的临界点在哪里，过了就会不可逆 |
| 90 | entropy | 不持续投入精力维护，任何系统都会自然走向混乱 |
| 91 | activation-energy | 万事开头难——启动一件事需要的能量远比维持它大 |
| 92 | eisenhower-matrix | 总是被紧急的事推着走，重要的事永远在排队 |
| 93 | pareto | 80% 的成果来自 20% 的投入——但不是每个人都找到了那 20% |
| 94 | leverage | 投入了同样的努力，产出却远不如那些"会借力"的人 |
| 95 | deep-work | 想进入心流状态但总是被各种事情打断 |
| 96 | antifragile | 别人在危机中倒下，你想成为那个在混乱中反而变强的人 |
| 97 | tyranny-small-decisions | 每一个单独的小决定都没问题，积累起来却导致了灾难 |

---

## 情景路由示例

### 用户说: "我在大厂干了 5 年，前同事拉我加入天使轮创业，年薪只有现在的三分之一但给股份，我很纠结"

匹配分析:
1. 多个方案各有概率性结果 → **decision-tree** 场景"换工作、创业方向"
2. 选了A就得放弃B → **opportunity-cost** 场景"跳槽抉择"
3. 重大决定，后果不可逆 → **de-risking** 场景"重大决定让你害怕，想先验证"

### 用户说: "我们公司设了 KPI 后，员工就只做能考核的事，产品质量下降了"

匹配分析:
1. 指标变成考核目标后不再有效 → **goodharts-law** 场景"Bug KPI、客服考核"
2. 激励制度扭曲了行为 → **perverse-incentives** 场景"PR数量、全勤奖"
3. 可能还有代理问题 → **principal-agent** 场景"委托别人做的事，利益不一致"
