# C2 · Coach Assistant Bot · Slack 上的 Coach 助手

> Slack Bot 接管 Coach 6 大重复劳动 · 让 Coach 专注做内容策略和创意指导

## 🎯 The Problem

Coach 日常工作里大量重复劳动：
- 催 Creator 回复消息
- 发邮件升级（提醒 N 次不听）
- 视频基础审核（重复机械的合规检查）
- 提醒 Creator 标 template 编号（格式规范）
- TikTok 视频破 5K 后提醒做 3 条评论回复拿 bonus
- 回答常见问题

→ **Coach 时间被这些占满，没空做真正高价值的内容策略和创意指导**。

## 💡 The Approach

设计 Slack Bot 的 **6 大功能**：

| # | 功能 | 一句话 |
|---|------|--------|
| 1 | **自动催回复** | 大使 24h 没回消息，Bot 自动 @ 提醒 |
| 2 | **邮件升级** | 提醒 2 次没用，Bot 自动发邮件 |
| 3 | **视频初审** | 大使丢视频过来，Bot 先过一遍基础审核（含硬否决规则）|
| 4 | **格式规范提醒** | 大使发视频没标 template 编号，Bot 提醒补上 |
| 5 | **问答助手** | 大使问常见问题（规则等），Bot 能答（Phase 3）|
| 6 | **5K+ 评论互动提醒** | TikTok 视频破 5K，Bot 提醒大使做 3 条评论回复拿 $10 bonus |

### 与 A3 AI 审核系统的衔接
功能 #3「视频初审」直接复用 A3 的 7 条硬否决规则 + 部分 4 类视频判断逻辑，降低重复建设。

## 📊 Key Results

- ✅ 完整需求文档 v0.3（基于 Notion Creator Hub + Content Coach Guide 整理）
- ✅ 已规划，进入开发对接阶段

## 🔧 What I Owned

- 完整需求文档（v0.1 → v0.3）
- Bot 状态机 + 各功能流程设计
- 与 A3 AI 审核系统的衔接方案
- 与 Creator 行为数据源的对接设计

## 📂 Related (Internal)

- Slack Bot · Coach 助手需求文档 v0.3

---

[← Board 03](../) · [← Main Portfolio](../../)
