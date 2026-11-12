<div align="center">

# 论证脉络
### 学术论文双栏批注 · Academic Argument Annotation

**读懂论文如何论证，而不只是它说了什么。**

[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-open%20standard-243B53?style=flat-square)](https://agentskills.io)
[![ChatGPT](https://img.shields.io/badge/ChatGPT-Skill%20ready-10A37F?style=flat-square)](https://help.openai.com/en/articles/20001066-skills-in-chatgpt)
[![License: MIT](https://img.shields.io/badge/License-MIT-D8B56D?style=flat-square)](LICENSE)

**长论文拆章读 · 中英逐段对照 · 论证链可视化 · 一键生成 HTML**

[快速开始](#快速开始) · [功能特色](#一份论文如何变成一张论证地图) · [安装到 ChatGPT](#安装到-chatgpt) · [安装到 Codex](#安装到-codex-及其他-agent) · [目录结构](#项目结构)

</div>

---

> 一篇论文的价值，不只在结论，也在它如何走到结论。
> **论证脉络**把论文拆解成可追踪的主张、证据、方法与反驳，再把它们编织成一份清晰、可浏览的双栏批注页。

## 快速开始

1. 在 ChatGPT Skills 或支持 Agent Skills 的 agent 中安装本项目。
2. 上传论文 PDF，或提供论文文本/可访问链接。
3. 直接输入：
   `@论证脉络｜学术论文双栏批注`
4. 告诉它课程信息和 HTML 保存位置；如果未提供，agent 会按当前环境询问或采用合适位置。

**你会得到：**一份独立 HTML，左侧为英文原文和学术中文译文，右侧为逐段论证批注，底部附全篇论证结构总览。

## 一份论文如何变成一张论证地图

| 阅读层 | 你会看到什么 |
| --- | --- |
| 原文与译文 | 英文原文保留论证标记；中文以自然学术表达意译，并与原段对应 |
| 五类论证标记 | 🟨 核心论点　🟥 关键概念　🟦 实证证据　🟩 让步/反驳　🟪 方法论 |
| 逐段批注 | 段落功能、在论证链中的位置、有效技巧与潜在漏洞 |
| 全篇总览 | 问题 → 主张 → 证据 → 反驳/限定 → 结论，并提炼强项与薄弱处 |

### 长论文，分章读再合并

长论文不会被一次性压成一段摘要。Skill 先逐章记录问题、主张、证据、异议和章节衔接，再跨章节校对术语与推理关系，最后重建完整论证链。

### 表格与公式，先核对再排版

遇到复杂表格或公式，先整理成 Markdown 表格或结构化公式说明并对照原文核验，再嵌入 HTML。遇到 PDF 提取不清的内容会标出待核验处，不会补造数据或符号。

## 安装到 ChatGPT

### 个人使用：上传 Skill

在 ChatGPT 打开 **Plugins → Skills → Create → Upload from your computer**，下载本仓库中的 Skill 文件夹/压缩包并上传。安装成功后可通过名称直接调用。

Skills 的可用性取决于账号类型与工作区设置；个人 Skills 当前面向符合条件的 Business、Enterprise、Healthcare 和 Edu 用户开放。

### 工作区共享：导入 GitHub marketplace

工作区管理员可将本仓库作为 marketplace 导入，以便工作区成员浏览和安装：

1. 打开 **Admin Console → Plugins → Add → Import marketplace**。
2. Source 填：`https://github.com/Zhangjian-maker/academic-argument-annotation`
3. Path 填：`.agents/plugins`；Branch 留空使用默认分支 `main`。
4. 导入后在工作区插件设置中启用成员安装，并按需安装该 skill。

管理员导入与个人上传受 ChatGPT 账号资格、工作区策略和管理员权限控制；GitHub 仓库本身不会自动出现在所有人的目录中。导入后安装到个人 Skills，才可以在聊天中直接使用名称调用。

## 安装到 Codex 及其他 agent

下载仓库中的 `academic-argument-annotation/` 文件夹，放到 agent 支持的 skills 目录。Codex 可使用个人 skills 目录，或项目内 `.agents/skills/`。确保 `SKILL.md` 位于该 skill 文件夹根部。Agent Skills 格式可被支持该标准的其他 agent 使用；调用方式以对应产品为准。

## 项目结构

```text
.
├── academic-argument-annotation/
│   └── SKILL.md
├── .agents/plugins/
│   ├── marketplace.json
│   └── academic-argument-annotation/
│       └── .codex-plugin/
│           └── plugin.json
├── README.md
├── LICENSE
└── CONTRIBUTING.md
```

## 项目原则

- **忠于原文：**不编造数据、引文、方法或作者立场；翻译保留限定条件。
- **让逻辑可见：**区分作者主张、证据、方法、让步和反驳。
- **诚实标注边界：**PDF 提取、公式识别或论证证据不足时明确指出。
- **结构优先于装饰：**页面视觉服务于阅读和推理追踪，支持桌面与移动设备。

## 参与改进

欢迎提交 Issue 或 Pull Request：术语一致性、不同学科论文适配、HTML 阅读体验、无障碍支持和翻译质量都值得持续打磨。详见 [贡献指南](CONTRIBUTING.md)。

## License

本项目以 MIT License 发布，详见 [LICENSE](LICENSE)。论文原文及其版权仍归原作者和出版方所有。

<div align="center">

**从读懂结论，到看见论证。**

</div>
