# D2 · Onboarding Analysis · 新大使入职转化漏斗分析

> 分析新加入的校园大使从「入职」到「首次发视频」的转化漏斗 · 直接反哺 C1 Bot 二期设计

## 🎯 What

分析新加入的校园大使从**入职**到**首次发视频**的转化漏斗：
- 哪个环节流失最多
- 流失原因分类
- 哪些大使（按 Tier / 来源 / 时段）更容易留下

## 💡 Approach

### 4.2-4.8 周专项分析
- **数据可视化**：每个环节的转化率图表
- **视频数据快照**：首批发布视频的表现
- **留存率分析**：不同特征大使的留存差异

### 完整 Python 分析 Pipeline
```
01_clean_and_part1 → 02_make_charts → 03_make_report 
→ 04_prep_urls → 05_split_videos (v1+v2) 
→ 06 deep dive (a/b/c/d) → 07-09 Part2 报告 
→ 10 video metadata → 12 dedup → 14 confound check
```

10+ 个 Python 脚本组成的分析 pipeline，输出 HTML 报告 + 视频数据快照。

## 📊 Outcomes

- ✅ 输出 **4.2-4.8 周完整分析报告**（HTML + Markdown）
- ✅ **直接反哺 [C1 SolviFox Bot](../../03-ai-workflow-automation/C1-solvifox-onboarding-bot/) 二期设计**——FAQ 优化 / 流程简化都基于这份数据
- ✅ 识别出 Onboarding 关键流失点，给团队提供改进方向

## 🔧 What I Owned

- 完整分析 pipeline 设计（数据清洗 → 可视化 → 报告生成）
- Python 实现（10+ 脚本）
- HTML 报告输出
- 与 C1 Bot 二期需求的对齐

## 📂 Related (Internal)

- 4.2-4.8 周完整数据分析报告 HTML
- 视频可视化 HTML + 数据快照 Markdown
- 完整 Python pipeline（onboarding_analysis 文件夹）

---

[← Board 04](../) · [← Main Portfolio](../../)
