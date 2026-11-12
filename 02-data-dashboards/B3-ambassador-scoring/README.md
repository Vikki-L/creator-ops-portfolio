> 本页属于[Coach × Creator 自营 UGC 系统](../../README.md)，在整条流程中负责：周期评估。模块上下游见[完整归属表](../../docs/module-map.md)。以下保留原案例描述，数字与上线状态请结合[材料核对](../../docs/evidence-and-gaps.md)阅读。

# B3 · Ambassador Scoring · 校园大使潜力评分

> ⭐ Python 自研评分模型 · 评估 600+ 大使 · 辅助 Coach 团队基于数据清退 ~400 位

## 🎯 The Problem

Coach 团队凭经验判断该不该清退某位大使，缺乏量化标准：
- "感觉这人不行了" 是经验判断，但没有数据支撑
- 600+ 位大使**无法逐个手动评估**
- 不同 Coach 的判断标准不一致

需要一套**统一的量化评分体系**辅助决策。

## 💡 The Approach

### 评分模型（Python 自研）

**评分维度**：
| 维度 | 说明 |
|------|------|
| max views | 历史最高播放 |
| median views | 视频播放中位数（看稳定性）|
| 5K 突破率 | 多少比例的视频超过 5K |
| 10K 突破率 | 多少比例的视频超过 10K |
| 100K 爆款率 | 爆款命中率 |
| 早期突破 | 加入后多久出第一个爆款 |
| 视频数 | 累计产出量 |
| 阶段判断 | Early / Mid / Potential Validation |

### 输出
**4 级分级** + 推荐动作：

| 等级 | 推荐动作 |
|------|---------|
| HIGH | 重点培养 |
| MEDIUM | 持续观察 |
| LOW | 警告 + 改进期 |
| DROP RISK | 清退候选 |

### 数据清洗细节
- **Trend / Warmup 视频自动识别与剔除**（关键词匹配）→ 避免被低质量视频拖累评分

### 方法论来源
配套的「三段踢人」标准**来自 D3 Turbo.ai 数据洞察**（"30 视频判断爆款"规律）。详见 [D3 模块](../../04-data-analysis-insights/D3-turbo-insights/)。

## 📊 Key Results

- ✅ **评估 600+ 位大使**
- ✅ **基于学期数据辅助清退 ~400 位**
- ✅ Coach 团队按评分结果执行清退，达人池整体质量明显提升

## 🔧 What I Owned

- **评分模型设计**（多维度权重 + 4 级分级阈值）
- **Python 实现**（数据清洗 + 评分计算 + 报告生成）
- **HTML 报告输出**（Coach 团队直接打开看）
- **与 Coach 清退执行流程对齐**（评分输出 → Coach 团队清退执行 → Creator 池状态更新）

---

[← Board 02](../) · [← Main Portfolio](../../)

## 已收回本项目的详细材料

- [01 · Problem & Context](docs/01-problem-and-context.md)
- [02 · Data Insight · "30 视频判断爆款"](docs/02-data-insight.md)
- [03 · Scoring Model · 评分模型详细设计](docs/03-scoring-model.md)
- [04 · Product Integration · 与 Coach 工作流的集成](docs/04-product-integration.md)
- [05 · Results · 量化效果](docs/05-results.md)
- [sample_data.csv](samples/sample_data.csv)
