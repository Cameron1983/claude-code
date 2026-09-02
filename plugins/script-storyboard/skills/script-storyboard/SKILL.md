---
name: script-storyboard
description: This skill should be used when the user wants to break a script, screenplay, story outline, or ad brief down into a shot-by-shot storyboard (分镜头剧本/分镜表), and/or write AI video-generation prompts for each shot — covering shot size, camera movement, lens, lighting, composition, cinematic film-style or animation-style keywords, and platform-specific prompt syntax (e.g. Sora, Runway, Kling/可灵, Veo, Pika, Vidu, Luma). Trigger on requests like "把这个剧本拆分镜头", "写分镜表", "生成视频提示词", "storyboard this script", "shot list", "AI 视频生成提示词".
---

# 剧本分镜与 AI 视频生成提示词设计 (Script-to-Storyboard & Video Prompt Design)

将剧本/故事大纲/广告脚本拆解为专业分镜头剧本，并为每个镜头撰写可直接投喂给 AI 视频生成工具（Sora / Runway / 可灵 Kling / Veo / Pika / Vidu / Luma 等）的提示词。核心能力：镜头语言（景别、机位、运镜、焦段、构图）+ 电影/动画视觉风格关键词库 + 各平台提示词语法。

## 工作流程

### 1. 理解输入与产出目标
先明确：
- 输入是完整剧本、故事梗概，还是几句话的创意点子？如果只有点子，先帮用户扩写出场景/情节要点，再进入分镜。
- 成片时长与镜头数量级（例如 30 秒短片 ≈ 6–10 个镜头，2 分钟短片 ≈ 20–40 个镜头）。
- 目标平台（Sora2/Runway/可灵/Veo3/Pika/Vidu…），决定提示词语法与时长上限（多数平台单镜头 4–10 秒）。
- 整体视觉风格：写实电影感、动画风格，还是二者混合（例如"皮克斯风格 3D 动画 + 电影级布光"）。不确定就主动问用户，或给 2–3 个风格方向供选择。

### 2. 场景与情节切分
把剧本按"场景（Scene）"切分：地点、时间、场内动作变化处即切分点。每场标注 INT./EXT.、地点、时间（日/夜）。

### 3. 分镜拆解（场景 → 镜头）
每个场景内按"剪辑点"拆成镜头（Shot）：视角切换、动作节拍、情绪转折、对白轮次都是切镜信号。一场戏通常由建立镜头（establishing shot）+ 若干中近景/特写的正反打或动作分解组成，遵循 180 度轴线规则保持空间连贯。

给每个镜头填写以下字段（详见 `references/storyboard-format.md` 的表格模板）：

| 字段 | 说明 |
|---|---|
| 镜号 | 场号-镜号，如 1-3 |
| 景别 | 远/全/中/近/特写等，见 `references/shot-grammar.md` |
| 机位角度 | 平视/俯拍/仰拍/鸟瞰/荷兰角等 |
| 运镜 | 固定/推拉/摇/移/跟/升降/手持/无人机等 |
| 镜头焦段 | 广角/标准/长焦/微距，影响透视与压缩感 |
| 画面内容 | 主体、动作、构图要点 |
| 台词/音效/音乐 | 对白、环境音、配乐情绪 |
| 时长 | 秒数，需与目标平台单镜头上限匹配 |
| 转场 | 切/淡入淡出/叠化/匹配剪辑等 |

拆解时主动运用电影化分镜语言（见 `references/shot-grammar.md`）：用远景/大远景建立空间与规模，用中景承载对话与关系，用近景/特写强化情绪与关键道具，用运镜（推近=聚焦/紧张，拉远=揭示/孤立，摇/移=引导视线，跟拍=沉浸/动感，升降=权力/视野变化）服务叙事而非炫技。

### 4. 视觉风格设定
与用户确认或主动建议：
- **电影感风格**：参考 `references/cinematic-styles.md` 中的导演/摄影风格、色彩分级、光影关键词库（如"诺兰式 IMAX 实景感"、"韦斯·安德森对称构图+高饱和"、"黑色电影高对比侧光"、"赛博朋克霓虹雨夜"）。
- **动画风格**：参考 `references/animation-styles.md`（吉卜力手绘感、皮克斯 3D、日系赛璐璐、定格黏土、水墨风、像素风、剪纸风等）。
- 风格关键词要贯穿全片所有镜头提示词，保持视觉一致性（同一色调、同一光源逻辑、同一渲染质感）。

### 5. 撰写视频生成提示词
为每个镜头生成一条提示词，结构建议：**主体与动作 → 环境/背景 → 镜头语言（景别+运镜+机位）→ 光影与色彩 → 风格关键词 → 氛围/情绪词 → 技术参数（时长、画幅、帧率，若平台支持）**。

不同平台语法差异较大（自然语言 vs 参数化标签、是否支持镜头运动指令、是否支持首尾帧/参考图），撰写前查阅 `references/prompt-templates.md` 获取对应平台的模板与实例。默认给出中英双语提示词：中文便于用户理解和修改，英文提示词是多数生成模型效果更稳定的实际投喂版本。

### 6. 输出与迭代
- 用表格或分节列表输出完整分镜头剧本（模板见 `references/storyboard-format.md`），每个镜头紧跟其视频生成提示词。
- 主动标注需要人工确认的地方：连戏细节（服装/道具/时间连续性）、需要真人出镜或授权素材的镜头、平台时长/内容政策可能限制的镜头（暴力、真人肖像、版权角色等）。
- 用户可能要求"只改某几个镜头的风格/运镜"——只重写受影响镜头，不要整份重写。

## 参考资料

- `references/shot-grammar.md` — 景别、机位角度、运镜方式、焦段与构图法则（电影摄影机语言核心知识）
- `references/cinematic-styles.md` — 电影/摄影风格与色彩、光影关键词库
- `references/animation-styles.md` — 动画/插画风格关键词库
- `references/prompt-templates.md` — Sora / Runway / 可灵 Kling / Veo / Pika / Vidu / Luma 等平台提示词模板与写作要点
- `references/storyboard-format.md` — 分镜头剧本输出表格模板与完整示例
