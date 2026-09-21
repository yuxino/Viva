<p align="center">
  <img src="public/art/viva-character-logo-round.webp" width="136" height="136" alt="Viva character logo">
</p>

<h1 align="center">Viva</h1>

<p align="center"><a href="https://viva.yuxino.cn">Website</a></p>

<p align="center">A Markdown editor for local files on macOS and Windows.</p>

<p align="center">
  English · <a href="README_ZH.md">简体中文</a>
</p>

Viva opens a folder of Markdown files so you can write notes, edit drafts, and
search across documents. Click a paragraph to edit its source in place, or keep
source and preview side by side. Files stay on your computer as ordinary
Markdown; no account or sync service is required.

<!-- project-demo-v1 -->
## Demo

<p align="center">
  <a href="docs/demos/demo.mp4"><img src="docs/demos/preview.gif" alt="viva — Demo"></a>
</p>
<p align="center">Write Markdown, switch editing views, and organize notes with outlines, tabs, and search.</p>
<p align="center"><a href="docs/demos/demo.mp4">Watch video</a></p>
<!-- /project-demo-v1 -->

## Edit Markdown in place

In Live mode, click a paragraph to edit its Markdown while the rest of the
document stays rendered. Source, Split, and Preview views let you work with
source text, a side-by-side preview, or the rendered document. Focus mode hides
the sidebar and preview.

## Features

- Open a folder, keep several documents in tabs, and navigate or manage files from the file tree.
- Search the whole workspace, follow the document outline, and recover earlier saves.
- Find and replace in the current document, and paste images into local `assets/` with relative paths.
- Read Dart, TypeScript, and other fenced code with built-in syntax highlighting.
- Preserve each document's LF or CRLF line endings across editing, Save As, and history restores.
- See which documents have unsaved changes and choose what to save before closing a tab, window, or the app.
- Choose a light or dark theme and, optionally, a local background image.

## Local by default

Viva does not upload documents, run analytics, or require an account. Markdown,
history, appearance settings, and optional background artwork stay on the device.
External links open only when you choose them. A manual Software Update check
makes one native HTTPS request to Viva's fixed GitHub Release feed; documents,
settings, and usage data are never included.

## Signed software updates

Open **Appearance and background → Software Update** to check for a new
version, read the release notes, and choose whether to download. Tauri verifies
the update package against Viva's embedded public key before installation.
Packages that fail verification cannot be installed.

**Bootstrap:** Install 2.0.7 or later manually once from
[GitHub Releases](https://github.com/yuxino/viva/releases) if you use 2.0.6 or earlier.
Versions through 2.0.5 have no updater; 2.0.6 is missing the permission needed to
read the app version during a check. Version 2.0.7 fixes that permission, so future
signed releases can be installed from inside Viva.

<details>
<summary>Development</summary>

Viva is built with Tauri, Rust, React, and TypeScript for macOS and Windows.
Development requires Node.js 24, pnpm 11, stable Rust, and the platform-specific
[Tauri prerequisites](https://v2.tauri.app/start/prerequisites/).

```bash
pnpm install
pnpm tauri dev
```

</details>

## License

MIT
