# A3 · AI Video Review · AI 视频自动审核系统 + Prompt 工程

> 用 Gemini 给短视频做多步审核 · AI 自动判断准确率 90%+ · 4 类视频体系 · 6 大维度 · 反幻觉策略

## 🎯 The Problem

人工审核每条视频的痛点：
- 耗时长（一位 Coach 一天审核几十条已经满载）
- 不同 Coach 之间标准不一致
- 新 Coach 上手周期长
- 错误案例（badcase）无沉淀

## 💡 The Approach

### 完整审核链路

```
业务类别识别 → 模板规则匹配 → AI 多步审核 → 人工复核
```

### 模型与决策框架
- **模型**：Gemini
- **7 条客观硬否决规则**：
  AI 生成视频 / 时长 < 10s / 无人脸无产品 / 纯屏幕录制 / 搬运他人视频 / 非英语无字幕 / 音频不可用

### 4 类视频 Prompt 体系
| 类型 | 状态 |
|------|------|
| Skit | ✅ |
| Product Lead | ✅ |
| Original | ✅ |
| Traditional | 🚧 |

### 6 大审核维度
品牌露出 · 脚本结构 · 字幕 · 口播准确性 · 模板命中 · 强弱营销识别

### 反 AI 幻觉策略
- **JSON Schema enum 锁死输出格式**
- **反例先于正例**（让 AI 先看到什么是错的）
- **二次自检**（输出后自己回头检查一遍）
- 把主观「评级」改造成客观 **decision 字段**（reject / review / pass）

### Badcase 闭环
错误案例沉淀回 Prompt 优化数据源 → 下一轮 Prompt 迭代直接吸收

## 📊 Key Results

- ✅ **AI 自动判断准确率 90%+**
- ✅ 最终结论以人工复核为准，AI 作为辅助**提前识别问题、统一标准**
- ✅ 新 Coach 上手周期显著缩短（参考 AI 给出的判断 + 维度拆解就能学会）

## 🔧 What I Owned

- 完整 Prompt 体系设计（4 类视频 × 6 维度的矩阵）
- 多版本演进（v1.0 → v1.6）
- Prompt-Studio 内部平台原型设计
- Badcase 库管理与反哺机制
- 与开发对接（API 集成 + 审核工作台对接）

## 📂 Related (Internal)

- 4 类视频完整 Prompt 文档
- 审视频 Prompt 当前版本 + 演进 Roadmap
- Prompt-Studio 原型 HTML
- 测试样本库 + Badcase 案例集

---

[← Board 01](../) · [← Main Portfolio](../../)
