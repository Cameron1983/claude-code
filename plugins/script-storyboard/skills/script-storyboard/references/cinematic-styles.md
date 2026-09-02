# 电影/摄影风格关键词库 (Cinematic Styles)

用于在视频生成提示词中统一全片视觉基调。选定后应贯穿所有镜头的提示词，保持光影逻辑、色彩基调、质感一致。

## 一、导演/摄影风格参考（可直接作为提示词关键词或灵感描述，不直接使用真人姓名生成肖像）

| 风格标签 | 关键词组合 | 视觉特征 |
|---|---|---|
| 诺兰式 IMAX 实景感 | IMAX 70mm film look, large-format, natural lighting, epic scale, minimal CGI feel | 大画幅、实景质感、宏大但克制 |
| 韦斯·安德森式 | symmetrical composition, pastel color palette, flat frontal framing, whimsical production design | 对称构图、粉彩色调、正面平视构图 |
| 昆汀式 | saturated colors, low-angle hero shots, retro grindhouse film grain, sharp dialogue framing | 高饱和、仰拍英雄视角、复古颗粒感 |
| 黑色电影 (film noir) | high-contrast lighting, hard shadows, venetian blind shadows, low-key lighting, monochrome or desaturated | 强对比硬光、百叶窗光影、低调布光 |
| 王家卫式都市感 | saturated neon colors, slow motion, handheld intimacy, step-printing motion blur, rain-soaked streets | 霓虹饱和色、慢动作、手持亲密感 |
| 赛博朋克 | neon-lit rain-soaked streets, holographic signage, blade-runner atmosphere, cyan-magenta color grade | 霓虹雨夜、全息广告、青品色调 |
| 末日废土风 | desaturated dusty palette, harsh sunlight, overexposed sky, gritty texture, sand and rust tones | 低饱和沙尘色、强烈日光、粗粝质感 |
| 复古胶片感 | 35mm film grain, warm halation, vignette, slightly faded colors, light leaks | 胶片颗粒、暖色光晕、褪色感 |
| 极简高级感广告 | clean minimalist studio lighting, soft shadows, single color background, premium product photography look | 干净影棚光、极简背景、高级质感 |
| 纪录片写实风 | documentary style, natural available light, observational handheld camera, muted realistic color | 自然光、旁观式手持、克制色彩 |
| 宫崎骏电影感真人版 | soft natural light, lush green landscapes, warm nostalgic tone, gentle wind motion | 柔和自然光、翠绿景观、温暖怀旧 |
| 惊悚悬疑感 | cold blue color grade, deep shadows, tight framing, unsettling silence, dutch angle | 冷蓝调、深阴影、逼仄构图 |

## 二、光影风格 (Lighting)

| 关键词 | 效果 |
|---|---|
| golden hour lighting | 日出日落暖金色光，柔和且富电影感，人像/风光首选 |
| blue hour | 日落后的深蓝天光，忧郁静谧 |
| high-key lighting | 明亮均匀少阴影，轻松/商业/喜剧基调 |
| low-key lighting | 大面积阴影强对比，紧张/悬疑/戏剧化 |
| Rembrandt lighting | 人像三角光斑，经典肖像用光 |
| backlighting / rim light | 逆光/轮廓光，勾勒主体边缘，梦幻或神秘感 |
| practical lights | 画面内实际光源（台灯、霓虹灯牌）营造真实感 |
| volumetric light / god rays | 丁达尔光束，穿透烟雾/云层，神圣或空间感 |
| hard light / soft light | 硬光边缘锐利有戏剧性；柔光过渡柔和自然 |
| silhouette lighting | 剪影逆光，强调形态与情绪而非细节 |

## 三、色彩分级 (Color Grading)

| 关键词 | 情绪基调 |
|---|---|
| teal and orange color grade | 好莱坞商业片经典冷暖对比色调 |
| desaturated muted tones | 沉重、写实、压抑 |
| warm amber tones | 怀旧、温馨、安全感 |
| cool blue/cyan tones | 冷峻、孤独、科技感 |
| high saturation vivid colors | 活力、奇幻、儿童向 |
| monochrome / black and white | 经典、严肃、回忆/闪回 |
| pastel color palette | 柔和梦幻、童话感 |
| high contrast dramatic grade | 紧张、力量感、动作片 |

## 四、质感与后期 (Texture)

- `35mm film grain` / `16mm grainy texture`：胶片颗粒感，增强复古与情感质地。
- `anamorphic lens flare`：变形宽银幕镜头耀光，横向拉长的光斑，强电影感。
- `motion blur`：动作模糊，增强速度感。
- `shallow depth of field, bokeh background`：浅景深虚化，突出主体的电影质感标配。
- `chromatic aberration`：轻微色差，增加真实光学质感。
- `slow motion, 120fps`：慢动作，强调关键瞬间的仪式感/冲击力。

## 使用建议

在提示词中按"整体基调 + 光影 + 色彩 + 质感"的顺序组合 2–4 个关键词即可，避免堆砌过多互相矛盾的风格标签（例如同时写 high-key 与 low-key）。全片所有镜头应共用同一套核心风格词，仅按场景情绪微调（例如高潮戏切换为 low-key + cool tones）。
