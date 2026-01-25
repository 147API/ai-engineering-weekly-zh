### 安全 / 合规 / 脱敏

条目模板：[`../templates/resource-entry.md`](../templates/resource-entry.md)

---

### 资源列表

- **项目**：[Azure/PyRIT](https://github.com/Azure/PyRIT)
  - **一句话价值**：面向 LLM 的安全测试/红队工具（提示词注入、越权等攻击面），帮助建立安全评测与回归用例。
  - **适用场景**：
    - 做 LLM 应用安全评审、红队测试、上线前安全回归
    - 希望把“安全测试”工程化成可重复跑的用例集
  - **注意事项 / 不适用**：
    - 安全测试结果需要落到工程措施（权限隔离、最小权限、审计、guardrails），别停留在“跑报告”
  - **标签**：`Security` `RedTeam` `Testing`
  - **引用/参考**：
    - README/Docs：https://github.com/Azure/PyRIT

- **项目**：[microsoft/presidio](https://github.com/microsoft/presidio)
  - **一句话价值**：PII（敏感信息）识别与脱敏工具集，可用于日志/输入输出的隐私保护。
  - **适用场景**：
    - 需要在记录 LLM 请求/响应时做脱敏（邮箱、电话、身份证等）
    - 合规场景下对用户输入输出进行检测与清洗
  - **注意事项 / 不适用**：
    - 识别准确率与覆盖范围需要结合你业务数据做评估与自定义规则
  - **标签**：`PII` `Redaction` `Compliance` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/microsoft/presidio

- **项目**：[protectai/llm-guard](https://github.com/protectai/llm-guard)
  - **一句话价值**：面向 LLM 输入/输出的安全检测与清洗（例如提示词注入、敏感内容、越权等方向的防护组件）。
  - **适用场景**：
    - 想在 LLM 应用入口/出口做基础安全护栏（guardrails）
    - 需要可插拔的安全检查组件，配合策略与审计
  - **注意事项 / 不适用**：
    - 安全不是“装个库就完事”，仍需做权限隔离、最小化工具权限、审计与回归用例
  - **标签**：`Security` `Guardrails` `PromptInjection`
  - **引用/参考**：
    - README/Docs：https://github.com/protectai/llm-guard

- **项目**：[guardrails-ai/guardrails](https://github.com/guardrails-ai/guardrails)
  - **一句话价值**：面向结构化输出与规则约束的 guardrails 工具，帮助约束 LLM 输出格式与内容。
  - **适用场景**：
    - 需要强制结构化输出（JSON/Schema）并做校验与重试
    - 希望用规则/校验器减少“输出漂移”与格式错误
  - **注意事项 / 不适用**：
    - guardrails 会增加调用与重试开销，需评估成本与延迟影响
  - **标签**：`Guardrails` `StructuredOutput` `Validation` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/guardrails-ai/guardrails

- **项目**：[OWASP/www-project-top-10-for-large-language-model-applications](https://github.com/OWASP/www-project-top-10-for-large-language-model-applications)
  - **一句话价值**：OWASP 的 LLM Top 10 风险清单与最佳实践参考，帮助做安全评审与风险对齐。
  - **适用场景**：
    - 做 LLM 应用安全评审/威胁建模/合规对齐
    - 用作团队安全培训与“上线前检查清单”的依据
  - **注意事项 / 不适用**：
    - 清单是框架，不是落地方案；仍需结合业务做具体控制措施与测试用例
  - **标签**：`Security` `OWASP` `ThreatModel`
  - **引用/参考**：
    - README/Docs：https://github.com/OWASP/www-project-top-10-for-large-language-model-applications

