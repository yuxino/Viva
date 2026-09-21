<p align="center">
  <img src="public/art/viva-character-logo-round.webp" width="136" height="136" alt="Viva 少女 Logo">
</p>

<h1 align="center">Viva</h1>

<p align="center"><a href="https://viva.yuxino.cn">官网</a></p>

<p align="center">在 macOS 和 Windows 上编辑本地文件的 Markdown 编辑器。</p>

<p align="center">
  <a href="README.md">English</a> · 简体中文
</p>

用 Viva 打开存放 Markdown 文件的文件夹，就能写笔记、修改草稿和搜索文档。
点开段落可以原地编辑源码，也可以并排查看源码和预览。文件以普通 Markdown
格式保存在你的电脑上，不需要账户或同步服务。

<!-- project-demo-v1 -->
## 演示

<p align="center">
  <a href="docs/demos/demo.mp4"><img src="docs/demos/preview.gif" alt="viva — 演示"></a>
</p>
<p align="center">写 Markdown，切换编辑视图，用大纲、多标签和查找整理笔记。</p>
<p align="center"><a href="docs/demos/demo.mp4">观看视频</a></p>
<!-- /project-demo-v1 -->

## 在排版后的页面里编辑 Markdown

在 Live 模式中，点开段落即可编辑对应的 Markdown，其他段落仍然保持排版。
也可以切换到 Source、Split 或 Preview，分别查看源码、分屏预览或排版后的文档。
Focus 专注模式会收起侧边栏和预览。

## Viva 能做什么

- 打开文件夹，用多个标签页同时查看文档，在文件树中查找和管理文件。
- 搜索整个工作区、浏览文档大纲，并找回以前保存过的版本。
- 在当前文档中查找和替换，并将粘贴的图片保存到本地 `assets/`，以相对路径引用。
- 内置 Dart、TypeScript 等常用语言的围栏代码语法高亮。
- 在编辑、另存为和恢复历史版本时，保留每篇文档原有的 LF 或 CRLF 换行格式。
- 查看哪些文档有未保存的修改，在关闭标签页、窗口或退出应用前选择是否保存。
- 选择浅色或深色界面，也可以使用本地图片作为背景。

## 默认留在本地

Viva 不上传文档、不做行为统计，也不需要账户。Markdown、历史版本、外观设置
和可选背景图都保存在本机；外部链接只有在你主动点击时才会打开。手动检查软件更新时，
Viva 会通过原生 HTTPS 请求访问固定的 GitHub Release 更新源，不会携带文档、设置或使用数据。

## 签名软件更新

打开**外观与背景 → 软件更新**，即可检查新版本、阅读更新说明，再决定是否下载。
安装前，Tauri 会使用 Viva 内置公钥验证更新包签名；验证失败的更新包无法安装。

**首次启用：** 使用 Viva 2.0.6 及更早版本时，请先从
[GitHub Releases](https://github.com/yuxino/viva/releases) 手动安装一次 2.0.7 或更高版本。
2.0.5 及更早版本没有更新器；2.0.6 缺少检查时读取应用版本所需的权限。
2.0.7 已修复该权限，此后的签名版本可以直接在 Viva 内完成更新。

<details>
<summary>开发</summary>

Viva 使用 Tauri、Rust、React 与 TypeScript 构建，支持 macOS 和 Windows。
开发需要 Node.js 24、pnpm 11、稳定版 Rust，以及对应平台的
[Tauri 前置环境](https://v2.tauri.app/start/prerequisites/)。

```bash
pnpm install
pnpm tauri dev
```

</details>

## 许可证

MIT
