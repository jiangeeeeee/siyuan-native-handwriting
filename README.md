#源生笔迹

> 思源笔记的轻量化手写插件，支持正文批注与自由白板。

本仓库为源生笔迹[发行仓库](https://github.com/jiangeeeeee/siyuan-native-handwriting)。

**当前版本：** `0.14.4` · **思源笔记要求：** `3.8.4` 及以上


## ✨ 插件介绍

我的初中老师曾告诉我：**No pencil, No reading.**

我始终认为，只有真正拿起一支笔，才能沉下心来读一读、想一想。无论是阅读时随手写下的批注，还是灵光一闪时记录的想法，笔尖划过纸面的过程，本身就是思考的一部分。

步入 AI 时代，我们拥有了越来越多强大的数字化工具，但我依然希望保留这种最朴素的习惯：手握一支笔，在思源笔记中自由地阅读、批注、记录与思考。

于是，有了 **源生笔迹**。

这个插件绝大部分功能已经完善。我希望它能让思源笔记不仅是一个知识管理工具，也成为一个可以拿起笔来书写的数字空间。无论是在正文中圈画重点、记录批注，还是打开白板自由挥洒想法，都能让书写自然地融入知识整理与思考的过程。

> **让笔迹留在知识里，让思考不止于键盘。**

## ✨ 核心功能

### ✍️ 正文批注

**让笔迹直接融入阅读，而不是游离于笔记之外。**

阅读文献、整理资料时，直接在笔记正文上使用压感笔圈画重点、添加批注。不必在笔记软件与其他手写工具之间来回切换，让阅读与思考自然衔接。

### 📝 自由白板

**不受正文排版限制，让想法自由生长。**

打开独立白板，随手画图、推导公式、记录灵感。支持SiYuan双链，不受文字排版和页面结构的约束，让思考不再受输入方式限制。

## 版本与使用说明

当前 **0.14.4** 支持钢笔、马克笔和彩笔、精确擦除和笔画擦除、圈选移动与基础编辑、白板书写与缩放、输入切换、撤销重做及笔迹备份恢复。

Pro 提供铅笔、圈选擦除、选区换色与缩放、照片生成、图层、激光笔、白板插入与双链、PDF／HTML／SVG 导出、多指撤销重做和工具栏外观。

要求思源笔记 **3.8.4 或更高版本**。推荐使用支持触控笔及压感输入的设备，以获得更完整的书写体验。

> **开发说明：** 仓库中的授权管理服务目前仅用于内部开发。

## 项目结构

| 目录 | 用途 |
| --- | --- |
| [siyuan-native-handwriting](./siyuan-native-handwriting/README.md) | 插件源码、构建脚本、测试与使用说明。 |
| [siyuan-license-server](./siyuan-license-server/README.md) | Pro 激活与授权管理服务，包含本机运行和部署说明。 |

## 📦 安装包与构建

### 正式发布包

[获取 0.14.4 安装包](https://github.com/jiangeeeeee/siyuan-native-handwriting/releases/download/v0.14.4/package.zip) · [完整源码与校验值](./releases/0.14.4/README.md)

文件路径：`releases/0.14.4/package.zip`。

SHA-256：`6f13db80dae0d4df96beb541660ce3b9e848ef6541efc6be9f265a81458bd352`。

### 从源码构建

使用 **Node.js 26**、**pnpm 11** 和 **Python 3**，在仓库根目录打开终端并执行：

```bash
cd siyuan-native-handwriting
pnpm install --frozen-lockfile
pnpm run build
python3 scripts/package_plugin.py
```

构建后的安装包位于 `siyuan-native-handwriting/artifacts/siyuan-native-handwriting-0.14.4-account.zip`。

## 许可说明

本项目自有部分适用 [商业使用许可](./siyuan-native-handwriting/LICENSE)，并授权思源官方集市分发完整安装包。

[第三方组件](./siyuan-native-handwriting/THIRD_PARTY_NOTICES.md) 继续适用各自的原许可证。
