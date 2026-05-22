# Sutton & Barto《强化学习导论》第 2 版 (2020) 中文章节索引

> 用于让 AI 助手快速定位章节，**避免每次重读 548 页 PDF**。
> PDF 页码 = 印刷页码 + 22（例：印刷页 1 = PDF 第 23 页）
> 标 ★ 的为面试重点；标 `*` 的小节为高级/可选。

---

## 第一部分 — 表格型解法（Tabular Solution Methods，地基，**面试重点**）

### 第 1 章 导论 Introduction (印 p.1 / PDF 23)
- 1.1 什么是强化学习 ★
- 1.2 例子
- 1.3 强化学习的要素（policy / reward / value / model）★
- 1.4 局限与适用范围
- 1.5 扩展示例：井字棋
- 1.6 小结
- 1.7 强化学习的早期历史

### 第 2 章 多臂老虎机 Multi-armed Bandits (印 p.25 / PDF 47) ★面试高频
- 2.1 k 臂老虎机问题
- 2.2 动作-价值方法（action-value）
- 2.3 10 臂测试床
- 2.4 增量式实现（incremental update）
- 2.5 非平稳问题（常步长 α）
- 2.6 乐观初始值
- 2.7 上置信界 UCB ★
- 2.8 梯度老虎机算法（softmax / preference）
- 2.9 关联搜索（contextual bandit）
- 2.10 小结

### 第 3 章 有限马尔可夫决策过程 Finite MDPs (印 p.47 / PDF 69) ★必背
- 3.1 智能体–环境接口
- 3.2 目标与奖励
- 3.3 回报与回合（return / episode）
- 3.4 回合式与连续任务的统一记号
- 3.5 策略与价值函数（**Bellman 方程**）★
- 3.6 最优策略与 **Bellman 最优方程** ★
- 3.7 最优性与近似
- 3.8 小结

### 第 4 章 动态规划 Dynamic Programming (印 p.73 / PDF 95) ★必懂
- 4.1 策略评估（policy evaluation）
- 4.2 策略改进（policy improvement）
- 4.3 **策略迭代** ★
- 4.4 **价值迭代** ★
- 4.5 异步动态规划
- 4.6 广义策略迭代 GPI
- 4.7 动态规划的效率
- 4.8 小结

### 第 5 章 蒙特卡洛方法 Monte Carlo Methods (印 p.91 / PDF 113) ★
- 5.1 MC 预测
- 5.2 MC 动作价值估计
- 5.3 MC 控制（带 exploring starts）
- 5.4 无 exploring starts 的 on-policy 控制（ε-soft）
- 5.5 **Off-policy 预测：重要性采样** ★
- 5.6 增量式实现
- 5.7 Off-policy MC 控制
- 5.8* 折扣感知重要性采样
- 5.9* 逐步重要性采样
- 5.10 小结

### 第 6 章 时序差分学习 TD Learning (印 p.119 / PDF 141) ★★面试核心
- 6.1 TD 预测（**TD(0) 更新式**）★
- 6.2 TD vs MC
- 6.3 TD(0) 的最优性
- 6.4 **Sarsa（on-policy 控制）** ★
- 6.5 **Q-learning（off-policy 控制）** ★
- 6.6 期望 Sarsa
- 6.7 最大化偏差与 **Double Q-learning** ★
- 6.8 后位状态（afterstates）
- 6.9 小结

### 第 7 章 n 步自举 n-step Bootstrapping (印 p.141 / PDF 163)
- 7.1 n 步 TD · 7.2 n 步 Sarsa · 7.3 n 步 off-policy
- 7.4* 带控制变量的逐步法 · 7.5 树备份算法 · 7.6* Q(σ) · 7.7 小结

### 第 8 章 表格型方法的规划与学习 (印 p.159 / PDF 181)
- 8.1 模型与规划 · 8.2 **Dyna-Q** ★ · 8.3 模型出错时
- 8.4 优先级扫描 · 8.5 期望更新 vs 采样更新 · 8.6 轨迹采样
- 8.7 实时动态规划 RTDP · 8.8 决策时规划 · 8.9 启发式搜索
- 8.10 Rollout · 8.11 **MCTS** ★
- 8.12 本章小结 · **8.13 第一部分维度总结**（必读图谱）

---

## 第二部分 — 近似解法（Approximate Solution Methods，**深度 RL 入口**）

### 第 9 章 带近似的 on-policy 预测 (印 p.197 / PDF 219)
- 9.1 价值函数近似 · 9.2 预测目标 VE
- 9.3 **随机梯度法 / 半梯度法** ★ · 9.4 线性方法
- 9.5 特征构造（多项式 / Fourier / Coarse / **Tile** / RBF）
- 9.6 步长选择 · 9.7 **神经网络非线性近似** · 9.8 LSTD
- 9.9 基于记忆的近似 · 9.10 核方法 · 9.11 兴趣与强调

### 第 10 章 带近似的 on-policy 控制 (印 p.243 / PDF 265)
- 10.1 回合式半梯度控制 · 10.2 半梯度 n 步 Sarsa
- 10.3 **平均奖励设定** · 10.4 弃用折扣设定 · 10.5 微分半梯度 n 步 Sarsa

### 第 11 章* 带近似的 off-policy 方法 (印 p.257 / PDF 279)
- 11.3 **致命三元组 (deadly triad)** ★（off-policy + bootstrap + 函数近似）
- 11.7 Gradient-TD · 11.8 Emphatic-TD

### 第 12 章 资格迹 Eligibility Traces (印 p.287 / PDF 309)
- 12.1 λ-return · 12.2 **TD(λ)** ★ · 12.5 真在线 TD(λ) · 12.7 Sarsa(λ)

### 第 13 章 策略梯度方法 Policy Gradient (印 p.321 / PDF 343) ★★深度 RL 必懂
- 13.1 策略近似的优势 · 13.2 **策略梯度定理** ★
- 13.3 **REINFORCE** ★ · 13.4 带基线的 REINFORCE
- 13.5 **Actor-Critic** ★ · 13.6 连续任务 · 13.7 连续动作 · 13.8 小结

---

## 第三部分 — 拓展（Looking Deeper，可选）

- 第 14 章 心理学 (印 p.341)
- 第 15 章 神经科学 (印 p.377)
- 第 16 章 应用案例 (印 p.421)：TD-Gammon · Atari DQN · **AlphaGo / AlphaGo Zero**
- 第 17 章 前沿 (印 p.459)：通用价值函数 · Options · 奖励设计 · AI 未来

---

## 推荐学习路径（面试导向，深啃模式）

**地基阶段**（必啃）：1 → 2 → 3 → 4 → 5 → 6 → 8（Dyna-Q + MCTS）→ 8.13 总结
**进阶阶段**（函数逼近）：9 → 10 → 11.3 致命三元组 → 13 策略梯度
**应用阶段**：16.5 Atari DQN → 16.6 AlphaGo / Zero
**可跳过/速读**：7（与 6/12 重叠）、12（理论加深）、14、15、17
