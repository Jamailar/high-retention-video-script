# High Retention Video Script

一个面向真实创作者的视频脚本 Skill：先理解观众要完成什么，再选择合适的视频结构，最后用 HKRR 和 12 点刺激时钟把内容落成可拍、可剪、可检查的脚本。

## 它解决什么问题

这个 Skill 不把每条视频都写成同一种“故事”，也不把产品介绍拆成机械的功能清单。它会根据视频任务选择结构：

- 工具介绍和操作教程：先展示结果，再解释产品、输入、操作、输出和边界。
- 发布、教育、测评、案例和创作者内容：分别匹配揭示、讲解、比较、实验或观点结构。
- 从用户提供的素材、旧稿、录屏、评论、参考视频、知识库文件和说话样本中整理事实、证据、声音和限制。
- 先写能读出口的真人初稿，再用 HKRR 和 12 点刺激时钟做设计与质检。
- 交付一个离线 HTML：逐字 A-roll/B-roll 时间轴、拍摄清单、时钟节拍器、HKRR 评分、质检结论和拍摄 PNG。

## 核心方法

视频设计顺序是：

`原始材料 -> 观众任务与视频类型 -> 一个核心结果或观点 -> 标题与开场 -> 真人初稿 -> HKRR + 12 点时钟 -> AV 时间轴 -> 拍摄 -> 剪辑 -> 质检`

HKRR 的四个元素必须同时存在：

- **H / Happiness（快乐）**：惊喜、爽点、幽默、释然或小胜利。
- **K / Knowledge（知识）**：方法、机制、演示、判断规则或可执行信息。
- **R / Resonance（共鸣）**：观众的痛点、身份、欲望、担忧或自我识别。
- **R / Rhythm（节奏）**：刺激点的分布，以及句子、停顿、画面、声音、剪辑和信息密度的变化。

12 点刺激时钟把整条视频按比例分成 12 个点。`12 / 3 / 6 / 9` 是结构性大刺激，其他点负责持续刷新注意力；最后的 `Finish` 负责偿还承诺并落到行动。时钟不是装饰图，而是脚本设计和剪辑检查工具。

## 安装

将仓库根目录复制为一个 Skill 目录：

```bash
cp -R high-retention-video-script "$CODEX_HOME/skills/high-retention-video-script"
```

也可以放进项目的 `.codex/skills/high-retention-video-script/`。目录中必须保留 `SKILL.md`、`agents/`、`assets/` 和 `references/` 的相对位置。

## 使用

在 Codex 中直接说明要使用这个 Skill，并把所有可能相关的材料一次发来，不需要先整理：

```text
使用 high-retention-video-script。
我要做一个介绍工具的视频。下面是产品资料、参考视频、我的旧稿、录屏和我自己的说话样本。
请先整理背景知识、可用证据、缺失信息和观众任务，再和我确认视频方向；
确认后生成一个最终 HTML，包含逐字稿、A-roll/B-roll 时间轴、HKRR、12 点刺激时钟、拍摄清单和质检。
```

背景资料可以是文字、文件路径、截图、录屏、链接、评论、数据、知识库内容、旧视频或语音转写。资料不完整时，Skill 必须标记假设和暂定内容，不能编造创作者经历、产品能力或用户结果。

## 仓库结构

```text
SKILL.md
agents/openai.yaml
assets/video-script-package-template.html
references/
  clock-theory.md
  context-intake-and-source-use.md
  creator-production-system.md
  human-voice-and-editorial-audit.md
  ideation-packaging-and-titles.md
  output-specs-and-qc.md
  product-script-taxonomy.md
  story-script-and-spoken-copy.md
  timing-pacing-and-retention.md
```

## 输出原则

最终默认只交付一个 HTML 文件。它的主表是拍摄和剪辑的执行依据：每行有明确时间、逐字台词、画面动作、素材 ID、声音/剪辑提示。拍摄清单里的素材 ID 必须能被时间轴引用，避免“脚本写了但不知道拍什么”。

模板保持离线可用，保留可视化时钟节拍器，并提供完成勾选、未完成筛选、打印、重置和生成简化拍摄 PNG 等减少行动成本的交互。复杂的内部推理不塞进最终界面；对用户有用的判断、证据和修改动作才会展示。

## 边界与来源

- 这是一个辅助创作的 Skill，不是自动生成好视频的按钮。高质量结果依赖真实素材、产品事实、观众信息、创作者声音和持续的人机交互。
- HKRR 和 12 点时钟用于设计与诊断，不替代创作者的判断，也不要求每个刺激点都新增一句解释。
- 本项目与影视飓风、Tim 或 Beav 没有官方关联，也不代表其立场或获得其背书。
- 工作流中关于内容流程、检查和素材组织的部分参考并独立改写了 [dbskill](https://github.com/dontbesilent2025/dbskill) 的公开方法。相关改编内容保留署名，并按仓库中的 [CC BY-NC 4.0](LICENSE) 发布；请阅读许可证后再用于商业项目。

## 许可证

本项目使用 [Creative Commons Attribution-NonCommercial 4.0 International](LICENSE)。商业使用、再分发或大规模改编前，请先确认许可证条件和上游来源要求。
