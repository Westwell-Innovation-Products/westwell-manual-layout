---
name: westwell-manual-layout
description: 按已确认的西井青蓝手册样式创建、修改或统一操作指南，处理功能页逻辑、章节扉页、目录、步骤配图、注意事项与 Tips，以及中英文术语和 A4 分页。适用于产品操作手册；不将此版式自动用于宣传材料或通用网页。
---

# Westwell Manual Layout

依据用户最终确认的青蓝版手册工作。正文与主要标题黑色；目录一级蓝色、二级黑色；章节扉页纯白；操作入口浅灰、4px 圆角、无框；提示卡片仅保留左侧青色色条。不要从历史配色预览或旧规范恢复已经取消的方案。

## 工作方式

1. 从当前请求确定输入文件、修改范围、语言和交付格式。已有手册优先做局部修改；没有要求时不重建内容、不翻译、不同时改其他语言或导出 PDF。明确的本次例外优先于 Skill。
2. 阅读 [最终版规范](references/layout-spec.md)。复用现有 DOM 时按样式角色适配；创建新手册时使用 [CSS](assets/manual.css) 和 [HTML 组件样例](assets/components.html)，不要用模板示例内容替代用户原文。
3. 按内容性质组织页面。功能页使用“标题 → 操作入口 → 简短场景/用途说明 → 操作文字及对应配图 → 注意事项/Tips”。解释、场景和规则不强行套操作编号或入口。
4. 翻译或处理 FMS 专业内容时阅读 [术语表](references/terminology.md)。保留界面按钮原名；遇到影响业务含义的不确定术语先询问，其他独立部分继续处理。
5. 交付前使用 [检查清单](references/delivery-checklist.md)，检查实际渲染、图文关系、页面溢出和本次修改范围。新增脚本或模板需运行验证，不能仅凭源代码判断效果。

## 按需资源

- [调用示例](references/invocation.md)：给同事的简短 Prompt；只填写本次任务参数，不复制一套规范。
- [FMS 案例与样板来源](references/fms-examples.md)：区分这本手册的局部决定与通用规则。
- `assets/examples/cover.png`、`assets/examples/chapter-opener.png`、`assets/examples/function-page.png`：最终确认版的封面、扉页和功能页参照，包含 FMS 示例内容；不当作新任务的事实来源。HTML 组件样例按封面、目录、扉页、功能页、说明页排列。
- `assets/logo-horizontal.jpg`：正式横版标志，保持比例与配色。

保持 Skill 自包含。已有项目具备字体、Logo 和图标时优先沿用正确资源；不要为一次版式调整强制新增联网字体或更换工具栈。处理实际 PDF/Word 等格式时再使用当前环境对应的导出能力。不同格式保持同一视觉与内容原则，但不假设 HTML CSS 可直接移植到 Word。
