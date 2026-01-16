### 可观测 / 调试 / Streaming

条目模板：[`../templates/resource-entry.md`](../templates/resource-entry.md)

---

### 资源列表

- **项目**：[langfuse/langfuse](https://github.com/langfuse/langfuse)
  - **一句话价值**：开源 LLM 可观测平台，用于采集/分析 LLM 应用的 traces、prompt、成本、延迟等指标。
  - **适用场景**：
    - 需要把 LLM 调用“看得见”（请求链路、耗时、错误、成本、prompt/输出）
    - 想在迭代 prompt/模型时保留可追溯数据，支持对比与回归
  - **注意事项 / 不适用**：
    - 线上接入需注意敏感数据脱敏与访问控制；不要把用户隐私直接打到日志里
  - **标签**：`Observability` `Tracing` `Prompt` `SelfHosted`
  - **引用/参考**：
    - README/Docs：https://github.com/langfuse/langfuse

- **项目**：[Arize-ai/phoenix](https://github.com/Arize-ai/phoenix)
  - **一句话价值**：开源的 LLM 评测与可观测工具，常用于排查 RAG/Agent 质量问题与数据问题。
  - **适用场景**：
    - 调试 RAG（检索是否命中、答案是否引用正确、哪里开始漂）
    - 想把评测/追踪数据可视化，辅助定位质量瓶颈
  - **注意事项 / 不适用**：
    - 需要先定义你关心的质量指标/用例，否则“有面板但不知道看什么”
  - **标签**：`Observability` `Eval` `RAG` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/Arize-ai/phoenix

- **项目**：[openlit/openlit](https://github.com/openlit/openlit)
  - **一句话价值**：开源 AI/LLM 可观测平台，强调 OpenTelemetry 原生，支持成本、延迟、链路追踪等。
  - **适用场景**：
    - 你已经在用 OpenTelemetry，希望把 LLM/Agent 的指标统一纳入 OTel 体系
    - 需要快速自托管一套可观测栈（含看板）来排查线上问题
  - **注意事项 / 不适用**：
    - 自托管需要存储与采集组件（如 ClickHouse/OTel Collector），要评估运维成本
  - **标签**：`Observability` `OpenTelemetry` `SelfHosted`
  - **引用/参考**：
    - README/Docs：https://github.com/openlit/openlit
    - Docs：https://docs.openlit.io/

- **项目**：[Helicone/ai-gateway](https://github.com/Helicone/ai-gateway)
  - **一句话价值**：轻量 AI 网关（OpenAI-compatible），提供路由、缓存、限流、可观测等能力（更偏“LLM 的 Nginx”）。
  - **适用场景**：
    - 多模型/多供应商接入，希望统一入口并做策略控制（限流/缓存/负载均衡）
    - 需要在网关层做请求观测与基础治理
  - **注意事项 / 不适用**：
    - 网关解决的是“入口治理”，不等于应用层评测/质量保障
  - **标签**：`Gateway` `Observability` `RateLimit` `Caching`
  - **引用/参考**：
    - README/Docs：https://github.com/Helicone/ai-gateway

