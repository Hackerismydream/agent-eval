# 资料索引

整理日期：2026-10-11。以下是首轮阅读入口，已查看原文或项目 README；仓库尚未在本项目中安装、运行。

## 文章

| 资料 | 阅读重点 |
| --- | --- |
| [Anthropic：Demystifying evals for AI agents](https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents) | 入门首选。任务、trial、grader、trace，以及不同 Agent 的评测设计 |
| [Hamel Husain & Shreya Shankar：AI Evals FAQ](https://hamel.dev/blog/posts/evals-faq/) | 从失败案例出发做错误分析、设计标准、校准 judge，处理多轮交互 |
| [Eugene Yan：An LLM-as-Judge Won’t Save the Product](https://eugeneyan.com/writing/eval-process/) | 评测如何进入观察、假设、实验与改进的过程 |
| [Han Lee：Agent Evaluation Infrastructure](https://leehanchung.github.io/blogs/2026/06/13/hidden-technical-debt-agent-evaluation-infra/) | 任务、运行环境、trace、状态变化、verifier 和回放如何组成评测系统 |
| [Anthropic：Quantifying infrastructure noise](https://www.anthropic.com/engineering/infrastructure-noise) | 资源限制和运行环境如何影响 coding agent 的分数 |

## 仓库

| 仓库 | 阅读重点 |
| --- | --- |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) | 通用评测框架，学习任务、执行、工具、评分与日志如何组织 |
| [Inspect Evals](https://github.com/UKGovernmentBEIS/inspect_evals) | 基于 Inspect 的评测实现，作为论文与代码之间的对照 |
| [Harbor](https://github.com/harbor-framework/harbor) | 容器环境中的 Agent 评测框架，Terminal-Bench 2.0 的官方 harness |
| [Sierra τ-bench](https://github.com/sierra-research/tau2-bench) | 业务规则、工具和用户模拟共同构成的多轮 Agent 评测 |
| [AgentEvals](https://github.com/langchain-ai/agentevals) | 执行轨迹匹配与 LLM judge，适合阅读较小范围的评分实现 |

Sierra 的仓库路径仍为 `tau2-bench`，整理时 README 已介绍 τ³-bench。复现时要固定版本；其 `banking_knowledge` 域在 v1.0.1 修复了评分相关任务错误，修复前后的分数不能直接比较，详见[项目说明](https://github.com/sierra-research/tau2-bench)。

## 继续找资料

[BenchFlow awesome-evals](https://github.com/benchflow-ai/awesome-evals) 适合按主题检索资料，其中的 [PATTERNS.md](https://github.com/benchflow-ai/awesome-evals/blob/main/PATTERNS.md) 提供代码和示例。整理时查到默认分支最近提交为 2026-08-20；清单中的部分条目标有未验证提示，引用前仍需核对原文。
