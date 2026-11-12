<div align="center">

# 论证脉络
### 学术论文双栏批注 · Academic Argument Annotation

**读懂论文如何论证，而不只是它说了什么。**

[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-open%20standard-243B53?style=flat-square)](https://agentskills.io)
[![ChatGPT](https://img.shields.io/badge/ChatGPT-Plugin%20ready-10A37F?style=flat-square)](https://developers.openai.com/plugins/)
[![License: MIT](https://img.shields.io/badge/License-MIT-D8B56D?style=flat-square)](LICENSE)

**长论文拆章读 · 中英逐段对照 · 论证链可视化 · 一键生成 HTML**

</div>

---

> 一篇论文的价值，不只在结论，也在它如何走到结论。
> **论证脉络**把论文拆解成可追踪的主张、证据、方法与反驳，再编织成清晰、可浏览的双栏批注页。

## 快速开始

在 ChatGPT 插件目录安装后，输入 `@`，选择 **论证脉络**，再上传论文 PDF 或提供文本/链接和课程信息。安装后可重复调用，无须每次复制文件。

本仓库既提供可移植的 Agent Skill，也包含 ChatGPT 公开插件提交包。

## 一份论文如何变成一张论证地图

| 阅读层 | 你会看到什么 |
| --- | --- |
| 原文与译文 | 英文原文保留论证标记；中文以自然学术表达意译并与原段对应 |
| 五类论证标记 | 🟨 核心论点　🟥 关键概念　🟦 实证证据　🟩 让步/反驳　🟪 方法论 |
| 逐段批注 | 段落功能、在论证链中的位置、有效技巧与潜在漏洞 |
| 全篇总览 | 问题 → 主张 → 证据 → 反驳/限定 → 结论，并提炼强项与薄弱处 |

### 长论文，分章读再合并

Skill 逐章记录问题、主张、证据、异议和章节衔接，再跨章节校对术语与推理关系，避免长文摘要截断论证脉络。

### 表格与公式，先核对再排版

复杂表格或公式先整理成 Markdown 表格或结构化公式说明并对照原文核验，再嵌入 HTML。PDF 提取不清时会标出待核验处，不会补造数据或符号。

## 在 ChatGPT 中通过 @ 调用

### 公开插件目录（面向个人用户）

1. 下载 [公开插件提交包目录](chatgpt-plugin/)（或从 Releases 下载 ZIP）。
2. 在 OpenAI 插件开发者目录上传插件 ZIP，完成自动检查并提交审核。
3. 审核通过并发布后，用户可在 ChatGPT 插件目录找到并安装 **论证脉络**。
4. 安装一次后，在输入框输入 `@` 选择 **论证脉络**，之后即可反复调用。

发布需要经过 OpenAI 开发者身份验证、自动检查和平台审核；GitHub 仓库或工作区 marketplace 不会自动变成公开目录条目。仓库文件用于提交，发布状态以开发者目录审核结果为准。

### 工作区 GitHub marketplace

管理员可以在 **Admin Console → Plugins → Add → Import marketplace** 导入本仓库，Path 填 `.agents/plugins`。成员安装后可在该工作区重复使用。该方式仅覆盖该工作区，不能代替公开目录发布。

## Codex 及其他 agent

下载 `academic-argument-annotation/` 并放入受支持的 skills 目录。Codex 显式调用方式为 `$academic-argument-annotation`；支持自动发现的 agent 也可根据论文分析任务匹配该 Skill。

## 项目结构

```text
.
├── academic-argument-annotation/SKILL.md
├── chatgpt-plugin/
│   ├── plugin.json
│   ├── assets/logo.svg
│   └── skills/academic-argument-annotation/SKILL.md
└── .agents/plugins/
    ├── marketplace.json
    └── academic-argument-annotation/
        ├── .codex-plugin/plugin.json
        └── skills/academic-argument-annotation/SKILL.md
```

更新 Skill 时同步更新独立版本与两个插件包中的副本。

## 项目原则

- **忠于原文：**不编造数据、引文、方法或作者立场；翻译保留限定条件。
- **让逻辑可见：**区分作者主张、证据、方法、让步和反驳。
- **诚实标注边界：**PDF 提取、公式识别或证据不足时明确指出。
- **结构服务阅读：**页面适配桌面和移动端，视觉帮助追踪推理。

## 参与改进

欢迎提交 Issue 或 Pull Request。请阅读 [贡献指南](CONTRIBUTING.md)。论文原文版权归作者与出版方所有，请勿提交未获授权传播的全文。

## License

MIT License，详见 [LICENSE](LICENSE)。

<div align="center">**从读懂结论，到看见论证。**</div>
