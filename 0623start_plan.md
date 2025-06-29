在 **5 个月出头** 的时间里从 0 到 CVPR 2026 投稿是紧张但可行的，只要做到**目标前移、并行推进、预留缓冲**。下面先给出关键结论，再展开具体时间表与配套建议。

------

## 关键结论速览

- **预计硬截点**：根据 2023–2025 连续 3 届的官方日程（11 月第 2 周注册，第 3 周正式提交）推测，CVPR 2026 的主会论文应在 **2025 年 11 月 14–17 日** 左右提交，注册提前 7 天，补充材料再顺延 7 天。 ([cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2023/Dates?utm_source=chatgpt.com), [cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2024/Dates?utm_source=chatgpt.com), [cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2025/Dates?utm_source=chatgpt.com))
- **留给你的时间**：从今天（2025-06-23）到可能的提交日大约 **21 周**。
- **工作节奏**：3 大阶段、10 个里程碑、21 周周度安排，外加 2 周安全缓冲。
- **最早风险点**：OpenReview 账号与作者名单在注册截止（预计 2025-11-07）后不可更改 ([cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2025/AuthorGuidelines?utm_source=chatgpt.com))；务必在 10 月底前全部确认。
- **写作原则**：遵守 8 页主体 + 附录格式 ([cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2024/AuthorGuidelines?utm_source=chatgpt.com))，对照官方可复现性清单 ([cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2025/AuthorSuggestedPractices?utm_source=chatgpt.com))；建议按 “先写糟糕草稿” 再精修的策略推进 ([medium.com](https://medium.com/@black_51980/writing-a-good-scientific-paper-c0f8af480c91?utm_source=chatgpt.com))。

------

## 1 · CVPR 2026 官方日期尚未公布，该如何估计？

历年 CVPR 主会提交日始终落在 11 月中旬：

| 届次      | 提交截止   | 注册截止   | 补充材料   | 来源                                                         |
| --------- | ---------- | ---------- | ---------- | ------------------------------------------------------------ |
| CVPR 2023 | 2022-11-11 | 2022-11-04 | 2022-11-18 | ([cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2023/Dates?utm_source=chatgpt.com)) |
| CVPR 2024 | 2023-11-17 | 2023-11-04 | 2023-11-26 | ([cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2024/Dates?utm_source=chatgpt.com)) |
| CVPR 2025 | 2024-11-15 | 2024-11-08 | 2024-11-22 | ([cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2025/Dates?utm_source=chatgpt.com)) |

因此在官方页面上线前，可**安全地按照 2025-11-14（周五）提交**来倒排计划。若官方稍有变动，你仍有 2 周缓冲可调整。

------

## 2 · 五个月总体路线图

| 周次 (起-止)                | 主要目标                  | 关键交付物                        |
| --------------------------- | ------------------------- | --------------------------------- |
| **W1-W3 (6-23 → 7-13)**     | 选题与可行性评估          | ★ 最终题目 + 1 页问题陈述         |
| **W4-W6 (7-14 → 8-3)**      | 深度文献查阅、确定创新点  | 系统化笔记 + 明确贡献列表         |
| **W7-W9 (8-4 → 8-24)**      | 数据/代码基线 & 实验框架  | 可跑通的 baseline 结果 & 代码仓库 |
| **W10-W13 (8-25 → 9-21)**   | 核心方法实现，初步结果    | 核心模块 + 初始 ablation          |
| **W14-W16 (9-22 → 10-12)**  | 强化实验、可复现性打磨    | 完整实验表格 + 复现脚本           |
| **W17-W18 (10-13 → 10-26)** | **论文首稿**（8 页）      | 草稿 v0 + 所有图表草图            |
| **W19 (10-27 → 11-2)**      | 内部评阅 & 反复润色       | 草稿 v1（投稿格式合规）           |
| **W20 (11-3 → 11-9)**       | OpenReview 注册、冲刺修改 | 最终稿 v2 + 元数据提交            |
| **W21 (11-10 → 11-16)**     | 正式提交 & 附录整理       | 提交 PDF + suppl. 占位            |
| **W22 (11-17 → 11-23)**     | 补充材料上传              | 代码 zip / 视频 / checklist       |
| **后备 (两周)**             | 风险缓冲                  | 处理应急 bug、重复实验            |

> *★ 若你的题目到 W3 仍摇摆不定，应立即简化问题或调研其他可重用数据集，以免拖延后续链条。*

------

## 3 · 周度任务拆解

### W1-W3 选题冲刺

1. 每天至少阅读 3 篇近 2 年 CVPR/ICCV/ECCV 相关论文，生成调研表。
2. 用 “空白-贡献-差异” 三栏快速评估想法可行性，选择 **1 主线 + 1 备份**。
3. 完成 15 分钟 internal pitch（对同学/导师试讲）。
   - 参考 Freeman 的经典 “怎么写好 CVPR” 建议，把问题、贡献、实验想法各 1-2 句阐明 ([cs.ryerson.ca](https://www.cs.ryerson.ca/~wangcs/resources/How-to-write-a-good-CVPR-submission.pdf?utm_source=chatgpt.com))。

### W4-W6 深耕文献 & 创新点定位

- 为主线想法写一页 “Related Work Map”，标出方法/数据/度量三条纵轴。
- 设计最简 proof-of-concept 实验，哪怕先用公开数据跑 1 天拿负面结果，也能迅速验证方向。
- 同步搭建代码框架：模板推荐 mm-engine / PyTorch Lightning 等方便复现。

### W7-W9 建立 Baseline

- 取得可对照的 baseline 曲线；确保数据预处理脚本与随机种子可复现（日后 Supplementary 会检查）。
- 把实验日志与图表自动同步到论文目录，节省后期制图时间。

### W10-W13 核心方法实现

- **迭代节奏：** 每周一次 ablation，周会讨论，立即修正。
- 与实验同时写 “Method” 草稿；图公式同步更新能避免收尾爆量。

### W14-W16 结果完善与可复现性

- 对照 CVPR 2025 Reproducibility Checklist 提前自检 ([cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2025/AuthorSuggestedPractices?utm_source=chatgpt.com))。
- 生成所有主表格与关键图；留意最终版需满足 8 页限制 ([cvpr.thecvf.com](https://cvpr.thecvf.com/Conferences/2024/AuthorGuidelines?utm_source=chatgpt.com))。

### W17-W18 首稿完成

- 采用 “Shitty First Draft” 策略：先不纠结语言，专注逻辑完整 ([medium.com](https://medium.com/@black_51980/writing-a-good-scientific-paper-c0f8af480c91?utm_source=chatgpt.com))。
- 邀请 2-3 位同行做 **无情评审**；根据反馈集中修改核心漏洞。

### W19-W21 注册-提交

1. **10-31 前**：所有作者完成 OpenReview Profile，检查冲突列表。
2. **11-07（预计）**：Registration Deadline；必须提交题目摘要关键词。
3. **11-14（预计）**：最终稿上传（PDF + 盲审版 + BibTex）。提交后立刻核验生成的 PDF 版式。

### W22 补充材料

- 代码（推荐匿名 GitHub zip），附录实验细节、视频 demo；严格 ≤100 MB。

------

## 4 · 风险缓冲与备选方案

| 风险               | 触发点             | 缓解措施                                                     |
| ------------------ | ------------------ | ------------------------------------------------------------ |
| 算法进展受阻       | W10 前准确率无提升 | **Plan B** 备份课题立即启动；或精简贡献聚焦速度/效率提升     |
| 数据隐私或授权问题 | W7-W9              | 换用公开数据或 synthetic 数据；提前审阅 license              |
| 团队作者信息错误   | 注册日-1           | 建立共享表格，逐项核对拼写 & ORCID                           |
| 版式超页           | W18                | 提前用脚注/图表排版技巧压缩；若仍超限，准备编辑脚本自动调节行距 |

更多写作经验可参考 SJTU Vision 资源汇总页面（含 “如何写好 CVPR提交” 与 “如何被拒稿” 幽默清单）([vision.sjtu.edu.cn](https://vision.sjtu.edu.cn/writing.html?utm_source=chatgpt.com))，以及 Voxel51 的会前准备技巧 ([voxel51.com](https://voxel51.com/blog/how-to-get-the-most-out-of-cvpr?utm_source=chatgpt.com))。社区经验表明，一旦数据与实验完备，主文 8 页写作大约需 1-2 周高强度投入即可完成 ([reddit.com](https://www.reddit.com/r/AskAcademia/comments/efp5kk/how_long_does_it_take_you_to_write_a_68_page/?utm_source=chatgpt.com))。

------

## 5 · 立即行动清单（今天-本周）

1. **锁定研究大方向**（如 3D 重建、点云理解等你熟悉的领域），列出 3 个候选问题。
2. 订阅 ArXiv cs.CV 邮件推送 & RSS，快速跟踪近 30 天论文。
3. 搭建专用 Git 仓库 + Notion/Obsidian 知识库，确保所有阅读和实验记录可追溯。
4. 与潜在合作同学或导师敲定每周例会时间，保持节奏。

只要严格执行上述里程碑并保留 2 周缓冲，你将在 2025 年 11 月中旬自信地按时投稿，为 CVPR 2026 的同行评审打下坚实基础。祝你一路顺利！

![image-20250623162231659](D:\workbench\paper\paper_note\assets\image-20250623162231659.png)