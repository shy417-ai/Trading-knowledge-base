# Trading Knowledge Base

交易系统知识库。

这是一个面向个人交易系统的知识库。它采用类似 Andrej Karpathy 倡导的个人知识库思路：不要只把资料扔进一个静态 RAG 仓库，而是持续把原始材料、对话、交易复盘和研究结论压缩成可读、可引用、可更新的知识单元。

目标不是保存更多信息，而是让知识库逐渐回答这些问题：

- 我相信哪些市场假设？
- 哪些交易 setup 被历史证据支持？
- 哪些规则是硬约束，哪些只是启发式？
- 最近的亏损来自系统失效、执行偏差，还是样本内幻觉？
- 下一轮研究应该验证什么？

## Workflow

1. Capture: 把原始材料放入 `00_raw/` 或 `01_inbox/`。
2. Distill: 从材料中提炼 claim、概念、风险、反例，写入 `02_extracts/`。
3. Organize: 将稳定知识沉淀到 `03_concepts/`、`04_playbooks/`、`05_system/`。
4. Review: 将交易、回测和周/月复盘写入 `06_reviews/`。
5. Write back: 每次重要复盘后，更新已有概念、setup、规则，而不是只追加新笔记。

## Directory Map

- `00_raw/`: 原始资料。PDF、网页摘录、书摘、课程笔记、数据说明等。
- `01_inbox/`: 未处理想法。临时想法、问题、聊天记录、交易灵感。
- `02_extracts/`: 从原始资料中提炼出的结构化知识卡片。
- `03_concepts/`: 市场结构、订单流、波动率、风险管理、心理等稳定概念。
- `04_playbooks/`: 可执行交易剧本，包括入场、失效、仓位、出场和样例。
- `05_system/`: 交易系统级规则、检查清单、风控约束和研究路线图。
- `06_reviews/`: 日/周/月复盘、交易日志、回测结论和规则变更记录。
- `99_prompts/`: 用于让 LLM 处理资料、复盘和维护知识库的提示词。
- `_templates/`: 新建笔记时使用的模板。
- `wiki/`: 首页、索引和主题地图。

## Operating Principles

- Evidence first: 每个稳定结论都应能追溯来源、样本或交易记录。
- Small notes, strong links: 单篇笔记只回答一个问题，并链接到相关概念或剧本。
- Separate belief from rule: 市场观点、交易规则和执行纪律分开存放。
- Prefer falsifiable claims: 用“在什么条件下会失效”来检验知识质量。
- Review changes: 修改系统规则时记录原因、证据和生效日期。

## First Three Habits

1. 每天把交易想法和盘后观察放到 `01_inbox/`。
2. 每周把最重要的 3-5 条观察压缩成 `02_extracts/` 的 claim 卡片。
3. 每月更新一次 `05_system/`，只让被证据支持的内容进入系统规则。
