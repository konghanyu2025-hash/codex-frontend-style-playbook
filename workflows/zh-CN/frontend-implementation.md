# 前端实现工作流

在 `style_brief.md` 和 `visual_anchor.md` 完成后使用这个工作流。

## 目标

把视觉方向转成目标项目中的真实前端。

## Implementation Brief

编码前先创建 `implementation_brief.md`：

```md
# Implementation Brief

## Scope

## Layout

## Navigation

## Components

## Typography

## Color

## Imagery and Media

## Interactions and States

## Responsive Behavior

## Accessibility

## QA Criteria
```

## 构建规则

- 使用现有项目技术栈和约定。
- 先做结构和内容层级，再做装饰样式。
- 为重复交互元素构建完整状态。
- 尽量使用语义化 HTML。
- 图标只在能明确表达已知操作时使用。
- 卡片、面板和控件在悬停、加载、选中状态下应保持尺寸稳定。
- 明确桌面端、平板和移动端响应式行为。
- 使用真实内容或与产品匹配的可信占位内容。

## 布局规则

- 定义最大宽度、网格轨道、比例和稳定工具栏尺寸。
- 不要用视口宽度缩放字体。
- 不要让内容变化意外改变导航或控件尺寸。
- 除非确实是弹窗、重复项或被框定的工具，不要卡片套卡片。
- 业务工具不要使用大型装饰区块。

## 视觉规则

- 从锚点提取令牌：背景、表面、正文、强调、边框、弱文本、危险、成功和焦点。
- 使用清晰且有限的字体层级。
- 除非设计系统已有明确规则，字距保持正常。
- 检查关键文本和控件的对比度。
- 除非 brief 明确要求，不要让调色板退化成单一色相的多种变化。

## 完成标准

只有满足以下条件才算完成：

- UI 可以本地运行。
- 已审查桌面端和移动端截图。
- 结果匹配 `implementation_brief.md`。
- 主要流程可见且可用。
- 结果看起来是有意识设计过的，而不是只套了样式。
