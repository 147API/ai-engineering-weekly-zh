### RAG / 检索 / 向量数据库

条目模板：[`../templates/resource-entry.md`](../templates/resource-entry.md)

---

### 资源列表

- **项目**：[weaviate/weaviate](https://github.com/weaviate/weaviate)
  - **一句话价值**：开源向量数据库/检索平台，支持向量检索与过滤，适合做 RAG 的检索底座。
  - **适用场景**：
    - 自托管向量检索，并需要 metadata filter 的检索增强应用
    - 想在工程上可控地管理集合/索引/检索策略
  - **注意事项 / 不适用**：
    - 向量库只是底座，RAG 质量仍需靠数据清洗、chunk 策略与评测回归
  - **标签**：`VectorDB` `RAG` `Retrieval`
  - **引用/参考**：
    - README/Docs：https://github.com/weaviate/weaviate

- **项目**：[infiniflow/ragflow](https://github.com/infiniflow/ragflow)
  - **一句话价值**：端到端的 RAG 引擎/平台，提供从文档处理、检索到对话应用的工程化能力。
  - **适用场景**：
    - 想快速落地“可用的 RAG 应用”，而不是只拼一堆脚本
    - 需要对检索、召回、chunking、索引等环节做可视化/可配置管理
  - **注意事项 / 不适用**：
    - 平台型项目上手成本更高，团队应先明确数据流与评测指标再接入
  - **标签**：`RAG` `Search` `Platform` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/infiniflow/ragflow

- **项目**：[deepset-ai/haystack](https://github.com/deepset-ai/haystack)
  - **一句话价值**：成熟的检索增强与 NLP 应用框架，适合搭建可组合的检索/问答管线。
  - **适用场景**：
    - 需要搭建可配置的检索/问答 pipeline（多 retriever、多 reranker、多数据源）
    - 想要较成熟的工程抽象来管理 RAG 组件
  - **注意事项 / 不适用**：
    - 组件丰富但选择也多，建议先用最小链路跑通并建立评测基线
  - **标签**：`RAG` `Pipelines` `Retrieval` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/deepset-ai/haystack

- **项目**：[qdrant/qdrant](https://github.com/qdrant/qdrant)
  - **一句话价值**：开源向量数据库，支持向量检索与过滤条件，常用于 RAG 的向量索引层。
  - **适用场景**：
    - 需要自托管向量库，并支持 metadata filter 的检索
    - 需要在工程上可控地管理索引、集合与检索策略
  - **注意事项 / 不适用**：
    - “向量库≠RAG质量”，chunk 策略与检索评测往往更关键
  - **标签**：`VectorDB` `ANN` `RAG` `Rust`
  - **引用/参考**：
    - README/Docs：https://github.com/qdrant/qdrant

- **项目**：[milvus-io/milvus](https://github.com/milvus-io/milvus)
  - **一句话价值**：高性能向量数据库，适合更大规模的向量检索与工程化部署。
  - **适用场景**：
    - 向量规模较大、对性能/扩展性有要求的检索场景
    - 需要完善的自托管与运维能力（集群/监控等）
  - **注意事项 / 不适用**：
    - 部署与运维复杂度较高，小团队可先从托管/更轻量方案起步
  - **标签**：`VectorDB` `ANN` `Scalability` `Go`
  - **引用/参考**：
    - README/Docs：https://github.com/milvus-io/milvus

- **项目**：[chroma-core/chroma](https://github.com/chroma-core/chroma)
  - **一句话价值**：面向应用开发的向量数据库/存储，常用于快速原型与中小规模检索。
  - **适用场景**：
    - 需要快速搭建 RAG 原型（本地/轻量自托管）
    - 想要更“应用开发友好”的向量存储体验
  - **注意事项 / 不适用**：
    - 大规模生产场景需评估性能、备份、运维与一致性需求
  - **标签**：`VectorDB` `RAG` `Prototype` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/chroma-core/chroma

