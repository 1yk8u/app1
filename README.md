# APK 下载页

轻量静态下载页：[在线访问](https://1yk8u.github.io/apk-downloads/)

包含应用：

| 应用 | 版本 | 大小 | 下载方式 |
|---|---|---|---|
| 流光音乐（Compose 音乐播放器） | 1.0 | 18 MB | 本仓库 Pages 直链 `apks/liuguang-music-v1.0.apk` |
| AlistApp（alist 3.65.0 内核安卓壳） | 1.0 | 172.6 MB | [Releases v1.0](https://github.com/1yk8u/apk-downloads/releases/tag/v1.0)（超过 Pages 100 MB 限制，走 Release 附件） |

## 本地使用

仓库内附 `server.js`（零依赖 Node 静态服务器，支持断点续传）：

```powershell
cd download-page
node server.js   # 默认 http://0.0.0.0:8765/ 手机同 Wi-Fi 可访问
```

也可用 `tools` 中或任意静态服务器托管本目录。

## 结构

- `index.html` — 下载页（内置二维码，自动指向当前地址）
- `apks/` — 小体积 APK
- `server.js` — 本地静态服务器（可选）

许可证：页面代码 MIT；分发的第三方应用各自许可见其工程说明。
