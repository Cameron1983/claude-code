# 分镜头剧本输出模板 (Storyboard Output Format)

## 表格模板

```
场次：1 - INT. 老旧公寓客厅 - 夜

| 镜号 | 景别 | 机位/角度 | 运镜 | 焦段 | 画面内容 | 台词/音效 | 时长 | 转场 |
|---|---|---|---|---|---|---|---|---|
| 1-1 | 远景 | 平视 | 固定 | 广角 | 昏暗客厅，唯一光源来自窗外霓虹，男人背对镜头站立 | 环境音：雨声、远处车流 | 4s | 切 |
| 1-2 | 中景 | 平视 | 缓慢推近 | 标准 | 男人转身，露出疲惫神情，手里拿着一张照片 | (无台词) | 5s | 切 |
| 1-3 | 特写 | 平视 | 固定 | 中长焦 | 照片特写，边缘已经磨损，画面泛黄 | 音乐：低沉钢琴 | 3s | 叠化 |
```

## 每镜头附带的视频生成提示词区块

在表格之后，为每个镜头附上可直接使用的提示词（中英双语），格式：

```
【镜头 1-1】
中文提示词：昏暗的老旧公寓客厅，远景固定镜头，唯一光源来自窗外霓虹灯透入，一名男子背对镜头站立，雨夜氛围，黑色电影风格，低调布光，高对比阴影。
English: A dim old apartment living room, wide static shot, the only light source is neon glow through the window, a man stands with his back to camera, rainy night atmosphere, film noir style, low-key lighting, high-contrast shadows. 4 seconds, 16:9.

【镜头 1-2】
中文提示词：中景镜头缓慢推近，男子转身露出疲惫神情，手中拿着一张泛黄照片，标准镜头视角，延续黑色电影低调布光与高对比阴影。
English: Medium shot, camera slowly dollies in as the man turns to reveal a weary expression, holding a faded photograph, standard lens perspective, continuing the film-noir low-key lighting and high-contrast shadows. 5 seconds, 16:9.
```

## 完整分镜头剧本的段落结构建议

1. **项目信息**：标题、目标平台、总时长、整体视觉风格（引用 `cinematic-styles.md` / `animation-styles.md` 中选定的关键词组合）。
2. **分场概览**：按场次列出场景大纲（一句话概括每场戏的目的/转折点）。
3. **逐场分镜表 + 提示词**：按 `场次 → 镜头表格 → 每镜头提示词` 的顺序输出，场与场之间用标题分隔。
4. **需人工确认事项清单**：连戏细节、可能触发平台内容政策的镜头、需要真实素材/授权的部分。

## 快速估算参考

| 时长目标 | 建议镜头数 | 平均单镜时长 |
|---|---|---|
| 15 秒（社媒广告） | 4–6 个 | 2.5–4s |
| 30 秒（短广告/预告） | 6–10 个 | 3–5s |
| 60 秒（短片/MV 片段） | 10–18 个 | 3–6s |
| 2–3 分钟（短片） | 20–40 个 | 4–8s |

以上仅为经验参考，实际镜头数量应服务于叙事节奏，动作/冲突场景镜头更短更密集，情绪/氛围场景镜头可适当拉长。
