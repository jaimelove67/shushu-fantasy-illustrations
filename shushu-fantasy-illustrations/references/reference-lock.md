# 参考图硬约束

当生成结果和参考图不符时，优先读取本文件并重写提示词。

## 参考图共同特征

- 不是普通“可爱鼠鼠插画”，而是表情包拼贴。
- 鼠鼠头是照片质感：低清、灰褐/灰绿、毛绒、略糊、像从素材里剪下来。
- 鼠鼠身体是手绘质感：白色布袋/团子形，黑色粗描边，短手短脚。
- 头和身体不是同一画风，必须有明显拼贴违和感。
- 表情核心是怪异白牙笑或害羞腮红，不是正常萌宠表情。
- 幻想云是手绘云团：白底、黑/深棕粗线、重复描线、线条不干净。
- 云泡泡内容像“脑内小剧场”，不是正式漫画、海报或解释图。
- 核心幻想不靠文字直说。名人、职业、暴富、毕业、冠军等幻想要靠道具、服装、编号、场景和姿态表达。

## 三张参考图的用途

- `assets/examples/02-coin-fantasy-template.png`：最重要。用于锁定白底模板、鼠鼠头身比例、大牙笑、云泡泡线条。
- `assets/examples/01-park-camera-fantasy.png`：用于锁定真实户外照片 + 前景鼠鼠贴纸 + 右上幻想云的关系。
- `assets/examples/03-lab-presentation-fantasy.png`：用于锁定室内真实照片 + 多个鼠鼠贴纸 + 多个幻想云的关系。

## 生成策略

图像工具支持参考图输入时：

1. 白底模板任务：附带 `02-coin-fantasy-template.png`。
2. 真实照片叠加任务：附带用户照片 + `02-coin-fantasy-template.png`，必要时再附带 `01` 或 `03`。
3. 多鼠鼠任务：附带 `03-lab-presentation-fantasy.png`。

图像工具不支持参考图输入时，提示词必须写明：

```text
The shushu must be constructed like the reference: a low-resolution pasted photographic gray-brown furry animal head attached to a separate white hand-drawn blob body with thick black uneven outline. The head and body must not share one clean illustration style.
```

## 最常见偏差与修正

- 偏差：生成成可爱卡通仓鼠。
  修正：强调 cropped low-resolution photographic animal head, awkward toothy grin, not a cute cartoon hamster。

- 偏差：全身统一画风。
  修正：强调 mixed-media collage, photo head plus doodle body, visibly pasted together。

- 偏差：画得太精致。
  修正：强调 rough phone edit, low-effort Douyin meme, uneven thick black outline, slightly jagged edges。

- 偏差：幻想云太像漫画对话框。
  修正：强调 irregular white thought cloud, rough repeated black/dark-brown sketch strokes, 2-3 small bubbles。

- 偏差：不像参考图的牙齿笑。
  修正：强调 exaggerated awkward white human-like toothy grin, slightly uncanny meme smile。

- 偏差：图上写出“我是某某 / 我发财了 / 我是冠军”。
  修正：删除解释性文字，用视觉符号表达身份和愿望，只保留可选的“嘿嘿/OAO”情绪字。
