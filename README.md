# Develop Research Ideas

一个用于**科研选题发现与主线收敛**的 Agent Skill。

它从一个感兴趣的领域、已有论文或初步研究想法出发，帮助：

- 梳理前人研究与领域脉络；
- 发现值得继续研究的问题；
- 核查最近邻工作与新颖性；
- 判断研究价值和可行性；
- 避免无意义发散，最终收敛为一条清晰的研究主线。

它的目标不是批量生成“看起来创新”的 Idea，而是找到一个**有研究价值、有证据支持、能够实际推进的问题**。

## 使用示例

可以直接告诉模型：

```text
请使用 develop-research-ideas。

我对 LLM Agent Security 感兴趣，
但目前还没有具体 Idea。

请从前人研究开始梳理，
寻找值得研究的问题，并最终帮我收敛一条主线。
```

也可以用于：

```text
我已经读了几篇论文，帮我从这些工作中寻找新的研究机会。
```

```text
我已经有一个初步 Idea，先帮我核查是否已有类似工作。
```

```text
我现在有几个候选方向，帮我比较并收敛到一条。
```

## 项目结构

```text
develop-research-ideas/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── icon.svg
└── references/
    ├── field-discovery.md
    ├── domain-checks.md
    ├── templates.md
    └── case-retrospective.md
```

`SKILL.md` 是核心工作流，`references/` 中包含领域发现、检查规则、输出模板和选题案例等辅助内容。

## 安装

下载仓库：

```bash
git clone https://github.com/ryxucas/develop-research-ideas.git
```

或在 GitHub 页面选择：

```text
Code → Download ZIP
```

然后将完整 Skill 目录导入支持 Agent Skills 的环境。

## 设计原则

- Problem First, Method Second
- Evidence Before Novelty Claims
- Research Value ≠ Novelty
- Explore Broadly, Converge Deliberately
- Preserve Confirmed Research State

## Disclaimer

本 Skill 用于辅助科研选题和研究设计。

新颖性、研究价值和发表潜力仍需要结合完整文献检索、实际实验以及领域专家判断进行确认。

## 许可说明 / License

Copyright (c) 2026 ryxucas

本项目允许任何人自由使用、复制、修改和分发，包括用于商业用途。

在复制或重新分发本项目或其主要内容时，请保留原作者及本许可说明。

本项目按“现状”提供，作者不对使用本项目产生的任何问题或损失承担责任。

---

Copyright (c) 2026 ryxucas

Permission is granted to freely use, copy, modify, and distribute this project,
including for commercial purposes.

When copying or redistributing this project or substantial portions of it,
please retain the original author attribution and this license notice.

This project is provided "as is", without warranty of any kind.
The author is not liable for any damages arising from its use.
