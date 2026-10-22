# High Retention Video Script

一个面向真实创作者的视频脚本 Skill：先理解观众要完成什么，再选择合适的视频结构，最后用 HKRR 和 12 点刺激时钟把内容落成可拍、可剪、可检查的脚本。

> **理论来源**：本 Skill 的理论来源是影视飓风公开内容中讲解的 HKRR 理论和时钟理论。本仓库将这套方法整理为可被 AI 调用、可被创作者复核、可以直接指导拍摄与剪辑的工作流。

## 它解决什么问题

这个 Skill 不把每条视频都写成同一种“故事”，也不把产品介绍拆成机械的功能清单。它会根据视频任务选择结构：

- 工具介绍和操作教程：先展示结果，再解释产品、输入、操作、输出和边界。
- 发布、教育、测评、案例和创作者内容：分别匹配揭示、讲解、比较、实验或观点结构。
- 从用户提供的素材、旧稿、录屏、评论、参考视频、知识库文件和说话样本中整理事实、证据、声音和限制。
- 先写能读出口的真人初稿，再用 HKRR 和 12 点刺激时钟做设计与质检。
- 交付一个离线 HTML，按真实拍摄顺序分成三页：逐字稿（带提词器）、拍摄清单（按机位一次录完）、节奏（HKRR 与 12 点时钟）。

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

最终默认只交付一个 HTML 文件。模板只有一个 JSON 数据块，AI 只填数据，页面上的开头 3 秒、逐字稿、拍摄卡片、HKRR、时钟、A/B 轨道、提词器和拍摄单图片都由这份数据渲染，同一件事只写一次，不会前后不一致。

页面按创作者真实的使用顺序排：

1. **逐字稿**：先出声读一遍，读着别扭就改；提词器全屏滚动，可调速、可镜像。
2. **拍摄**：按机位分组，口播卡片里列出这个机位要说的所有台词，一次录完；每张卡片写清起→拍→止、景别和合格标准，拍完勾选。
3. **节奏**：HKRR 四张卡、12 点刺激时钟、按时长比例的 A/B 轨道、开拍前检查。

页面离线可用，跟随系统浅色 / 深色，手机上同样好用；可以打印成 PDF，也能生成一张拍摄单图片带去现场。数据有遗漏时（镜头 ID 找不到、时间接不上、时钟不满 12 个点等），页面顶部会直接提示。

## 边界与来源

- 这是一个辅助创作的 Skill，不是自动生成好视频的按钮。高质量结果依赖真实素材、产品事实、观众信息、创作者声音和持续的人机交互。
- 本 Skill 的理论起点来自影视飓风公开内容中的 HKRR 理论和时钟理论；仓库中的流程、提示和模板是独立整理与实现。
- `references/mediastorm-observed-patterns.md` 整理了影视飓风已发布视频中可观察到的写法（开头钩子类型、提升立意、论点单元、自问自答节奏、长视频拆成短视频链、升华四步、点映），参考了两个 MIT 许可的社区分析项目 [imfangli/mediastorm-copywriter](https://github.com/imfangli/mediastorm-copywriter) 与 [phaseddd/PhasedddSkill 的 tim-mediastorm](https://github.com/phaseddd/PhasedddSkill/tree/main/tim-mediastorm)，内容为我们自己的整理和改写。截至 2026-10-22 未找到影视飓风官方发布的脚本 Skill。
- HKRR 和 12 点时钟用于设计与诊断，不替代创作者的判断，也不要求每个刺激点都新增一句解释。
- 本项目与影视飓风、Tim 或 Beav 没有官方关联，也不代表其立场或获得其背书。
- 工作流中关于内容流程、检查和素材组织的部分参考并独立改写了 [dbskill](https://github.com/dontbesilent2025/dbskill) 的公开方法。相关改编内容保留署名，并按仓库中的 [CC BY-NC 4.0](LICENSE) 发布；请阅读许可证后再用于商业项目。

## 许可证

本项目使用 [Creative Commons Attribution-NonCommercial 4.0 International](LICENSE)。商业使用、再分发或大规模改编前，请先确认许可证条件和上游来源要求。

## Skill

这是一个把影视飓风的 HKRR 理论与时钟理论整理为可执行视频脚本工作流的 Skill
