# 📊 MediaScope - 媒体分析工具

> 一个纯前端的图片和音频分析工具，支持详细的文件属性检测、波形可视化等功能

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Web Audio API](https://img.shields.io/badge/Web%20Audio%20API-FF6B6B?logo=google-chrome&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)

**GitHub 仓库**: [Links17/mediascope](https://github.com/Links17/mediascope)

## 📖 项目简介

MediaScope 是一个功能强大的媒体文件分析工具，完全在浏览器中运行，无需服务器支持。它可以深入分析图片和音频文件的各项属性，帮助用户了解文件的详细技术信息。

### 主要优势

- 🔒 **完全隐私**：所有文件处理都在本地浏览器完成，不会上传到任何服务器
- 🚀 **即开即用**：无需安装，无需配置，打开即用
- 📱 **跨平台**：支持所有现代浏览器，包括桌面和移动设备
- 🎯 **功能全面**：支持图片和音频的深度分析
- 💡 **易于使用**：直观的界面，拖拽即可使用

## ✨ 功能特性

### 🖼️ 图片分析

- ✅ **文件信息检测**：文件类型、大小、尺寸、宽高比、像素总数
- ✅ **颜色分析**：位深（24位/32位）、颜色模式（RGB/灰度/Alpha通道）
- ✅ **灰度级别检测**：自动识别1位到8位灰度级别
- ✅ **抖动算法识别**：支持检测2色、4色、6色、8色、16色等抖动算法
- ✅ **压缩算法识别**：JPEG、PNG、GIF、WebP、LZW等压缩格式识别
- ✅ **图片预览**：实时预览上传的图片

### 🎵 音频分析

- ✅ **音频信息**：文件类型、大小、时长、采样率、位深、声道数
- ✅ **频率分析**：主要频率、频率范围、奈奎斯特频率
- ✅ **波形可视化**：实时绘制音频波形图
- ✅ **音频播放**：内置播放器，支持试听
- ✅ **采样点统计**：显示总采样点数

### 🎨 界面特性

- ✅ **左侧菜单导航**：清晰的菜单结构
- ✅ **拖拽上传**：支持点击和拖拽两种上传方式
- ✅ **响应式设计**：适配桌面和移动设备
- ✅ **纯前端实现**：无需服务器，所有处理在浏览器本地完成
- ✅ **隐私安全**：文件不会上传到任何服务器

## 🚀 快速开始

### 方法一：直接使用（推荐，最简单）

1. 克隆或下载本项目到本地
2. 直接用浏览器打开 `index.html` 文件即可使用

```bash
# 克隆仓库
git clone git@github.com:Links17/mediascope.git

# 进入项目目录
cd mediascope

# 直接用浏览器打开 index.html 文件
# macOS: open index.html
# Windows: 双击 index.html
# Linux: xdg-open index.html
```

> ⚠️ **注意**：某些浏览器可能因为安全策略限制，直接打开 HTML 文件时部分功能可能无法使用。如果遇到问题，请使用方法二（本地服务器）。

### 方法二：本地服务器（推荐，功能完整）

如果直接打开 HTML 文件遇到问题，可以使用本地服务器运行。

#### 使用 Python（推荐）

```bash
# Python 3
python -m http.server 8000

# 然后在浏览器访问 http://localhost:8000
```

#### 使用 Node.js

```bash
# 安装 http-server（如果还没安装）
npm install -g http-server

# 启动服务器
http-server

# 访问终端显示的地址（通常是 http://localhost:8080）
```

#### 使用 PHP

```bash
# 启动 PHP 内置服务器
php -S localhost:8000

# 然后在浏览器访问 http://localhost:8000
```

#### 使用 VS Code Live Server

如果你使用 VS Code，可以安装 "Live Server" 扩展，然后右键点击 `index.html` 选择 "Open with Live Server"。

## 📖 使用说明

### 图片分析

1. 点击左侧菜单的"图片分析"
2. 点击上传区域或直接拖拽图片文件
3. 工具会自动分析并显示：
   - 文件类型、大小、尺寸
   - 颜色模式（RGB/灰度）
   - 位深信息
   - 抖动算法（如6色抖动）
   - 压缩算法

### 音频分析

1. 点击左侧菜单的"音频分析"
2. 上传或拖拽音频文件
3. 工具会显示：
   - 音频基本信息
   - 频率分析结果
   - 波形图可视化
   - 内置播放器可试听

## 📁 支持的格式

### 图片格式

| 格式 | 支持 | 说明 |
|------|------|------|
| JPEG/JPG | ✅ | 完全支持 |
| PNG | ✅ | 完全支持，包括透明度 |
| GIF | ✅ | 完全支持 |
| WebP | ✅ | 完全支持 |
| BMP | ✅ | 完全支持 |
| SVG | ✅ | 基本支持 |
| ICO | ✅ | 基本支持 |
| TIFF | ✅ | 基本支持 |

### 音频格式

| 格式 | 支持 | 说明 |
|------|------|------|
| MP3 | ✅ | 完全支持 |
| WAV | ✅ | 完全支持 |
| OGG | ✅ | 完全支持 |
| AAC | ✅ | 完全支持 |
| M4A | ✅ | 完全支持 |
| FLAC | ⚠️ | 部分浏览器支持 |
| WMA | ⚠️ | 部分浏览器支持 |
| Opus | ✅ | 完全支持 |

## 🛠️ 技术栈

### 核心技术

- **HTML5 File API** - 文件读取和处理
- **Canvas API** - 图片像素分析和波形绘制
- **Web Audio API** - 音频解码和频率分析
- **FileReader API** - 文件数据转换

### 技术特点

- 纯前端实现，无需后端
- 零依赖，单文件即可运行
- 支持现代浏览器（Chrome、Firefox、Safari、Edge）
- 响应式设计，适配移动端

## 📐 项目结构

```
mediascope/
├── index.html          # 主文件（包含HTML、CSS、JavaScript）
├── README.md          # 项目说明文档
├── LICENSE            # MIT许可证
└── .gitignore         # Git忽略文件
```

## 🔍 功能详解

### 抖动算法检测

工具可以自动识别图片使用的抖动算法：

- **2色抖动** - 仅使用2种颜色
- **4色抖动** - 使用3-4种颜色
- **6色抖动** - 使用5-6种颜色
- **8色抖动** - 使用7-8种颜色
- **16色抖动** - 使用9-16种颜色
- **32色抖动** - 使用17-32种颜色
- **64色抖动** - 使用33-64种颜色
- **128色抖动** - 使用65-128种颜色
- **256色** - 使用129-256种颜色（可能是抖动或调色板）

### 灰度级别检测

自动识别灰度图的位深级别：

- **1位灰度** = 2级（纯黑白）
- **2位灰度** = 4级
- **4位灰度** = 16级
- **8位灰度** = 256级（最常见）

## ⚙️ 浏览器兼容性

| 浏览器 | 版本要求 | 图片分析 | 音频分析 |
|--------|---------|---------|---------|
| Chrome | 60+ | ✅ | ✅ |
| Firefox | 55+ | ✅ | ✅ |
| Safari | 11+ | ✅ | ✅ |
| Edge | 79+ | ✅ | ✅ |
| Opera | 47+ | ✅ | ✅ |

## ⚠️ 注意事项

1. **文件大小限制**：建议分析小于50MB的文件，具体限制取决于浏览器
2. **隐私安全**：所有文件处理都在本地浏览器完成，不会上传到服务器
3. **位深检测**：由于浏览器Canvas API的限制，位深检测可能不是100%准确
4. **音频格式**：不同浏览器对音频格式支持不同，建议使用MP3或WAV格式
5. **频率分析**：使用简化的算法，对于复杂音频可能不够精确

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！你的贡献会让这个项目变得更好。

### 如何贡献

1. **Fork 本项目** - 点击 GitHub 页面右上角的 Fork 按钮
2. **克隆你的 Fork** - `git clone git@github.com:你的用户名/mediascope.git`
3. **创建特性分支** - `git checkout -b feature/你的功能名称`
4. **提交更改** - `git commit -m '添加了某个功能'`
5. **推送到分支** - `git push origin feature/你的功能名称`
6. **开启 Pull Request** - 在 GitHub 上提交 PR，我们会尽快 review

### 贡献类型

- 🐛 报告 Bug
- ✨ 提出新功能建议
- 📝 改进文档
- 🎨 优化界面
- ⚡ 性能优化
- 🔧 代码重构

## 📝 更新日志

### v2.1.0 (2024)
- ✨ 新增抖动算法检测功能（支持2色、4色、6色、8色等）
- 🎨 优化界面布局，改为左侧菜单导航
- 🐛 修复图片分析功能
- 📱 改进响应式设计

### v2.0.0 (2024)
- ✨ 新增音频分析功能
- ✨ 支持音频波形图绘制
- ✨ 支持频率分析
- ✨ 内置音频播放器
- 🎨 添加Tab切换界面

### v1.0.0 (2024)
- 🎉 初始版本发布
- ✨ 支持基础图片信息分析
- ✨ 支持拖拽上传
- 🎨 现代化UI设计

## ❓ 常见问题

### Q: 为什么某些图片的位深显示不准确？

A: 浏览器的Canvas API会将所有图片转换为标准格式（通常是RGBA），因此原始位深信息可能会丢失。工具会尝试通过分析像素数据来推断位深。

### Q: 可以分析网络图片吗？

A: 当前版本只支持本地文件。如果需要分析网络图片，需要先将图片下载到本地。

### Q: 支持哪些浏览器？

A: 支持所有现代浏览器，包括Chrome、Firefox、Safari、Edge等。音频分析功能需要浏览器支持Web Audio API。

### Q: 为什么音频频率分析不够准确？

A: 当前版本使用简化的频率分析方法（零交叉点分析），主要用于估算。如果需要更精确的频率分析，可以使用专业的音频分析工具。

### Q: 如何检测6色抖动？

A: 上传使用6色抖动的图片，工具会自动识别并在"颜色模式"中显示"RGB (6色抖动)"或类似信息。

## 🔗 相关链接

- **GitHub 仓库**: [Links17/mediascope](https://github.com/Links17/mediascope)
- **问题反馈**: [Issues](https://github.com/Links17/mediascope/issues)
- **功能建议**: [Feature Requests](https://github.com/Links17/mediascope/issues/new)

## 📄 许可证

本项目采用 [MIT License](LICENSE) 许可证。

---

**Made with ❤️ by Links17**

如果这个项目对你有帮助，欢迎给个 ⭐ Star！