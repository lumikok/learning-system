# Learning System

一组面向计算机科学与软件工程学习的 Codex Skills。它们把学习、实践、复盘和输出串成一个轻量闭环，强调真实证据、主动练习与可迁移的理解。

## Skills

| Skill | 用途 |
| --- | --- |
| `algorithm-coach` | 通过提示、调试和迁移练习训练算法能力 |
| `blog-from-learning` | 从真实学习与项目经历中提炼技术博客 |
| `fragment-learning` | 用 5–20 分钟探索一个新鲜的技术主题 |
| `idea-miner` | 从近期学习与项目线索中发现可实践的点子 |
| `learn-by-doing` | 以预测、尝试、反馈和迁移为核心进行主动学习 |
| `learning-digest` | 筛选值得沉淀为长期笔记或博客的知识 |
| `one-picture` | 用一张技术图建立复杂主题的整体心智模型 |
| `project-mentor` | 在真实项目中提供循序渐进的工程学习指导 |
| `weekly-review` | 基于代码、笔记和提交记录完成学习周复盘 |

## 使用方式

每个一级目录都是一个独立 Skill，核心说明位于该目录的 `SKILL.md`。将需要的目录复制到 Codex 的个人 skills 目录，或在本仓库中继续开发后再安装。

安装后，可以直接用自然语言描述学习目标；当请求与某个 Skill 的适用范围匹配时，Codex 会读取并遵循对应说明。也可以在请求中明确点名 Skill，例如：

```text
使用 algorithm-coach 带我分析这道动态规划题，但先不要给完整答案。
```

```text
使用 weekly-review，根据我最近七天的 Git 记录做一次学习复盘。
```

## 仓库结构

```text
learning-system/
├── algorithm-coach/
│   ├── SKILL.md
│   └── agents/openai.yaml
├── ...
└── weekly-review/
    ├── SKILL.md
    └── agents/openai.yaml
```

- `SKILL.md`：Skill 的触发条件、行为原则和工作流程。
- `agents/openai.yaml`：可选的界面名称、描述和默认提示配置。

## 设计原则

- **主动学习**：优先让学习者预测、尝试、解释和修正。
- **基于证据**：复盘和内容创作尽量依赖真实代码、提交、笔记与实验。
- **保护思考**：默认不给出会跳过核心学习过程的完整答案。
- **形成闭环**：把探索、练习、项目、复盘和知识输出连接起来。
- **保持聚焦**：每个 Skill 解决一个边界清晰的问题。

## 开发与贡献

修改或新增 Skill 时，请保持目录职责单一，并确保 `SKILL.md` 的 front matter 至少包含清晰的 `name` 与 `description`。提交前建议检查：

1. 触发条件是否明确，且包含不适用场景。
2. 工作流程是否能直接执行，而非只有抽象原则。
3. 是否避免与已有 Skill 大量重叠。
4. 示例、路径和配置中是否包含个人隐私或敏感信息。

更详细的协作约定见 [CONTRIBUTING.md](CONTRIBUTING.md)。

