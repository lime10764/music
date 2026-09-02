# music

Liquid Glass Player 的音乐库。

## 使用规则

1. **直接把音乐文件丢到本仓库根目录**，文件名就是歌名，**不要带后缀**：

```
晴天
海阔天空
Bohemian Rhapsody
```

2. 播放器（`lime10764-liquid-glass-player`）通过 jsDelivr 目录接口自动扫描本仓库，
   识别到新文件后会自动出现在播放列表，**无需改任何代码**。

3. 想填歌手名，编辑本仓库的 `manifest.json`：

```json
[
  { "file": "晴天", "artist": "周杰伦" },
  { "file": "海阔天空", "artist": "Beyond" }
]
```

> `manifest.json` 是**可选的**。不写也能跑，播放器会自动探测每首歌的真实后缀。

## 支持的格式

MP3 / FLAC / WAV / OGG / M4A / AAC / OPUS / WMA / AIFF / APE / WV / CAF / WebM

> ⚠️ 酷狗 `.kgm` / `.kgg` 是加密格式（DRM），浏览器无法解码。
> 请用酷狗客户端转成 MP3 或 FLAC 后再上传，文件名无后缀即可。

## 背景图（可选）

把 `image_download_1787389320083.jpg` 放到本仓库根目录，
播放器会自动加载它作为背景。找不到就降级为 CSS 渐变。
