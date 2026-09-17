# Contributing

欢迎通过 issue 或 pull request 改进现有 Skill，或贡献职责清晰的新 Skill。

## 新增或修改 Skill

1. 使用小写字母与连字符命名目录。
2. 在 `SKILL.md` 顶部提供 YAML front matter，并填写 `name` 和 `description`。
3. 在 `description` 中同时说明适用场景和主要的不适用场景。
4. 将可执行的工作流程、边界条件与输出要求写入正文。
5. 如需界面元数据，在 `agents/openai.yaml` 中提供对应配置。
6. 同步更新根目录 README 中的 Skills 列表。

## 提交建议

- 一次提交聚焦一个 Skill 或一类相关改动。
- 使用清晰、可追溯的提交信息。
- 不要提交密钥、访问令牌、个人学习记录或其他敏感数据。
- 提交前检查 Markdown 与 YAML 的结构和可读性。

