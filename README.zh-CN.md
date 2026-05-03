# Codex 前端风格工作流手册

语言：[English](README.md) | 简体中文

Codex 前端风格工作流手册是一个面向 Codex 的前端工作流仓库，用来帮助编程代理做出更稳定、更有设计判断力的前端。

核心思路很直接：不要只对代理说“做得现代一点”然后期待它有审美。应该先确定风格方向，再提取可执行规则，最后用截图验收实现质量。

这个仓库不是模型、npm 包、UI 组件库或训练数据集。它是一组可复用的代理指令、工作流、提示词和示例，适合在没有明确参考网站时指导前端开发。

## 为什么需要这个项目

当给定明确参考站点时，编程代理通常可以较好地复刻结构和视觉。但当需求只是“高级”“现代”“干净”“有创意”这类模糊风格词时，结果很容易变成空洞模板、泛用渐变、信息层级混乱或移动端不可靠。

这个手册把模糊风格意图转成实现约束：

1. 发现真实优秀案例。
2. 使用 Codex 和 GPT Image 2 生成视觉锚点。
3. 审查视觉锚点并提取可落地的设计规则。
4. 实现真实前端。
5. 用桌面端和移动端截图验收。

OpenAI 图像生成文档介绍了 GPT Image 系列模型，并展示了通过 Image API 使用 `gpt-image-2`。参考官方文档：[图像生成指南](https://developers.openai.com/api/docs/guides/image-generation) 与 [模型页面](https://developers.openai.com/api/docs/models)。

## 适合谁使用

- 希望提升 Codex 前端产出质量的用户。
- 使用 Claude Code 或其他代理、但仍需要降级工作流的用户。
- 希望给 AI 生成 UI 建立重复验收标准的维护者。
- 需要在风格、布局和视觉 QA 上建立共同语言的设计师和工程师。

## 快速开始

可以把相关文件复制到你的项目里，也可以在开始前让代理读取这个仓库。

推荐 Codex 提示词：

```text
请使用这个工作流完成前端任务：

1. 读取 AGENTS.zh-CN.md。
2. 按 workflows/zh-CN/style-discovery.md 完成风格发现。
3. 按 workflows/zh-CN/gpt-image-2-anchor.md 生成 1-3 张视觉锚点图。
4. 产出 style_brief.md、visual_anchor.md、implementation_brief.md。
5. 实现前端。
6. 完成 workflows/zh-CN/visual-qa.md 中的视觉验收。
```

如果代理无法生成图片，请使用 `workflows/zh-CN/gpt-image-2-anchor.md` 中的降级路径：收集参考截图或链接，然后手动产出同样的三份 brief。

## 仓库结构

- `AGENTS.md` / `AGENTS.zh-CN.md`：给 Codex 类代理读取的默认前端规则。
- `workflows/`：英文工作流。
- `workflows/zh-CN/`：简体中文工作流。
- `prompts/`：英文提示词模板。
- `prompts/zh-CN/`：简体中文提示词模板。
- `templates/`：英文 brief 模板。
- `templates/zh-CN/`：简体中文 brief 模板。
- `examples/saas-dashboard/`：高信息密度 SaaS 仪表盘示例。
- `examples/portfolio-site/`：创意作品集网站示例。
- `CONTRIBUTING.md` / `CONTRIBUTING.zh-CN.md`：贡献说明。

## 三份必需 Brief

每个前端任务在实现前都应该产出：

- `style_brief.md`：用户、产品类型、参考案例、视觉意图、信息密度。
- `visual_anchor.md`：生成图或参考图、保留点、舍弃点、需要提取的规则。
- `implementation_brief.md`：布局、排版、颜色、组件、响应式行为、状态和 QA 标准。

这三份 brief 是视觉探索阶段和编码实现阶段之间的契约。

## 默认工作流

1. 收集产品目标、用户、页面/功能、关键操作、内容优先级和品牌约束。
2. 搜索或列举同类优秀案例。
3. 使用 Codex 和 GPT Image 2 生成 1-3 张视觉锚点。
4. 审查锚点图并提取可实现规则。
5. 写出三份 brief。
6. 使用现有项目技术栈实现前端。
7. 进行桌面端和移动端截图检查。
8. 迭代到没有明显布局破损、文本溢出、弱层级、空洞首屏或风格漂移。

## 非目标

- 不替代设计系统。
- 不训练或微调模型。
- 不要求像素级复刻生成图。
- 不鼓励复制受版权保护的网站。
- 不要求所有项目使用同一种视觉风格。

## License

MIT
