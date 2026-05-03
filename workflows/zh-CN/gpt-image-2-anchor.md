# GPT Image 2 视觉锚点工作流

在 `style_brief.md` 完成后、前端实现前使用这个工作流。

## 目标

使用 Codex 和 GPT Image 2 生成 1-3 张视觉锚点，然后从图像中提取可落地的设计规则。

这些图片不是最终产品。它们是布局、比例、密度、颜色和气质的视觉证据。

## Codex 主路径

让 Codex 生成 1-3 张视觉锚点。每张图应代表一种可行方向，同时保持在 style brief 的约束内。

提示词结构：

```text
请为这个产品生成一张高保真的前端风格探索图。

产品：
[产品摘要]

用户：
[目标用户]

页面：
[页面或站点区块]

风格约束：
[来自 style_brief.md 的视觉方向]

必须展示：
[必需内容和操作]

避免：
[反目标]

输出应像真实的响应式 Web 产品，而不是情绪板、海报或通用模板。
```

## 降级路径

如果无法使用 GPT Image 2：

1. 收集 3-7 张参考截图或 URL。
2. 为每个参考写短视觉总结。
3. 选择一个主方向和一个备选方向。
4. 使用同样的 `visual_anchor.md` 结构继续。

## 审查每个锚点

对每张生成图或参考图识别：

- 哪些布局想法可实现。
- 哪些颜色和对比值得保留。
- 可见的字体层级。
- 有用的组件形状和密度。
- 相关的图像或媒体处理。
- 哪些只是装饰噪音。
- 哪些无法负责任地实现。
- 哪些在移动端会失败。

## Visual Anchor 输出

创建 `visual_anchor.md`：

```md
# Visual Anchor

## Inputs

## Anchor Images

## Keep

## Reject

## Design Tokens to Extract

## Layout Rules

## Component Rules

## Responsive Implications

## Implementation Risks
```

## 硬性规则

- 不要直接按图片实现。
- 不要复制参考中的文案、Logo 或独特品牌资产。
- 不要保留只在静态图里好看的不现实 UI 细节。
- 如果锚点没有清晰导航、层级或真实内容，不要接受。
