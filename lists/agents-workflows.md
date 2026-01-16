### LLM 应用框架/编排（agents/workflows）

条目模板：[`../templates/resource-entry.md`](../templates/resource-entry.md)

---

### 资源列表

- **项目**：[langchain-ai/langchain](https://github.com/langchain-ai/langchain)
  - **一句话价值**：面向 LLM 应用的框架与组件集合，覆盖链式工作流、工具调用、RAG、Agent 等常见形态。
  - **适用场景**：
    - 快速搭建多步 LLM 工作流（模型调用 + 工具 + 记忆/状态）
    - 需要丰富生态集成（数据加载、向量库、工具适配等）
  - **注意事项 / 不适用**：
    - 抽象层较多，生产环境建议配套评测/回归与可观测，否则容易“能跑但难控”
  - **标签**：`Agents` `Workflows` `RAG` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/langchain-ai/langchain
    - Docs：https://python.langchain.com/

- **项目**：[run-llama/llama_index](https://github.com/run-llama/llama_index)
  - **一句话价值**：面向 RAG/数据增强型 LLM 应用的框架，提供数据连接器、索引、检索与编排能力。
  - **适用场景**：
    - 快速搭建“数据→索引→检索→生成”的 RAG 原型
    - 需要多数据源连接器与可配置检索策略的应用
  - **注意事项 / 不适用**：
    - RAG 质量强依赖数据清洗与评测；不要只“接上向量库就上线”
  - **标签**：`RAG` `Indexing` `Retrieval` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/run-llama/llama_index
    - Docs：https://docs.llamaindex.ai/

- **项目**：[microsoft/autogen](https://github.com/microsoft/autogen)
  - **一句话价值**：多智能体（multi-agent）编排框架，强调代理间协作与对话式任务分解。
  - **适用场景**：
    - 需要多角色协作（规划/执行/审查）来完成长任务的场景
    - 研究/原型阶段探索“多智能体协作”的工程落地方式
  - **注意事项 / 不适用**：
    - 多智能体很容易引入成本与不稳定性，建议先从单代理可控工作流做起
  - **标签**：`Agents` `MultiAgent` `Orchestration` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/microsoft/autogen

- **项目**：[crewAIInc/crewAI](https://github.com/crewAIInc/crewAI)
  - **一句话价值**：面向“角色扮演式”多代理协作的框架，强调角色、任务与工具的组织方式。
  - **适用场景**：
    - 希望用“角色/任务”结构化组织一组代理来完成复杂任务
    - 快速验证多代理协作在某个垂直场景的可行性
  - **注意事项 / 不适用**：
    - 生产落地前务必补齐评测回归、权限隔离与成本预算（多代理容易失控）
  - **标签**：`Agents` `MultiAgent` `Workflow` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/crewAIInc/crewAI

