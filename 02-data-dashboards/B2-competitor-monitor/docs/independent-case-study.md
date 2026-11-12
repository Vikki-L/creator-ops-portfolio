> 历史公开材料，原文来自 [data-driven-content-ops-dashboards · 7276f46](https://github.com/Vikki-L/data-driven-content-ops-dashboards/blob/7276f46d5ab6a52e3c531e65212fbf741db2eaed/dashboards/02-competitor-monitor/README.md)。本次导入用于补齐同一项目的模块资料；原文的数字、上线状态与技术判断未重新验证，使用前请看[效果与材料核对](../../../docs/evidence-and-gaps.md)。

# 🟢 Competitor Monitor · 竞品账号监控中台

> 多维度统一管理 · 覆盖 5-8 个北美 AI 教育竞品的 1000+ 账号 · 提供"竞品基准"作为自家决策参照

## 🎯 The Problem

竞品账号原本靠人工 Excel 维护：
- 多个版本散落在不同同事电脑里
- 字段不统一（这个表有 ER、那个表没有）
- 无法跨品牌横向对比
- 无法和内部 Video Tracking 模块联动

## 💡 The Approach

设计了**多维度统一管理表**，按以下维度组织：

| 维度 | 字段示例 |
|------|---------|
| 基础信息 | 账号 / 账号链接 / 平台 / 所属品牌 / Status |
| 数据快照 | Total_videos · Total_views · Avg_views · Median_views · Avg_ER · Top_video_url |
| 爆款分析 | 爆款数 · 爆款率 · 腰部 · 5K-10K · 尾部 · 废品 · 爆款集中度 · 爆款类型_时长 · 爆款类型_内容 |
| 时间轨迹 | first/last_video_posted · 运营时长 · First_viral_date · Days_to_Viral · Videos_to_Viral |
| 系统字段 | 数据更新时间 |

### 关键设计
- **表头自定义**（每位用户独立定制视图，详见 [02-design-principles · 按角色定制视图](../../docs/02-design-principles.md)）
- **与 Video Tracking 模块联动方案**（下一期）

## 📊 Key Results

- ✅ 覆盖 **5-8 个核心追踪竞品品牌**
- ✅ 监控账号数 **1000+**
- ✅ 把"散落 Excel"变成"统一数据中台"，跨品牌横向对比成为可能
- ✅ 为自家 Creator 表现提供**外部基准**（"我们的 10K 命中率 vs 行业基准"）

## 🔧 What I Owned

- 完整 PRD（字段定义 + 数据更新机制）
- 多维度的体系化设计
- 与 Video Tracking 模块的联动方案
- HTML 可交互式原型（Cursor 生成）

---

[← Back to Repo](../../README.md)
