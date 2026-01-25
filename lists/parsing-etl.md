### 文档 / 数据处理（parsing / ETL）

条目模板：[`../templates/resource-entry.md`](../templates/resource-entry.md)

---

### 资源列表

- **项目**：[docling-project/docling](https://github.com/docling-project/docling)
  - **一句话价值**：把 PDF/DOCX/HTML 等文档解析成统一结构，面向“文档进入 GenAI/RAG”场景的工程化 SDK/CLI。
  - **适用场景**：
    - RAG 数据前处理、文档抽取与结构化、文档到知识库流水线
    - 需要可复现的文档解析结果，便于做评测与回归
  - **注意事项 / 不适用**：
    - 文档解析质量需针对自家数据做抽样评测与回归（尤其表格/复杂排版）
  - **标签**：`Parsing` `Documents` `RAG` `LLMReady`
  - **引用/参考**：
    - README/Docs：https://github.com/docling-project/docling
    - Docs：https://docling-project.github.io/docling/

- **项目**：[microsoft/markitdown](https://github.com/microsoft/markitdown)
  - **一句话价值**：把 Office/PDF 等文档转换为 Markdown 的工具，常用于把资料变成“LLM 可处理”的中间格式。
  - **适用场景**：
    - 需要把用户上传的文档转成结构更清晰的文本（用于检索/摘要/问答）
    - 想快速做“文档→Markdown→分段→索引”的处理链路
  - **注意事项 / 不适用**：
    - 文档结构复杂时仍可能需要额外清洗（表格、脚注、多栏排版等）
  - **标签**：`Parsing` `Markdown` `Documents` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/microsoft/markitdown

- **项目**：[unstructured-io/unstructured](https://github.com/unstructured-io/unstructured)
  - **一句话价值**：文档解析与清洗工具链，覆盖多种文件类型与抽取策略，常用于 RAG 的数据前处理。
  - **适用场景**：
    - 需要处理多种格式（PDF、HTML、Word、PPT 等）并抽取结构化内容
    - 想把“文档清洗/切分/元数据提取”工程化
  - **注意事项 / 不适用**：
    - 复杂文档解析往往需要调参与评估，别指望一次就完美抽取
  - **标签**：`Parsing` `ETL` `RAG` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/unstructured-io/unstructured

- **项目**：[pymupdf/PyMuPDF](https://github.com/pymupdf/PyMuPDF)
  - **一句话价值**：高性能 PDF/文档处理库，适合在工程中做 PDF 文本/图片抽取与处理。
  - **适用场景**：
    - 需要在服务端稳定处理 PDF（抽文本、抽图、拆页、坐标信息等）
    - 想在自有 ETL 里精细控制解析流程
  - **注意事项 / 不适用**：
    - 低层库更灵活但也更需要你自己处理版面与噪声（比如多栏、页眉页脚）
  - **标签**：`PDF` `Parsing` `Library` `Python`
  - **引用/参考**：
    - README/Docs：https://github.com/pymupdf/PyMuPDF

- **项目**：[opendatalab/MinerU](https://github.com/opendatalab/MinerU)
  - **一句话价值**：把复杂文档（尤其 PDF）转成更适合 LLM 的 Markdown/JSON 等结构化格式（偏“面向 LLM 的文档抽取”）。
  - **适用场景**：
    - 需要把 PDF 转成更“可读、可检索”的结构化内容供 RAG/Agent 使用
    - 对抽取质量有要求，希望使用更偏 AI 的解析方式
  - **注意事项 / 不适用**：
    - 抽取质量受文档类型影响大，建议建立小样本评测集做回归
  - **标签**：`PDF` `Parsing` `LLMReady` `RAG`
  - **引用/参考**：
    - README/Docs：https://github.com/opendatalab/MinerU

