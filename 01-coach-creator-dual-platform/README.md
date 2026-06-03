# 01 · Coach × Creator Dual Platform
## 双端协作系统

> 一个给 Coach（内部 10 人团队）与 Creator（200+ 北美校园大使）共用的内容协作产品系统。

## Overview

这套系统覆盖校园大使在业务里的**完整生命周期**：
加入 → 拍视频 → 被审核 → 看反馈 → 看到 AI 评分 → 被结算薪资 → 自助确认收入。

每一环原本都散落在 Slack 消息 / Discord 频道 / 飞书表格里。我从 0 到 1 主导设计，把它们整合成一套**统一的内部产品**，由 Coach 端和 Creator 端两套界面共用一套数据模型。

## Modules

| 模块 | 一句话 | 状态 |
|------|--------|------|
| [A1 · Videos & Review](./A1-videos-review/) | 视频审核与反馈（Coach 端 + Creator 端双端） | ✅ 已上线 |
| [A2 · Internal Payroll](./A2-internal-payroll/) | 内部结算管理（Coach 端） · 自动算薪 + 美区薪酬平台半自动打款 | ✅ 已上线 |
| [A3 · AI Video Review](./A3-ai-video-review/) | AI 视频自动审核系统 + Prompt 工程 | ✅ 迭代中 |
| [A5 · Coach × Creator Management](./A5-coach-creator-management/) | 内部 CRM · 达人池管理 | ✅ 已上线 |
| [A6 · Creator Earnings](./A6-creator-earnings/) | Earnings 页面（Creator 端） · 与 A2 双端联动 | ✅ 已上线 |

## Architecture

```
   ┌─── Coach 端 ──────────────────────────────────────────────┐
   │                                                            │
   │  📋 待审视频列表 (A1)        🤖 AI 审核辅助 (A3)          │
   │  💸 结算管理 (A2)            👥 达人 CRM (A5)             │
   │                                                            │
   │  ➕ All Creators（Coach 看下属/内部人员看全员·可筛选）     │
   │  ➕ Coach Hub（个人工作台首页）                            │
   │  ➕ Coach Overview（团队整体概览）                         │
   │                                                            │
   └────────────────────────────────────────────────────────────┘
                          ↕ 共用数据模型
   ┌─── Creator 端 ────────────────────────────────────────────┐
   │                                                            │
   │  🎬 我的视频 + 反馈 (A1)     💰 Earnings (A6)             │
   │                                                            │
   │  ➕ Template Library（模板库 + 每个模板的数据呈现）        │
   │  ➕ Creator Hub（个人主页）                                │
   │  ➕ Creator Overview（个人数据总览）                       │
   │                                                            │
   └────────────────────────────────────────────────────────────┘
```

> 注：标 ➕ 的子模块属于完整系统的一部分（让整套产品成体系），但本仓库未单独立 case study，仅在此架构图中提及。

## Key Outcomes

- 每周协作处理 **2000+ 视频**
- 服务 **10 人 Coach + 200+ Creator**
- Coach 日均节省 **3-5 小时**
- Coach 周结算耗时从 **~10 小时 → 几分钟**

---

[← Back to Main Portfolio](../)
