# Codex Dream Skin · 项目记录

> 本地归档说明。面向维护者，不是用户安装手册。

仓库首页：

- 中文：[`../README.md`](../README.md)
- English：[`../README.en.md`](../README.en.md)
- GitHub：`https://github.com/ChenShuo2004/Codex-Dream-Skin`
- X：`https://x.com/ChenshuoAI`

## 1. 它是什么

**Codex Dream Skin · X Account Edition** 是给 **OpenAI Codex 桌面端** 用的外部主题 / 换肤方案：

- 本机 **CDP** 注入 CSS + 装饰 DOM。
- **不修改**官方 `.app` / `app.asar` / WindowsApps / 代码签名。
- 侧栏、建议卡、项目选择、输入框仍是原生可点控件。
- 可换图、可恢复。
- **不会**静默改写 API Key / Base URL。

非 OpenAI 官方产品。

## 2. 当前版本改动

本版本基于上游开源项目拉取，做了个人 X 账号版本改造：

- README 顶部赞助位改为 `@ChenshuoAI` 的 X 账号引导。
- macOS 主题配置里的底部 promo chip 改为 X 链接。
- Gallery 案例图替换为 5 张新的 Codex 皮肤案例图。
- 宣传文案改为个人品牌分发版本。

## 3. 仓库结构

```text
Codex-Dream-Skin/
├── README.md
├── README.en.md
├── docs/
│   ├── PROJECT.md
│   ├── platforms.md
│   ├── promo-copy.md
│   └── images/
│       ├── gallery/
│       │   ├── skin-01.jpg
│       │   ├── skin-02.jpg
│       │   ├── skin-03.jpg
│       │   ├── skin-04.jpg
│       │   └── skin-05.jpg
│       └── x-account-badge.svg
├── macos/
└── windows/
```

## 4. 安装后的运行位置

| 用途 | 路径 |
| --- | --- |
| macOS 引擎 | `~/.codex/codex-dream-skin-studio` |
| macOS 状态 / 主题 | `~/Library/Application Support/CodexDreamSkinStudio` |
| Windows 状态 | `%LOCALAPPDATA%\CodexDreamSkin` |

## 5. 常用维护动作

| 动作 | 说明 |
| --- | --- |
| 换案例图 | 替换 `docs/images/gallery/skin-XX.jpg`，同步改 README 两份 caption |
| 改 X 账号 | 搜索 `ChenshuoAI` 并统一替换 |
| 改仓库地址 | 搜索 `ChenShuo2004/Codex-Dream-Skin` 并统一替换 |
| 发版推送 | `git add` → `git commit` → `git push origin main` |

## 6. 安全与合规边界

1. CDP 仅绑定 `127.0.0.1`。
2. 不改官方安装目录与签名。
3. 禁止安装脚本静默写入第三方 Base URL / Key。
4. 效果图含人物 / IP 时仅作主题示意；商用再分发需自行确认授权。

---

最后更新：随仓库提交维护。
