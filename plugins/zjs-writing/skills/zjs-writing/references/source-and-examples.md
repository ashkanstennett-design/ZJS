# 来源与边界示例

## 来源

- 本版：`zjs-writing` v1.0.0，面向 ZJS 的中英文科研与专业写作。
- 基础仓库：https://github.com/Kiterlin/anti-defensive-writing
- 固定提交：`f516147d017a3fe43ae99192cb89d8261b0c8679`。
- 原始入口：https://github.com/Kiterlin/anti-defensive-writing/blob/f516147d017a3fe43ae99192cb89d8261b0c8679/SKILL.md
- 原始许可：https://github.com/Kiterlin/anti-defensive-writing/blob/f516147d017a3fe43ae99192cb89d8261b0c8679/LICENSE
- [原始中英文规则](kiterlin-rules.md)与根目录 `LICENSE` 保留原文。个人整理合并了重复规则，并明确了修改范围、技术保真、翻译、批判性审阅及交付方式。此为独立个人衍生版本，不冒充上游官方版本。
- 不自动追踪上游、不联网执行安装器、不要求额外 API 或外部服务；更新时核对新版本并保留个人差异。

下列数据全部是构造的教学示例，不是 ZJS 已完成的研究结果。

## 1. 去掉自我评价，保留比较

输入：同条件下，基线准确率90%、延迟100 ms，新方法准确率89%、延迟60 ms。原稿写“遗憾的是，准确率仅有89%，说明本方法仍存在诸多不足”。

可写：新方法将延迟从100 ms降至60 ms，准确率为89%，基线为90%。

不能只写速度收益而删掉准确率，也不能将准确率降低解释成未知机制。

## 2. 结论就近保留必要边界

输入：模型在两个工况完成计算，尚未与实验数据对比。

可写：模型已完成两个工况的计算，尚需与实验数据对比验证。

不能写成“模型已验证”“实现准确预测”或把“尚需验证”作为无用防御删除。

## 3. English evidence strength

Input: An observational study of 24 samples finds an association between X and Y. No intervention or causal identification was performed.

Possible revision: X was associated with Y in the observational study of 24 samples.

Do not substitute “X causes Y”, claim a mechanism, or add statistical significance. Place any further qualification where it is needed for the actual claim.

## 4. 技术条件和禁止事项

输入：仅当传感器完成校准且温度低于40 °C时，才能开始加载；未校准数据不得用于定量比较。

可写：传感器完成校准且温度低于40 °C后开始加载；未校准数据不得用于定量比较。

不能删掉“且”、把“低于”改成“低于或等于”，也不能把禁止事项改成不具等义性的操作建议。

## 5. 审稿回复区分计划与完成

输入：审稿人要求独立验证；作者只说明计划下月补充，尚未完成。

回复应如实承认独立验证尚未完成并写清计划；不能声称已新增实验、补充图表或具体行号。若用户需要可提交的回复，指出缺少可报告的完成结果，不替作者虚构。
