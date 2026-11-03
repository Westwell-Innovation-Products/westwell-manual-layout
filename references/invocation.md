# 调用 Prompt

给同事使用的最简形式：

```text
使用 $westwell-manual-layout 修改附件中的操作手册。
输入：本次提供的文件。
范围：统一版式和表达逻辑，保留业务含义与全部有效配图。
语言：中文。
输出：另存 HTML，确认排版后再导出 PDF。
例外：无。
```

局部修改示例：

```text
使用 $westwell-manual-layout，只调整我提供的 HTML 中的操作入口、注意事项和 Tips 卡片。
保持文字、截图、章节编号及分页不变；直接更新该 HTML，不处理英文版或 PDF。
```

中英文输出示例：

```text
使用 $westwell-manual-layout，将提供的中文手册整理为中英文两份独立 HTML，并分别导出 PDF。
以本次文件为内容源，使用 Skill 中的 FMS 术语表；不确定的专业含义先问我。
```

按实际任务修改输入、范围、语言、输出和例外即可，不必把固定规范复制到 Prompt 中。未提供关键输入时先定位用户已经指明的文件；无法确定才询问。

## 给同事的交接

将 `westwell-manual-layout` 整个文件夹放入同事自己的 Codex skills 目录（通常为 `~/.codex/skills/`），保留 `references/` 与 `assets/` 的相对结构。文件夹名与 `SKILL.md` 名称一致。该包不包含完整业务手册，使用时另行提供要修改的文件。若当前客户端技能列表尚未更新，可在新会话中使用 `$westwell-manual-layout`。
