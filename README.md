# 论证脉络｜学术论文双栏批注

把学术论文转换为强调论证结构的英中双栏批注 HTML 的 agent skill。

## 调用

在支持 skill 直接提及的 agent 中输入：

`@论证脉络｜学术论文双栏批注`

并附上论文 PDF、文本或可访问链接，以及课程信息和 HTML 输出目录。

## 安装

将 `academic-argument-annotation/` 文件夹复制到 agent 支持的 skills 目录，并保留 `SKILL.md`。Codex 用户可将其放入个人 skills 目录或项目 `.agents/skills/` 目录。安装后可以直接通过上述名称调用。

## 功能

- 长论文先分章节摘要，再综合全篇论证链，避免章节间逻辑断裂。
- 英文原文、流畅中文译文、逐段中文批注一一对应。
- 五类高亮：核心论点、关键概念、实证证据、让步/反驳、方法论。
- 生成深海军蓝导航、sticky 章节导航、桌面双栏和移动单栏的自包含 HTML。
- 表格或公式密集时先以 Markdown/结构化形式核对，再转成 HTML。

完整工作流程和交付规范见 [Skill 定义](academic-argument-annotation/SKILL.md)。