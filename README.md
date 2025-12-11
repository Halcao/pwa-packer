# 📦 Gemini PWA Packer

> **Turn your Gemini Canvas prototypes into installable Apps in seconds.**
>
> 🚀 **Live Demo:** [点击这里使用工具](https://lifeauto.vercel.app)

这是一个纯前端工具，旨在配合 **Google Gemini Canvas** 使用。它可以自动解析 Gemini 生成的 HTML 代码，提取其中“休眠”的 PWA 配置（Manifest & Service Worker），并将其自动注入、激活，最终打包成一个可直接部署的 ZIP 文件。

## ✨ 核心功能

*   **⚡️ 自动提取**：从 HTML 的 `<script type="text/file">` 标签中提取 `manifest.json` 和 `sw.js`。
*   **💉 智能注入**：自动在 `index.html` 中插入 `<link rel="manifest">` 和 Service Worker 注册代码。
*   **🛡 零干扰预览**：配合特定的 Prompt，Gemini 生成的预览页面不会有 404 报错。
*   **📦 一键打包**：生成标准的 ZIP 包，解压后即可上传至 GitHub Pages 或 Vercel。

## 📖 使用指南 (Workflow)

### 第一步：让 Gemini 生成代码
在 Gemini Canvas 中生成网页时，请**务必**使用以下 Prompt。

**复制 Prompt 给 Gemini：**


### 第二步：使用本工具打包
1. 复制 Gemini 生成的完整 HTML 代码。
2. 打开 [Gemini PWA Packer](https://lifeauto.vercel.app)。
3. 粘贴代码，点击 **"Extract & Download ZIP"**。

### 第三步：部署
1. 解压下载的 ZIP 文件。
2. 将所有文件上传到 GitHub 仓库或 Vercel。
3. 你的网页现在就是一个可安装的 PWA 应用了！📱

## 🛠 技术栈

*   HTML5 / JavaScript (Vanilla)
*   Tailwind CSS (UI Styling)
*   JSZip (File Bundling)

## 🤝 贡献

欢迎提交 Issue 或 PR 来改进提取逻辑！

## 📄 License

MIT License