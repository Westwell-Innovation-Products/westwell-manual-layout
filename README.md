# westwell-manual-layout

西井操作手册版式 Skill：统一手册的版式、表达逻辑、图文顺序和 FMS 术语。

采用最终确认的青蓝配色：黑色正文与主要标题、蓝色一级目录、黑色二级目录、纯白章节扉页；操作入口使用浅灰无框小圆角卡片，注意事项和 Tips 仅保留左侧青色色条。

## 安装

将本仓库克隆到 Codex 的 skills 目录；若该目录已有同名 Skill，先确认要更新的版本。

```sh
git clone https://github.com/Westwell-Innovation-Products/westwell-manual-layout.git ~/.codex/skills/westwell-manual-layout
```

也可以下载仓库 ZIP，解压为 `westwell-manual-layout` 文件夹后放入 skills 目录。保留 `references/` 和 `assets/` 的相对结构。在新会话中使用 `$westwell-manual-layout`。

## 使用

```text
使用 $westwell-manual-layout 修改我提供的操作手册。
范围：统一版式和表达逻辑，保留业务含义及全部有效配图。
语言：中文。
输出：HTML 和 PDF。
例外：无。
```

输入文件、修改范围、语言、输出格式和例外由本次请求指定。固定规范维护在 Skill 中，不在每次调用时复制另一套规则。

## 内容

- [SKILL.md](SKILL.md)：技能入口。
- [最终版规范](references/layout-spec.md)：封面、目录、扉页、功能页及提示卡片规范。
- [FMS 术语表](references/terminology.md)：已确认术语及使用边界。
- [调用示例](references/invocation.md)：局部修改、中英文输出和同事交接方法。
- [交付检查清单](references/delivery-checklist.md)：内容、链接、排版及导出检查。
- [FMS 案例](references/fms-examples.md)：区分通用规则与这本手册的局部决定。
- [HTML 组件样例](assets/components.html) 与 [CSS](assets/manual.css)：封面 → 目录 → 章节扉页 → 功能页 → 说明页。
- `assets/examples/`：最终版的封面、章节扉页及功能页截图。

下载后在浏览器中打开 `assets/components.html` 查看样例。示例包含 FMS 业务内容，用于说明组件结构，不替代本次任务提供的业务原文。

新增手册不要求固定为 60 页或固定图片数量。专业含义不确定时先确认，实际界面按钮名称保持原样。
