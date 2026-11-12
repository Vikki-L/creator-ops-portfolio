# 完整模块归属表

[返回项目首页](../README.md) · [系统总览](system-overview.md)

14 个旧模块属于同一个自营 UGC 运营项目。下表按业务关系排列，保留旧编号用于定位原材料。

| 旧编号 | 在系统中的位置 | 负责什么 | 输出 / 下游 | 归属说明 |
|---|---|---|---|---|
| [C1](../03-ai-workflow-automation/C1-onboarding-bot/) | 新人接入 | 身份确认、角色与欢迎引导 | Creator 归属、入职状态 | D2 分析反哺下一期设计 |
| [B6](../02-data-dashboards/B6-creator-submission-pipeline/) | 投稿与数据入口 | 解析投稿链接、入库、追踪 | A1 待审、A2 明细、B1 数据 | 服务下游，不是独立看板 |
| [A1](../01-coach-creator-dual-platform/A1-videos-review/) | 内容协作核心 | Coach 复核与 Creator 查看反馈 | 审核结论与反馈历史 | 双端查看同一条内容 |
| [A3](../01-coach-creator-dual-platform/A3-ai-video-review/) | AI 审核配套 | 分类、规则匹配、AI 建议、badcase | 可复核的判断建议 | 嵌入 A1；自动处理边界待核对 |
| [A2](../01-coach-creator-dual-platform/A2-internal-payroll/) | 结算核心：Coach 侧 | 生成明细、调整、导出与结果跟踪 | A6 展示的明细、支付批次 | 与 A6 合讲一条结算链路 |
| [A6](../01-coach-creator-dual-platform/A6-creator-earnings/) | 结算核心：Creator 侧 | 查看收入明细、确认和历史 | 确认结果与异议 | 与 A2 联动，不是另一个产品 |
| [B1](../02-data-dashboards/B1-coach-daily-monitor/) | 日常运营 | 投稿、视频表现、任务与异常监控 | Coach 当日待处理事项 | 读取 B6 等上游数据 |
| [B3](../02-data-dashboards/B3-ambassador-scoring/) | 周期评估 | 按阶段评估表现、输出建议 | Coach 复核与培养动作 | D3 方法来源；不自动决定人员去留 |
| [B4](../02-data-dashboards/B4-template-dashboard/) | 模板与内容指导 | 按模板、Creator、平台看表现 | 模板维护与指导依据 | 与 D1、B2 关联 |
| [B2](../02-data-dashboards/B2-competitor-monitor/) | 外部内容研究 | 竞品账号与内容数据观察 | 内容策略和模板参考 | 配套研究能力，不是独立业务主线 |
| [C2](../03-ai-workflow-automation/C2-coach-assistant-bot/) | Coach 助手设计 | 提醒、格式检查、初审与 FAQ 规划 | 对应环节的提醒和待处理项 | 原案例为规划 / 开发对接 |
| [D1](../04-data-analysis-insights/D1-video-effectiveness/) | 内容效果复盘 | 按类型、模板、平台复盘 | B4 与 Coach 指导的迭代依据 | 分析工作，不单独当产品模块 |
| [D2](../04-data-analysis-insights/D2-onboarding-analysis/) | 新人漏斗与 FAQ 复盘 | 分析入职到首次投稿的流失与问题 | C1 下一期需求依据 | 与 C1 同属新人流程 |
| [D3](../04-data-analysis-insights/D3-turbo-insights/) | 评分方法来源 | 竞品数据分析与经验假设 | B3 的方法论参考 | 经验阈值需验证，不是通用规律 |

## 未单独成篇的系统页面

原双端总览还提到 All Creators、Coach Hub、Coach Overview、Creator Hub、Creator Overview 和 Template Library。它们属于两端的基础管理、导航和查看能力。公开仓库没有逐页详细 PRD，不把这些页面数量算成新增独立项目，也不补写没有依据的上线状态。

## 为什么保留原目录

原目录已经被五个独立仓库引用。此次先收拢详细材料与阅读入口，保留既有路径；A/B/C/D 继续承担旧材料索引作用，首页和本表承担完整项目导航。
