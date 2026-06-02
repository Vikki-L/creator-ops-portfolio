# C1 · SolviFox Onboarding Bot · Discord 新人入职自动化

> 一个 Discord Bot 接管所有新校园大使的入职流程 · 5 步自动化 + 知识库 FAQ 智能回答 · 二期优化基于 11 步 Python 数据 pipeline 反哺

## 🎯 The Problem

新校园大使入职原本依赖 Onboarding 团队**人工 DM 一对一处理**：
- 收集姓名
- 手动拉群
- 手动改状态
- 回答常见问题

**效率低 / 易遗漏**，每月新人多的时候 Onboarding 团队会被淹没。

**Discord 平台特殊难点**：没有"邮箱即身份"的天然映射（不像 Slack 邮箱注册），是从 Slack 迁移到 Discord 后最大的卡点。

## 💡 The Approach

### 5 步自动化主流程

```
邀请码识别身份 → 改昵称 → 加角色 → 建私密频道 → 发欢迎消息
```

### 关键设计

| 设计 | 说明 |
|------|------|
| **邀请码识别身份机制** | 一次性 / 30 天过期 / 与候选人姓名一对一映射，解决 Discord 没有邮箱映射的根本问题 |
| **状态留底（json 持久化）** | Bot 挂了重启也不丢人 |
| **完整 Onboarding 流程** | 邀请 → 身份确认 → 群组接入 → 任务说明 → FAQ 回复 → 首次视频提交 |
| **知识库智能问答** | 录入数据库，能智能回答大使的常见问题 |
| **与 Recruiting 系统的状态衔接** | 候选人状态在两个系统间自动同步 |

### ⭐ 二期优化的数据依据

为了知道二期"该优化什么"，我设计了一套 **11 步 Python 数据 pipeline**：

```
pull Slack data → filter Onboarding messages → label & prepare 
→ Gemini batch (v1, v2, v3) → aggregate to FAQ → cluster FAQs 
→ generate FAQ dashboard
```

输出 FAQ 聚类成果（哪些问题被问得最多、Coach 标记 marker 的分布）→ **直接驱动 v2 Bot 知识库的内容设计**。

## 📊 Key Results

- ✅ Onboarding 团队**人工 DM 工作量显著下降**
- ✅ Bot 挂掉重启不丢人状态（状态持久化生效）
- ✅ 二期优化**有数据依据**（不是拍脑袋）

## 🔧 What I Owned

- 完整需求文档（v1 → v2 → 下一期）
- Bot 状态机设计 + 邀请码机制设计
- **11 步 Slack 数据分析 pipeline 设计与实现**（Python + Gemini）
- 与 Recruiting 系统的状态衔接方案

## 📂 Related (Internal)

- SolviFox Discord Bot 需求文档（v1 + v2 + 下一期）
- Onboarding 自动化方案 v2 完整文档
- 11 步 Python 数据分析 pipeline 完整代码（脱敏后）
- FAQ 聚类成果 + Coach marker 分析

---

[← Board 03](../) · [← Main Portfolio](../../)
