# paper-reverse-narrative

Claude Code skill：AI 交叉学科论文的**逆向叙事重构**工作流 —— 实验已做完（穷举试错史）时，从真实实验记录反向设计"假设驱动设计"的正向论文故事线。

A Claude Code skill for AI-interdisciplinary paper strategy: when your experiments are done (a long trial-and-error history), reconstruct a positive "hypothesis-driven design" storyline from your real experiment records — comparable-paper selection, storyline & ablation deconstruction, design↔evidence mapping, minimal supplementary-ablation planning, and method-section narrative drafting.

## 工作流概览 (A–E)

- **A 对标文献检索**：候选池 + 加权评分表（体系/任务/方法/指标/消融范式），CrossRef 核验 DOI，全文核验找定位锚点
- **B 对标文拆解**：故事线六句骨架 / 引言逻辑链 / 实验矩阵 / 消融表；其范式缺口 = 你超越它的清单
- **C 逆向故事线**：标题三型候选、摘要六句、设计↔证据映射表、主张自检表
- **D 消融就绪度盘点**：先查落盘数据再定最小补做集（成本表 / 组件留一 / 关键设计有无对照）
- **E 写作大纲**：图表清单、审稿人 Q&A 预演、红线声明表

核心纪律：只用真实实验记录与可核验文献；正向叙事 ≠ 隐瞒局限；消融粒度匹配审稿人背景。

另含两套方法节叙事模板：五问结构（"对比消融了…最终选择…因为数据…"）与"谱系综述→启发→提出"架构段（两句式创新声明句）。

## 安装 / Install

```bash
# 复制到项目级 skills 目录
cp -r paper-reverse-narrative <your-project>/.claude/skills/
# 或用户级（全局可用）
cp -r paper-reverse-narrative ~/.claude/skills/
```

之后在 Claude Code 中输入 `/paper-reverse-narrative` 或在论文策略类任务中自动触发。

## 文件结构

```
paper-reverse-narrative/
└── SKILL.md    # 完整工作流指令（中文）
```

## License

MIT
