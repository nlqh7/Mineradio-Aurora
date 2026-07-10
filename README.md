# Mineradio Aurora

Mineradio Aurora 是基于 Mineradio 的个人改版桌面音乐播放器，重点保留沉浸式暗色视觉、歌词舞台、3D 歌单架，并加入更适合日常使用的桌面背景和窗口体验。

![Mineradio 暗场启动页](./docs/assets/readme/cinema-beat-smoke.png)

## 这个版本有什么

- Wallpaper Engine 壁纸选择：可浏览本机已下载的创意工坊壁纸，并把图片或视频壁纸作为播放器背景。
- 桌面透传模式：让播放器进入近乎透明状态，桌面和其他窗口可直接操作；右下角提供退出和歌单架显示开关。
- 启动恢复上次视觉预设：重启后不再被首页预览强制切走。
- 记住窗口位置：下次启动恢复上次窗口大小和位置，屏幕变化时自动回到可见区域。
- 原有沉浸式音乐体验：搜索播放、歌词舞台、粒子视觉、3D 歌单架、网易云/QQ 音乐辅助接入等。

## 开发运行

```bash
npm install
npm start
npm run build:win
```

桌面版由 Electron 主进程启动本地服务。Windows 打包使用 `npm run build:win`，产物位于 `dist/`。

## 同步上游

本仓库保留原作者仓库作为 `upstream`，个人改动推送到 `origin`。

```bash
git switch main
git fetch upstream
git merge upstream/main
git push origin main
```

如果合并上游时出现冲突，需要手动处理后再提交。

## 第三方平台说明

本项目不是网易云音乐、QQ 音乐、腾讯音乐娱乐集团或 Wallpaper Engine 的官方客户端，也不隶属于这些平台。

第三方平台接入仅用于个人学习、本地客户端体验和用户自有账号的播放辅助。请遵守对应平台的用户协议、版权规则和会员权益规则。

## 出处与授权

本项目基于 [XxHuberrr/Mineradio](https://github.com/XxHuberrr/Mineradio) 修改。

原项目 Copyright (C) 2026 XxHuberrr，采用 GPL-3.0 授权。详见 [LICENSE](./LICENSE)。

MR Logo、Mineradio 名称、界面视觉设计与原创视觉表达归原作者所有；本仓库仅作为个人学习和自用改版维护。
