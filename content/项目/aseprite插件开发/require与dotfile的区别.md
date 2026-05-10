---
publish: true
enableToc: true
created: 2026-04-11T15:52:44.673+08:00
modified: 2026-04-11T15:57:46.080+08:00
tags:
  - lua
  - 插件开发
cssclasses: ""
---

在学习别人的插件时发现别人写插件使用的dotfile而不是require，故学习两者区别

| 特征       | require("module")                   | dofile("path/to/file.lua")              |
| -------- | ----------------------------------- | --------------------------------------- |
| **搜索路径** | 用途`package.path`（例如，在`lua/`文件夹中查找）。 | 需要提供文件的实际路径。                            |
| **缓存**   | 文件只加载**一次**；后续调用返回缓存的结果。            | **每次**调用时都会重新加载并重新执行该文件。                |
| **句法**   | 使用点：`require("config.options")`     | 使用斜杠：`dofile("lua/config/options.lua")` |
