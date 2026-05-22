# RL · Sutton & Barto Notes

《Reinforcement Learning: An Introduction》(2nd Edition, 2020) 学习笔记。

教材 PDF 不入库（见 `.gitignore`），可从 [作者主页](http://incompleteideas.net/book/the-book-2nd.html) 获取 `RLbook2020.pdf`。

## 目录结构

```
.
├── outline.md                    # 全书章节中文索引（含 PDF 页码、面试重点 ★）
├── progress.md                   # 学习进度跟踪
└── notes/
    └── 01-introduction/
        └── 1.1-强化学习是什么.md
```

## 笔记粒度

- **★ 重点节**：逐句精翻 + 讲解批注 + 公式推导 + 代码
- **非重点节**：提炼版（要点 + 表格 + 直觉例子）

## 推荐学习路径（面试导向）

地基：Ch 1 → 2 → 3 → 4 → 5 → 6 → 8 (Dyna-Q + MCTS) → 8.13
进阶：Ch 9 → 10 → 11.3 致命三元组 → Ch 13 策略梯度
应用：Ch 16.5 Atari DQN → Ch 16.6 AlphaGo / Zero
