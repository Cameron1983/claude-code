# Script Storyboard

将剧本、故事大纲或广告脚本拆解为专业分镜头剧本，并为每个镜头撰写可直接用于 AI 视频生成工具（Sora、Runway、可灵 Kling、Veo、Pika、Vidu、Luma 等）的提示词。

## 功能

- **剧本拆解**：把剧本按场次（Scene）、镜头（Shot）系统化拆分，输出标准分镜头表（镜号、景别、机位、运镜、焦段、画面内容、台词/音效、时长、转场）。
- **电影化镜头语言**：内置景别、机位角度、运镜方式、镜头焦段、构图法则、剪辑节奏的完整知识库，拆镜头时主动运用专业摄影术语服务叙事。
- **视觉风格关键词库**：涵盖写实电影/摄影风格（导演风格、光影、色彩分级、胶片质感）与动画风格（吉卜力、皮克斯 3D、赛璐璐、定格动画、水墨、像素风等），保证全片视觉一致性。
- **多平台提示词模板**：针对 Sora、Runway、可灵、Veo、Pika、Vidu、Luma 等主流 AI 视频生成平台的语法特点提供写作模板与要点。

## 内容

**Skill:** `script-storyboard` — 剧本转分镜头剧本与视频生成提示词设计流程，含以下参考资料：
- `references/shot-grammar.md` — 景别/机位/运镜/焦段/构图/剪辑节奏
- `references/cinematic-styles.md` — 电影/摄影风格与光影、色彩关键词库
- `references/animation-styles.md` — 动画/插画风格关键词库
- `references/prompt-templates.md` — 各视频生成平台提示词模板
- `references/storyboard-format.md` — 分镜头剧本输出表格模板与示例

## 使用

安装后直接向 Claude 描述剧本或创意点子，并说明目标平台与视觉风格（例如"帮我把这段剧本拆分镜头，走赛博朋克电影风格，投给可灵"），技能会自动触发。
