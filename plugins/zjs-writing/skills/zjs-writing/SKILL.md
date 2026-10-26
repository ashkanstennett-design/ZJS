---
name: zjs-writing
description: "中英文科研与专业写作、润色、压缩和审稿回复。以 Kiterlin anti-defensive-writing 为底，删减冗余、自我辩解和层层保留，保留数据、术语、技术条件及证据强度。Use for drafting or revising papers, abstracts, reports, SOPs and reviewer responses; support faithful translation when requested. 不用于强制改写普通问答，也不承诺通过AI检测。"
license: MIT
metadata:
  version: "1.0.0"
  upstream: "Kiterlin/anti-defensive-writing"
  upstream_commit: "f516147d017a3fe43ae99192cb89d8261b0c8679"
---

# ZJS 中英文写作｜第一版

用具体事实、证据和清楚的推理推进文章。删除没有信息量的防御性表述；让结论强度与证据强度一致。

本版基于 Kiterlin 的中英文规则整理，保留原作者 MIT 许可。完整原规则见 [Kiterlin 底稿](references/kiterlin-rules.md)；来源、版本与边界示例见 [来源与示例](references/source-and-examples.md)。底稿是参考，不覆盖用户本次要求。

## 先确认修改范围

- 适用于论文、摘要、引言、讨论、结论、科研项目报告、技术方案、SOP、审稿回复及其他专业文本的起草与修改。
- 用户只要求润色一段时，改善该段表达和衔接，保留贡献、论证范围与技术含义。整篇重构、改变主线或实验设计只在请求允许时进行。
- 按指定语言和格式输出；未指定时沿用原稿语言。中文指令要求润色英文论文，正文仍用英文；简短说明可用中文。依据中文要点起草英文稿时，按要点写作。要求翻译时忠实翻译，保留否定、条件、证据强度与术语，不借润色改变意思。
- 写稿、润色、压缩和批判性审阅是不同任务。用户要求严格审查时，准确指出有依据的问题；不要以“避免防御”为由隐藏缺陷。纯排版、数据计算、一般问答不强行套本规则。

## 修改决策

先判断一句话的作用，再决定是否删除：

| 作用 | 处理 |
|---|---|
| 道歉、自我贬低、重复免责声明、回应无人提出的质疑 | 不提供事实、范围、逻辑或必要指引时删除 |
| 范围、前置条件、比较条件、禁止事项 | 保留或等义写得更直接，不能把有条件结论改成无条件动作 |
| 证据的不确定性、方法限制、冲突或不利结果 | 保留实质含义，明确影响；限制与主张分开会误导时就近说明 |
| 必要概念区分、技术对比、真实研究目的 | 保留，避免机械禁用转折或否定句 |

1. 找到这段的主要信息：研究了什么、比较了什么、发现了什么、下一步要做什么。
2. 删除重复铺垫、套话和无信息量的自我评价，缩减“可能—或许—在一定程度上”等叠加限定。
3. 用具体研究范围替换空洞的“不研究什么”。按论证需要组织段落，一段承担一个主要功能；不强制每段同一模板。
4. 与原稿逐项核对事实、数字、单位、条件、否定、证据强度与完成状态，再交付。

## 事实与证据保持一致

- 保留数值、单位、精度、正负号、不等号、时间、样本量、比较基线、实验条件、公式符号与引文归属；不为显得专业擅换术语。明显疑误可以指出，不静默猜改。
- 不补造引用、数据、机制、显著性、创新性、代表性或“最优”结论。示例中的事实和数字不能移入用户正文。
- 区分实验观察、模型假设、拟合、预测与工程建议；区分已完成、进行中和计划。数值计算跑通不等于实验或现场验证。
- “初步”“可能”“提示”“suggests”“may”符合证据时保留；相关性不能改成因果关系。证据只支持局部范围就缩小结论，完全不支持就撤回或另列待核实项。
- 必要限定可以出现在摘要、贡献段落或结论中；是否保留取决于删除后会不会误导，而非位置禁令。重复的同一限定可合并。

## 科研叙事与不利结果

结构调整在授权范围内时，围绕问题、缺口、贡献、证据与意义组织文字。贡献可以是新发现、新能力、机制解释、资源或有证据的效率收益，无需宣称所有指标领先。研究过程本身重要时保留过程顺序。

每项实验说明它检验的问题，例如有效性、机制、比较条件、适用范围或替代解释。重复展示可合并；影响核心结论或解释的不利证据必须保留，不能为了回避结果更换评价标准或重新定义成功。

指标有得有失时同时写清比较条件、收益与代价；两方面都有证据才称“权衡”。原因不明就不编解释。缺少实验时指出具体哪项主张因此缺少依据，不追加一串假想审稿质疑。

方法与结果保留复现所需信息。讨论说明意义、边界和未解决问题；结论回到已有支持的发现，不引入新成果或无关局限清单。阶段汇报如实写未完成项与下一步，不套用“只展示优势”的叙事。

## 中文表达与技术方案

- 用“做了什么、结果是什么、条件是什么”替换“仅仅做了初步尝试”“只能提供有限参考”等空洞自评；确属初步结果时保留这一状态。
- 简化“进行……的测量”等冗余动词。测量、表征、标定、拟合、校准等按实际操作区分，不用更华丽的词替代原操作。
- “值得注意的是”“需要澄清的是”“不是X而是Y”等表达逐句判断，没有内容作用时删除；真实区分、禁止和前提不能删。
- SOP 保留步骤顺序、前置条件、阈值、范围、停止条件和不可互换的要求。去掉说教语气后，原有禁止事项仍须表达清楚。原文条件不明时指出缺失，不自行补值。
- 沿用专业、直接、连贯的语气；不新增口号、泛泛拔高、机械总结或密集小标题。列表用于实际并列信息，不强制把段落拆碎。

## English editing

- Lead with the paragraph's point and support it with the supplied evidence. Preserve disciplinary voice and technical terminology.
- Replace stacked hedges with one expression calibrated to the evidence. Keep genuine uncertainty, scope conditions, negation and material limitations.
- Prefer concrete verbs and positive scope. Use contrast when it carries a necessary distinction; do not impose a blanket phrase ban.
- Preserve numbers, comparators, citations, causal status and completed-versus-proposed work. Do not turn an association into a mechanism or a pilot result into validation.
- Avoid stock contribution templates and promotional claims. When translating, preserve the meaning and strength of the source rather than making it sound more successful.

## 审稿回复与交付

回复实际意见：先回应问题，再写已有证据、澄清或具体修改。有效意见简短承认；有依据的不同意见明确说明。没有完成的分析只能写成计划；没有提供的页码、行号与新增实验不能编造。

默认直接交付修改后的正文，保留用户要求的格式。用户要求“只给正文”就不附说明。仅在实质改动、事实疑误或关键证据缺口影响使用时，另加短说明；不附例行免责声明、检查清单或假想反对意见。不能保证通过任何 AI 检测。
