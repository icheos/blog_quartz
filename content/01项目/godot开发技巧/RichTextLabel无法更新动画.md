---
publish: true
enableToc: true
created: 2026-03-18T16:55:31.144+08:00
modified: 2026-07-25T00:00:24.438+08:00
tags:
  - godot
  - 小技巧
---

![](01项目/godot开发技巧/assets/RichTextLabel无法更新动画/file-20260318170059089.gif)

字体消失了！！

原因是因为当为RichTextLabel添加重复文本不会对文本内容进行更新，导致文本在播放时没有更新动画

## 解决方法

添加重复文本时将RichTextLabel中的text设置为空，让其不再以重复文本进行播放动画

![](01项目/godot开发技巧/assets/RichTextLabel无法更新动画/file-20260724235622442.png)
