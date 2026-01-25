### 评测与回归（evals/testing）

条目模板：[`../templates/resource-entry.md`](../templates/resource-entry.md)

---

### 资源列表

- **项目**：[comet-ml/opik](https://github.com/comet-ml/opik)
  - **一句话价值**：开源的 LLM 应用调试/评测/监控平台，提供追踪、自动化评测与仪表盘。
  - **适用场景**：
    - 需要把 LLM 应用“跑出来以后”做可观测、可评测、可对比
    - 想把评测/回归纳入团队工程流程（而不是临时手工评估）
  - **注意事项 / 不适用**：
    - 平台型工具接入成本更高，建议先从最核心链路接入并建立基线
  - **标签**：`Eval` `Observability` `SelfHosted` `LLMApps`
  - **引用/参考**：
    - README/Docs：https://github.com/comet-ml/opik

- **项目**：[promptfoo/promptfoo](https://github.com/promptfoo/promptfoo)
  - **一句话价值**：Prompt/LLM 应用的测试与评测框架，适合做回归对比与 CI 集成。
  - **适用场景**：
    - 想为 prompt、RAG、工具调用流程建立“可回归”的评测用例
    - 需要在 PR/CI 中对比不同模型/不同版本 prompt 的效果
  - **注意事项 / 不适用**：
    - 评测结论强依赖用例与评分标准；不要把“跑了分”当作真实业务质量
  - **标签**：`Eval` `Regression` `CI` `JavaScript`
  - **引用/参考**：
    - README/Docs：https://github.com/promptfoo/promptfoo

- **项目**：[explodinggradients/ragas](https://github.com/explodinggradients/ragas)
  - **一句话价值**：聚焦 RAG 场景的评测框架，提供一组常见 RAG 质量指标与评测流程。
  - **适用场景**：
    - 需要对 RAG 的检索质量/答案质量做量化评测
    - 想建立 RAG 的基线与回归，指导 chunking、检索、rerank 调参
  - **注意事项 / 不适用**：
    - 指标并非万能，建议结合人工评审与线上指标，避免“刷指标”
  - **标签**：`RAG` `Eval` `Metrics` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/explodinggradients/ragas

- **项目**：[truera/trulens](https://github.com/truera/trulens)
  - **一句话价值**：LLM 应用评测与质量评估工具集，可用于实验与部分线上监控场景。
  - **适用场景**：
    - 想对 LLM 应用（含 RAG）建立可复现评测流程
    - 需要对输出质量做结构化评估与对比
  - **注意事项 / 不适用**：
    - 线上可观测需要更完整的采集/存储/权限体系，评估工具不等于全套 APM
  - **标签**：`Eval` `LLMApps` `RAG` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/truera/trulens

- **项目**：[confident-ai/deepeval](https://github.com/confident-ai/deepeval)
  - **一句话价值**：LLM 单元测试/评测框架，强调把评测用例像测试一样纳入工程流程。
  - **适用场景**：
    - 为关键 prompt/关键链路写“可重复跑”的测试用例
    - 做模型/提示词升级时的回归对比
  - **注意事项 / 不适用**：
    - 评测的关键是用例设计与判分标准，建议先从最核心的 10 个用例开始
  - **标签**：`Eval` `Testing` `Regression` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/confident-ai/deepeval

- **项目**：[openai/evals](https://github.com/openai/evals)
  - **一句话价值**：早期经典的评测框架与思路参考，适合理解评测组织方式与用例设计。
  - **适用场景**：
    - 研究如何组织评测集与评测流程（作为参考实现）
    - 想借鉴评测用例结构与评测方法论
  - **注意事项 / 不适用**：
    - 可能不再是最活跃路线，生产落地建议评估维护状态或选择更活跃方案
  - **标签**：`Eval` `Reference` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/openai/evals

