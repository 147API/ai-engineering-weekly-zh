### 推理 / 部署 / Runtime

条目模板：[`../templates/resource-entry.md`](../templates/resource-entry.md)

---

### 资源列表

- **项目**：[vllm-project/vllm](https://github.com/vllm-project/vllm)
  - **一句话价值**：高吞吐 LLM 推理与服务引擎，面向生产部署与性能优化。
  - **适用场景**：
    - 需要更高吞吐/更低延迟的模型服务（尤其是大并发推理）
    - 自建推理服务，希望有成熟的 serving 方案与社区经验
  - **注意事项 / 不适用**：
    - 部署涉及 GPU/驱动/模型格式等系统问题，建议先在小规模环境验证稳定性与成本
  - **标签**：`Serving` `Inference` `Performance` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/vllm-project/vllm

- **项目**：[ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp)
  - **一句话价值**：轻量本地推理实现（CPU/GPU），推动了本地模型运行生态。
  - **适用场景**：
    - 想在本地/边缘设备跑模型，追求“可控/可离线”
    - 需要理解本地推理与量化（quantization）相关工程细节
  - **注意事项 / 不适用**：
    - 性能与效果受模型与量化配置影响较大；不要把 demo 性能直接外推到生产
  - **标签**：`LocalInference` `Runtime` `Quantization` `C++`
  - **引用/参考**：
    - README/Docs：https://github.com/ggml-org/llama.cpp

- **项目**：[ollama/ollama](https://github.com/ollama/ollama)
  - **一句话价值**：本地模型运行与管理工具，提供较友好的本地部署体验与模型管理能力。
  - **适用场景**：
    - 团队/个人希望快速在本地跑通模型并做原型验证
    - 需要统一管理本地模型版本、拉取与运行
  - **注意事项 / 不适用**：
    - 适合本地/原型/小规模部署；大规模生产服务仍需评估专业 serving 方案
  - **标签**：`LocalLLM` `Runtime` `DeveloperExperience`
  - **引用/参考**：
    - README/Docs：https://github.com/ollama/ollama

- **项目**：[sgl-project/sglang](https://github.com/sgl-project/sglang)
  - **一句话价值**：面向 LLM 推理与编排的框架/运行时，强调性能与工程化能力。
  - **适用场景**：
    - 需要高性能推理服务，并希望在编排层有更强控制力
    - 关注推理侧优化、并发调度与服务稳定性
  - **注意事项 / 不适用**：
    - 技术栈偏系统与性能优化，上手前建议先明确你的瓶颈是否在推理侧
  - **标签**：`Serving` `Inference` `Performance`
  - **引用/参考**：
    - README/Docs：https://github.com/sgl-project/sglang

- **项目**：[BerriAI/litellm](https://github.com/BerriAI/litellm)
  - **一句话价值**：多模型/多供应商的统一调用层（OpenAI-compatible 方向），常用于把调用接口抽象为“同一套 SDK/Proxy”。
  - **适用场景**：
    - 需要对接多家模型供应商，希望统一接口并做路由/策略
    - 想在应用侧降低供应商耦合，便于切换与 fallback
  - **注意事项 / 不适用**：
    - 统一接口不代表语义完全一致，仍需做兼容性测试与回归（尤其是流式与工具调用）
  - **标签**：`Proxy` `OpenAICompatible` `Routing`
  - **引用/参考**：
    - README/Docs：https://github.com/BerriAI/litellm

