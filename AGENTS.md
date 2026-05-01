# AGENTS.md

## 项目背景

这是一个用于测试本地 Codex CLI、Codex 云端和 GitHub 联动的仓库。

## 协作规则

1. 本地 Codex 和云端 Codex 都必须优先阅读本文件。
2. 所有重要修改都要通过 GitHub 提交，避免只停留在本地对话中。
3. 修改代码前，先阅读 README.md 和当前目录结构。
4. 修改完成后，说明修改了哪些文件、为什么修改、如何验证。
5. 如需新增功能，优先创建独立分支或 Pull Request，不直接污染 main 分支。
6. 如发现需求不清楚，先在任务说明中列出假设，不要随意扩大范围。

## 本地 Codex 负责

- 本地运行和调试。
- 检查代码是否能启动。
- 处理依赖安装、终端报错、运行环境问题。
- 将本地修改提交到 GitHub。

## 云端 Codex 负责

- 阅读 GitHub 仓库。
- 根据任务修改代码。
- 创建 Pull Request。
- 在 PR 中说明改动内容和验证方式。

## Git 工作流

- main 分支保持稳定。
- 每个功能使用新分支。
- 云端 Codex 完成任务后提交 Pull Request。
- 本地验证通过后再合并。

## 常用命令

如果是前端项目，优先检查 package.json 后再决定是否执行：

```bash
npm install
npm run dev
npm test
