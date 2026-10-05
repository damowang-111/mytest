# Python 后端与 Agent 场景练习

两套面向实习准备的场景题。题目使用贴近业务的**模拟数据**，要求自行实现最小 Demo、运行验证并记录结果；文档不提供参考答案。

| 题单 | 内容 | 环境 |
|---|---|---|
| [Python 后端与 Agent 场景题单](./backend-agent-lab/README.md) | 24 题；MySQL、Redis、消息队列、API、文件存储、RAG 与工具调用 | [Compose](./backend-agent-lab/compose.yaml) |
| [Agent 工程场景题单](./agent-lab/README.md) | 24 题；工具权限、知识库、长流程、模型故障、评测与上线 | [Compose](./agent-lab/compose.yaml) |

每套题单都能独立运行。在对应目录执行 `docker compose up -d`，并按题目说明启用可选 profile。两套 Compose 使用相同的本机端口；切换题单时，先在当前题单目录执行 `docker compose down`。停止容器不会删除数据卷。

需要 Docker Desktop、Docker Compose 和本机 Python 开发环境。Compose 只启动基础组件；Python 应用、造数脚本、压测脚本与 Agent 实现由练习者完成。所有默认账号仅用于本机练习。不同机器上的实际性能会有差异，请记录数据量、并发数和测试环境。
