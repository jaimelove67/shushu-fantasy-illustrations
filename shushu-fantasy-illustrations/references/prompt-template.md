# 提示词模板

每张图单独生成。根据用户主题替换变量，不要把多张拼成一张。

## 新图生成

```text
Create one meme-style Chinese social media image that closely follows the provided shushu fantasy reference images.

Reference matching priority:
1. Match the reference character construction: a low-resolution pasted photographic gray-brown animal head + a separate white hand-drawn blob body.
2. Match the rough phone-edit collage feeling. It must look manually pasted, not professionally illustrated.
3. Match the thought cloud: white cloud bubble, rough black/dark-brown repeated doodle outlines, small bubbles connecting from the head.
4. Match the awkward toothy grin and slightly strange meme expression.
5. Do not reinterpret it as a clean cute mascot.

Scene:
{真实背景或白底模板描述}

Main character:
One rough pasted shushu meme character. The head must look like a cropped low-resolution photographic gray-brown furry animal head, slightly blurry and flattened, with tiny dark eyes and an exaggerated awkward white toothy grin. The body must be a separate simple white doodle blob/bag shape with thick black uneven hand-drawn outline and tiny short limbs. The head and body should visibly feel composited from different sources, like a low-effort Douyin phone edit.

Fantasy bubble:
Add a large white hand-drawn thought cloud above or beside the shushu, connected by 2-3 small bubbles. The cloud has rough black/dark-brown doodle outlines with repeated sketch strokes. Inside the cloud, show {幻想内容}. Keep it simple and instantly readable.

Composition:
Place the shushu at {鼠鼠位置}. Place the fantasy cloud at {泡泡位置}. Preserve enough background context. The fantasy cloud should occupy about 25%-45% of the image, and should not cover important people, screens, or objects.

Text:
Default: no explanatory text. If text is needed, use only tiny emotional meme sounds such as “嘿嘿”, “嘻嘻”, or “OAO”. Do not write the identity or fantasy directly. For example, do not write “我是汉密尔顿”, “我发财了”, “我是冠军”, or “我毕业了”. The fantasy must be understood from visual symbols.

Style constraints:
Douyin meme collage, rough phone-edit feeling, pasted sticker edges, low-resolution photographic head, thick doodle outlines, white bubble, gray-brown shushu photo head, white doodle body, strange white toothy grin, awkward and funny, intentionally unpolished.

Hard negatives:
No unified illustration style. No cute cartoon hamster. No realistic full-body animal. No clean vector sticker. No polished mascot. No glossy 3D. No children's book style. No anime. No formal comic panel. No PPT infographic. No long explanatory text. No explanatory identity text such as “I am ...”. No dreamy gradient. No cyber effects. No natural anatomical mouse body.
```

## 真实照片改图

```text
Edit the provided photo. Preserve the original background, perspective, lighting, people, screens, and main objects.

Add one rough sticker-like shushu meme character at {位置}. The head must look like a pasted cropped low-resolution photographic gray-brown furry animal head with tiny dark eyes and an exaggerated awkward white toothy grin. The body must be a separate white hand-drawn blob body with thick black uneven outline and tiny limbs. The result should look intentionally pasted onto the photo like a Douyin meme edit, not naturally integrated.

Add a white hand-drawn thought cloud at {泡泡位置}, connected to the shushu by small bubbles. Inside the cloud, show {幻想内容}. Use rough black/dark-brown sketch outlines. Do not add explanatory text naming the fantasy. If any text is added, use only a tiny emotional sound like “嘿嘿” or “OAO”.

Keep the edit playful, low-effort, and meme-like. Do not repaint the whole photo. Do not make the shushu realistic. Do not make the character a unified illustration. Do not turn the result into a polished poster.
```

## 替换幻想内容

```text
Edit the provided image. Keep the original shushu character, background, composition, thought-cloud shape, hand-drawn outline style, and image quality.

Replace only the content inside the thought cloud with {新幻想内容}. Remove the old cloud content cleanly. Do not add explanatory identity/wish text. If a tiny text accent is necessary, use only “嘿嘿”, “嘻嘻”, or “OAO”. Do not move the shushu or change the background.
```
