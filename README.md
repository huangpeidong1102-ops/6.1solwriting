# 6.1solwriting

基于6.1 sol写的

面向增材制造高熵合金的 SCI 学术写作 Agent Skill。

仓库：[huangpeidong1102-ops/6.1solwriting](https://github.com/huangpeidong1102-ops/6.1solwriting)

技能标识：`6-1sol-writing`；显示名称：**6.1sol writing**。

结合八篇已发表课题组论文的表达习惯、问题与证据编排方法，以及反防御性写作规则，辅助提纲、摘要、引言、结果、讨论与英文润色。

## 主要功能

- 学习图号定位、组织与相区对照、定量性能、机制归因的段落节奏。
- 提供 20 条基础句式和 5 种完整段落范式。
- 支持增材工艺、热处理、表征、力学曲线和断口的证据化写作。
- 按需使用强化模型，并核对参数来源、单位、适用条件和计算闭合性。
- 减少重复免责、过度自我弱化与空泛修辞，保留科学条件及真实性能权衡。

本技能的风格依据与科学内容分别管理：新论文使用作者本次实验数据，样文数据不自动迁移。
名称中的“6.1sol”是技能名称，不指定或切换运行模型。

## 使用

下载仓库内容后，将包含 `SKILL.md` 的本目录安装到所用工具的技能目录；保留 `agents/` 和 `references/` 的相对位置。
Codex 默认位置为 `~/.codex/skills/6-1sol-writing/`；使用自定义技能根目录时，放入对应的 `skills` 子目录。

可明确调用 `$6-1sol-writing`，或使用自然语言：

> 用 6.1sol writing，按课题组风格润色下面的 Results。

> 用 6.1sol writing，先根据这些图和实验记录拟定论文提纲。

> 用 6.1sol writing，检查这段 Discussion 的强化机理与表达。

请提供当前稿件、对应图表和必要测试条件。局部润色直接处理已有文字；新稿或大幅重构先核对数据与提纲。

## 文件结构

```text
SKILL.md
agents/openai.yaml
references/
  style-and-vocabulary.md
  microstructure-and-mechanics.md
  strengthening-models.md
  nature-storyboarding.md
```

入口按任务读取参考文件，避免一次加载全部内容。
八篇样文的 DOI 和定位保存在参考文件中；仓库不分发原论文 PDF、个人路径或未发表实验记录。

## 来源与许可

来源、改写范围及上游许可见 [ATTRIBUTION.md](ATTRIBUTION.md)。
本仓库尚未为新增内容选择项目级许可证；这里不声明整个项目采用 MIT 或其他许可。
上游 ARS 材料的版权与 CC BY-NC 4.0 许可通知保存在 `third-party/`，该通知不把其他来源或新增内容自动变为同一许可。
维护者应根据实际采用内容和来源许可确定项目级授权，再添加相应 LICENSE。

## 验证范围

初版完成技能结构、相对链接和编码检查，以及两项独立模拟写作任务检查。
模拟验证不构成对所有材料体系、统计分析或模型参数的科学有效性认证。
