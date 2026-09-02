# 动画风格关键词库 (Animation Styles)

用于非写实/动画类分镜的视频生成提示词。可与 `cinematic-styles.md` 中的光影、构图术语组合使用（动画同样需要景别、运镜、构图设计）。

| 风格标签 | 关键词组合 | 特征 |
|---|---|---|
| 吉卜力手绘感 | Studio Ghibli style, hand-painted watercolor backgrounds, soft lighting, whimsical, lush nature detail | 水彩感背景、柔和光线、自然细节丰富 |
| 皮克斯/迪士尼 3D | Pixar-style 3D animation, soft global illumination, expressive character rigging, vibrant saturated colors | 圆润角色造型、柔和全局光、高饱和 |
| 日系赛璐璐动画 | Japanese anime cel-shaded style, sharp line art, flat cel shading, dynamic speed lines | 锐利线稿、平涂阴影、动态速度线 |
| 新海诚式唯美光影 | hyper-detailed anime background, dramatic sky, lens flare, glowing light rays, emotional atmosphere | 极致背景细节、戏剧性天空、光晕 |
| 定格动画 (stop-motion) | stop-motion animation, claymation texture, visible fingerprints on clay, handcrafted felt and fabric look | 黏土质感、手工痕迹、逐帧定格感 |
| 剪纸/纸偶风 | paper cutout animation, layered paper texture, flat 2D silhouette style | 分层纸片质感、平面剪影 |
| 像素风 | pixel art style, 8-bit/16-bit retro game aesthetic, limited color palette | 复古游戏像素颗粒 |
| 水墨风 | Chinese ink wash painting style, flowing brush strokes, minimalist negative space, monochrome ink gradients | 水墨晕染、留白、单色渐变 |
| 剪影风格 | silhouette animation, high-contrast backlit shapes, minimal flat color background | 高对比逆光剪影 |
| 低多边形 (low poly) | low-poly 3D style, geometric faceted shapes, flat shading | 几何切面、极简多边形 |
| 蒸汽波/故障艺术 | vaporwave aesthetic, glitch art, VHS scanlines, chromatic distortion | 复古故障、扫描线、色差 |
| 涂鸦/手账风 | doodle animation, sketchbook line art, hand-drawn scribble texture, notebook paper background | 手绘涂鸦、素描线条 |
| 黏土 claymation 特写质感 | macro claymation texture, visible tool marks, tactile stop-motion surface | 强调材质触感的黏土特写 |
| 赛博未来插画风 | flat vector illustration, cyber-futuristic color scheme, geometric minimal shapes | 扁平矢量、几何极简、未来配色 |
| 水彩童话风 | watercolor storybook illustration, soft edges, pastel wash, dreamy fairy tale atmosphere | 柔边水彩、童话梦幻 |

## 动画特有的镜头/运动设计要点

- 动画运镜可以比实拍更夸张（弧线运镜、变形挤压 squash-and-stretch、速度线），但仍需遵守景别与构图基本法则以保证叙事清晰。
- 明确角色设计的一致性描述（体型比例、配色、服装细节），并在每个镜头提示词中重复关键特征词，避免多镜头间角色形象漂移（AI 视频生成的常见问题）。
- 二维赛璐璐风格建议加 `flat shading, clean line art, no 3D rendering` 等词，避免模型默认输出 3D 质感。
- 定格/黏土风格建议加 `slight stop-motion jitter, 12fps` 等词强化"逐帧感"，否则容易被生成为平滑的普通 3D 动画。
- 如果目标是"电影感真人 + 动画元素混合"（如实拍人物+2D 特效），需在提示词中同时给出实拍摄影关键词（见 `cinematic-styles.md`）与动画元素描述，并说明二者的合成关系。
