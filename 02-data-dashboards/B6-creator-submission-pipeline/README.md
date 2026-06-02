# B6 · Creator Submission Pipeline · 投稿自动入库

> Slack 投稿 → 自动解析 → 入库到结算/审核系统 · 让数据采集环节去人工化

## 🎯 The Problem

Creator 在 Slack 群里贴视频链接后：
- Coach 要**手动复制粘贴**到内部系统才能跟踪
- 视频数据更新（播放量、互动率）只能定期手动拉
- 数据采集滞后 → 下游所有数据看板（B1/B2/B3）跟着滞后

## 💡 The Approach

设计自动化的投稿入库 Pipeline：

- **Bot 监听特定频道**（投稿频道）
- **自动解析视频链接**（识别 TikTok / Instagram / YouTube）
- **提取元数据**（账号 / 平台 / 发布时间 / 模板编号等）
- **入库到结算 / 审核系统**（成为 A1 待审队列 + A2 结算数据 + B 类看板数据源）

### 暑期专项
针对暑期投稿密度高峰，单独设计「暑期投稿与结算」流程，对接 Payment Tracker。

## 📊 Key Results

- ✅ 投稿数据采集环节**去人工化**
- ✅ 数据时效提升，下游 B1 看板能拿到更"新鲜"的数据
- ✅ 暑期专项流程支持高密度时段

## 🔧 What I Owned

- 需求文档（中文版 + 飞书版双版本）
- 暑期专项方案设计（与 A2 结算系统联动）
- 与上游 Slack Bot、下游审核 / 结算系统的字段对齐

## 📂 Related (Internal)

- Creator 视频追踪联动需求文档（含飞书版）
- 暑期投稿与结算需求
- 暑期 Payment Tracker Excel

---

[← Board 02](../) · [← Main Portfolio](../../)
