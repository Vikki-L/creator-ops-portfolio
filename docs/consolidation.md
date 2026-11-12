# 仓库整合与来源

[返回项目首页](../README.md) · [模块归属](module-map.md)

## 整理范围

本次整理的是原 Coach × Creator 自营 UGC 项目。以 `creator-ops-portfolio` 为统一公开入口，将散落在五个独立公开仓库中的详细设计收回对应模块。海外达人自动化属于另一个项目，不在本次范围内。

- 重写项目首页，按业务流程组织阅读顺序。
- 建立系统总览、端到端交接、模块归属、设计决策与效果核对。
- 保留原有目录与 14 个公开模块入口，补上上下游和详细资料链接。
- 导入 25 份已公开材料：24 份 Markdown 与 1 份演示 CSV。
- 完整 PRD、原型、业务代码和原始数据继续保存在私有原始归档。
- 旧独立仓库保留为来源与历史入口；本次没有删除、重命名或归档仓库。

## 固定来源版本

主仓库整理基线：[`5c46a08`](https://github.com/Vikki-L/creator-ops-portfolio/commit/5c46a0834d53120b098c181405c47c0f7665bd25)。导入日期：2026-11-12。

| 原公开仓库 | 来源提交 | 收回的位置 | 文件数 |
|---|---|---|---|
| [ai-video-review-prompt-engineering](https://github.com/Vikki-L/ai-video-review-prompt-engineering) | [`1eb6d34`](https://github.com/Vikki-L/ai-video-review-prompt-engineering/commit/1eb6d343edf5a63bb6488e73f6917debadbaafee) | [模块资料](../01-coach-creator-dual-platform/A3-ai-video-review/) | 6 |
| [campus-ambassador-scoring-system](https://github.com/Vikki-L/campus-ambassador-scoring-system) | [`f5022cd`](https://github.com/Vikki-L/campus-ambassador-scoring-system/commit/f5022cdeb29815f78044e847072cb134b5ca7f78) | [模块资料](../02-data-dashboards/B3-ambassador-scoring/) | 6 |
| [internal-payroll-automation](https://github.com/Vikki-L/internal-payroll-automation) | [`29b7ecd`](https://github.com/Vikki-L/internal-payroll-automation/commit/29b7ecd85b3ff16eb2684e799f9fc258b79ad8cc) | [模块资料](../01-coach-creator-dual-platform/A2-internal-payroll/) | 4 |
| [onboarding-bot](https://github.com/Vikki-L/onboarding-bot) | [`dc35bc8`](https://github.com/Vikki-L/onboarding-bot/commit/dc35bc8eb4ebc1a2615520b5eac9b8df3293eb28) | [模块资料](../03-ai-workflow-automation/C1-onboarding-bot/) | 4 |
| [data-driven-content-ops-dashboards](https://github.com/Vikki-L/data-driven-content-ops-dashboards) | [`7276f46`](https://github.com/Vikki-L/data-driven-content-ops-dashboards/commit/7276f46d5ab6a52e3c531e65212fbf741db2eaed) | [模块资料](../02-data-dashboards/) | 5 |

逐文件来源、原路径、导入位置和 SHA-256 记录在[公开材料导入清单](public-source-imports.json)。导入文件保留原有 MIT 许可适用性；根目录 [LICENSE](../LICENSE) 继续保留。

## 如何处理旧内容

原案例概述继续保留，但在每个模块入口加上了项目归属与材料核对说明。导入的 Markdown 加有固定来源版本提示；失效的 A5 链接改指向系统总览，该修改记录在清单中。CSV 演示数据保持原文件字节，不当作真实团队数据。

原文里的量化效果、AI 自动处理边界、FAQ 版本、付款状态等存在不一致，集中在[效果与材料核对](evidence-and-gaps.md)记录。此次没有猜测并替换成某个数字，也没有把未公开的业务规则补写成事实。

## 后续维护方式

新的公开说明和经过脱敏的案例优先在本仓库对应模块维护；原始材料继续在私有归档按既有路径保存。补充上线证据或修订效果数据时，同时更新效果核对页和相关模块，避免多个仓库继续各写一套。
