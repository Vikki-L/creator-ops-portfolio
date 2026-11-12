> 历史公开材料，原文来自 [data-driven-content-ops-dashboards · 7276f46](https://github.com/Vikki-L/data-driven-content-ops-dashboards/blob/7276f46d5ab6a52e3c531e65212fbf741db2eaed/dashboards/01-coach-daily-monitor/README.md)。本次导入用于补齐同一项目的模块资料；原文的数字、上线状态与技术判断未重新验证，使用前请看[效果与材料核对](../../../docs/evidence-and-gaps.md)。

# 🔵 Coach Daily Monitor · 达人每日表现实时大屏

> 管理层和 Coach 每天上班第一件事就打开 · 决策周期从 2 周缩短到每天

## 🎯 The Problem

管理层和 Coach 每天需要回答：
- 我下属昨天/今天发了多少视频？
- 谁的视频跑爆了？谁断崖了？
- 哪些 Creator 没完成 quota？
- 我有多少待审 / 待回复 / 待结算？

原本只能靠：手动拉 Excel + 翻 Slack 群消息 + 凭印象拼出答案。**决策周期长、数据时效差**。

## 💡 The Approach

一个每日表现实时大屏，覆盖多个追踪维度：

| 维度 | 内容 |
|------|------|
| 📊 发布进度 | 当日 / 当周 / 累计视频数 |
| 🎯 Quota 完成 | 每位 Creator 的任务完成度 |
| 🚀 视频表现 | 播放量 · 互动率 · 爆款标记 |
| 🧩 模板命中 | 哪些模板被采用 + 表现 |
| ⚠️ 账号风险 | 异常账号（数据骤降 / 投放停止）|
| 📋 Coach 待处理事项 | 待审 / 待回复 / 待结算 |

### V2 增强
- **CPM 字段**：支持流量价值评估（流量贵不贵，单位成本回报）
- **跨期数据快照**：便于趋势对比
- **按 Coach 维度过滤**：每位 Coach 只看自己下属

## 📊 Key Results

- ✅ 上线后管理层和 Coach **每天上班都会先打开**看下属在当前时段或前一天的视频拍摄与上传数量、近期 Views 数据，并通过 CPM 同比辅助决策
- ✅ **决策周期从原来的两周缩短至每天**，每周做一轮人员优化
- ✅ 配合 A5 达人管理 + B3 评分模型，形成"监控 → 评估 → 调整"的闭环

## 🔧 What I Owned

- 完整需求文档（含 V1 → V2 演进）
- HTML 可交互式原型（Cursor 生成）
- 字段对齐 + 与上游数据源（投稿入库）的衔接
- 与下游模块（A5 达人 CRM / B3 评分）的联动设计

---

[← Back to Repo](../../README.md)
