### 开发者工具（CLI / 插件 / 模板）

条目模板：[`../templates/resource-entry.md`](../templates/resource-entry.md)

---

### 资源列表

- **项目**：[Aider-AI/aider](https://github.com/Aider-AI/aider)
  - **一句话价值**：终端里的 AI 结对编程工具，能在你的代码库上下文中完成修改与重构。
  - **适用场景**：
    - 个人/小团队想把 AI 辅助开发融入日常（尤其是重构、修 bug、加小功能）
    - 想要在本地 repo 里“对话式改代码”，并保留可审查的 diff
  - **注意事项 / 不适用**：
    - 仍需你做代码审查与测试；建议限制权限与敏感文件，避免误改
  - **标签**：`CodingAgent` `CLI` `DeveloperTools`
  - **引用/参考**：
    - README/Docs：https://github.com/Aider-AI/aider
    - Docs：https://aider.chat/docs/

- **项目**：[continuedev/continue](https://github.com/continuedev/continue)
  - **一句话价值**：VS Code / JetBrains 的开源 AI 编程助手，可对接多种模型并在 IDE 内工作。
  - **适用场景**：
    - 想在 IDE 内获得“理解代码库 + 生成/修改代码”的辅助能力
    - 希望模型可替换（自建/第三方/本地模型皆可）而不锁定供应商
  - **注意事项 / 不适用**：
    - IDE 插件更依赖配置与权限管理，团队使用建议统一配置与审计策略
  - **标签**：`IDE` `CodingAgent` `Plugin`
  - **引用/参考**：
    - README/Docs：https://github.com/continuedev/continue

- **项目**：[modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers)
  - **一句话价值**：MCP（Model Context Protocol）服务器集合，为 Agent 提供标准化“工具/数据源”接入方式。
  - **适用场景**：
    - 你在做 Agent 工具生态，希望用标准协议对接外部系统
    - 想快速复用现成 MCP Server（文件、浏览器、数据库等）搭建工具链
  - **注意事项 / 不适用**：
    - 工具接入意味着权限边界扩大，务必做最小权限与审计（尤其是写操作）
  - **标签**：`MCP` `Tools` `Agents`
  - **引用/参考**：
    - README/Docs：https://github.com/modelcontextprotocol/servers

- **项目**：[astral-sh/uv](https://github.com/astral-sh/uv)
  - **一句话价值**：更快的 Python 包管理与环境工具，适合提升 AI 工程项目的依赖安装与可复现性。
  - **适用场景**：
    - AI/数据项目依赖多、安装慢，希望加速并减少“works on my machine”
    - 需要更稳定的依赖锁定与环境管理
  - **注意事项 / 不适用**：
    - 迁移前要评估与你现有 pip/poetry/conda 工作流的兼容与团队习惯
  - **标签**：`Python` `DevTools` `Reproducibility`
  - **引用/参考**：
    - README/Docs：https://github.com/astral-sh/uv

