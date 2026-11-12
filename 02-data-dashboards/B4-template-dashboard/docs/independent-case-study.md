> 历史公开材料，原文来自 [data-driven-content-ops-dashboards · 7276f46](https://github.com/Vikki-L/data-driven-content-ops-dashboards/blob/7276f46d5ab6a52e3c531e65212fbf741db2eaed/dashboards/03-template-dashboard/README.md)。本次导入用于补齐同一项目的模块资料；原文的数字、上线状态与技术判断未重新验证，使用前请看[效果与材料核对](../../../docs/evidence-and-gaps.md)。

# 🟡 Template Dashboard · 模板数据看板

> 70+ 爆款 Hook 模板的统计端 · 让 Coach 知道每个模板「最近数据怎么样、需不需要淘汰、谁拍得好」

## 🎯 The Problem

70+ 爆款 Hook 模板沉淀下来后，Coach 团队需要持续判断：
- 哪些模板还在跑（最近数据好）
- 哪些已经废了（命中率断崖式下跌）
- 哪些大使拍这个模板最有效（适合定向派活）

凭经验判断容易遗漏，需要看板支持。

## 💡 The Approach

模板维度的数据看板：

- **每个模板的近期数据**：播放 / 互动率 / 爆款率
- **模板淘汰判断**：长期低于阈值的标红
- **谁拍这个模板效果好**：按模板 × Creator 的命中率排序
- **跨账号 × 跨平台透视**：同一个模板在 TikTok / IG / YT 三平台的表现对比
- **必拍模板覆盖度**：每位 Creator 必拍模板的完成情况

## 📊 Key Results

- ✅ 配合 Coach 给 Creator 定向派活，**提高模板命中率**
- ✅ 模板淘汰决策从"凭感觉"→"看数据"
- ✅ 反哺周/双周的视频效果分析（哪些模板需要重点投入）

## 🔧 What I Owned

- 数据库 schema 设计（模板 × Creator × 时间的多维表）
- HTML 可交互式原型（Cursor 生成）
- 数据更新机制设计

---

[← Back to Repo](../../README.md)
