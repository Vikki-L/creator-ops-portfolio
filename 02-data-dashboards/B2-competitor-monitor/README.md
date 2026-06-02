# B2 · Competitor Monitor · 竞品账号监控中台

> 31 字段五维度统一管理 · 覆盖 5-8 个北美 AI 教育竞品的 1000+ 账号

## 🎯 The Problem

竞品账号原本靠人工 Excel 维护：
- 多个版本散落在不同同事电脑里
- 字段不统一（这个表有 ER、那个表没有）
- 无法跨品牌对比
- 无法和内部 Video Tracking 模块联动

## 💡 The Approach

设计了**31 字段 × 五维度**的统一管理表：

### 五维度结构

| 维度 | 字段数 | 字段示例 |
|------|--------|---------|
| 基础信息 | 5 | 账号 / 账号链接 / 平台 / 所属品牌 / Status |
| 数据快照 | 6 | Total_videos · Total_views · Avg_views · Median_views · Avg_ER · Top_video_url |
| 爆款分析 | 13 | 爆款数(>100K) · 爆款率 · 腰部 · 5K-10K · 尾部 · 废品 · 爆款集中度 · 爆款类型_时长 · 爆款类型_内容 |
| 时间轨迹 | 6 | first/last_video_posted · 运营时长 · First_viral_date · Days_to_Viral · Videos_to_Viral |
| 系统字段 | 1 | 数据更新时间 |

### 关键设计
- **表头自定义**（每位用户独立定制视图）
- **与 Video Tracking 模块联动方案**（下一期）

## 📊 Key Results

- ✅ 覆盖 **5-8 个核心追踪竞品品牌**
- ✅ 监控账号数 **1000+**
- ✅ 把"散落 Excel"变成"统一数据中台"，跨品牌横向对比成为可能

## 🔧 What I Owned

- 完整 PRD（字段定义 + 数据更新机制）
- 31 字段五维度的体系化设计
- 与 Video Tracking 模块的联动方案
- 数据导入 Python 脚本（脱敏后保留）

## 📂 Related (Internal)

- 竞品账号模块 PRD
- 竞品账号模块原型 HTML
- Video Tracking 联动需求文档
- 数据导入脚本

---

[← Board 02](../) · [← Main Portfolio](../../)
