<div align="center">

<img src="https://jetpooh.com/specola.png" width="120" alt="Specola logo" />

# Specola

**本机的每一条连接，一目了然。**

基于 C++20 与 Qt Quick 的桌面网络工具：按进程查看实时连接、检索连接历史、路由地图、DNS 日志，
并用一个 TOML 文件按规则分流。目前提供 Windows 版本，macOS 与 Linux 即将推出

[English](Readme.md) · 简体中文

[![Website](https://img.shields.io/badge/website-jetpooh.com-ff5a1f)](https://jetpooh.com)
[![Docs](https://img.shields.io/badge/docs-手册-2a2a2f)](https://jetpooh.com/docs/zh/manual/)
![Platforms](https://img.shields.io/badge/platform-Windows-lightgrey)
![License](https://img.shields.io/badge/license-commercial-blue)
[![Releases](https://img.shields.io/github/v/release/jetpooh-software/specola?include_prereleases&label=release)](https://github.com/jetpooh-software/specola/releases)

**[购买授权 — $20](https://jetpooh.com/#pricing)** · [下载](https://github.com/jetpooh-software/specola/releases) · [使用手册](https://jetpooh.com/docs/zh/manual/) · [问题反馈](https://github.com/jetpooh-software/specola/issues)

</div>

---

看清每条连接由哪个进程发起、去了哪里、命中了哪条规则——实时可见，几周后也能查到。想换一条路径，写一条规则即可。

Specola 是一款本地软件。它观察本机自身的连接，并按你的规则分流，只会经过 **你自己运营或已获授权使用** 的网关。

## ✨ 功能亮点

| | |
| --- | --- |
| ⚡ **原生、轻量** | C++20 Core 基于 Asio 协程，无运行时、无 GC，内存占用低、启动快。 |
| 🔍 **实时连接** | 每条连接的进程、目标、命中规则、路由与吞吐；一键把连接变成规则。 |
| 🕘 **连接历史** | 检索 24 小时到 90 天的记录：热力图、应用到目标的流向、连接结束原因，支持导出 CSV。 |
| 🗺️ **路由地图** | 从本机经中继到目标的每条路由，附逐跳延迟。 |
| 🛡️ **增强模式** | 系统级接管所有应用的流量，不读网络环境变量的工具也能覆盖。 |
| 🎯 **清晰的规则** | 按域名、IP-CIDR、GeoIP、端口、进程名首条匹配；支持 Direct / Global / Rule 三种模式。 |
| 🔀 **网关组** | `select`、`url-test`、`fallback`、`load-balance`，带健康检查，上游失效不会卡住你的构建。 |
| 🌐 **DNS 检查** | 按域名指定解析服务器、fallback、hosts 与 Fake-IP，每次查询与应答都有日志。 |
| 🔌 **一个本地端口** | `127.0.0.1` 上的 HTTP / SOCKS5 混合监听；支持系统级接管的增强模式。 |
| 📝 **配置即代码** | 一个易读的 TOML 配置文件，可以和 dotfiles 一起放进 Git。 |
| 🖥️ **桌面界面或无界面运行** | Qt Quick 界面提供连接、历史、路由地图、DNS、日志视图；Core 也可以作为后台服务独立运行。 |

## 🧑‍💻 为开发者打造

- 弄清一次构建、一个安装程序或后台服务到底连了哪些地址。
- 通过指定网关测试某个服务。
- 清楚看到每条连接命中了哪条规则、最终去了哪里，几天后还能再查。
- 包管理器和 CI 工具走公司网关，其他流量保持直连。
- 从托盘或快捷键切换路由模式。

## 🚀 快速开始

1. **[购买授权](https://jetpooh.com/#pricing)**，付款后授权码会发送到你的邮箱。
2. **[下载](https://github.com/jetpooh-software/specola/releases)** 对应平台的安装包。
3. 打开 Specola，粘贴授权码，然后按照 **[快速上手](https://jetpooh.com/docs/zh/manual/quick-start)** 配置。

Specola 默认以直连模式启动，在你添加服务器或规则之前不会改变任何网络行为。

## 💳 价格

| Specola 个人授权 | **$20 美元，一次性付费** |
| --- | --- |
| 授权 | Specola 1.x 终身授权 |
| 设备 | 一台设备激活（可申请转移） |
| 更新 | 1.x 版本的全部更新与修复 |
| 支持 | 邮件支持 [support@jetpooh.com](mailto:support@jetpooh.com) |
| 退款 | 14 天内无理由全额退款 |

无订阅、无自动续费。结算由 [Gumroad](https://gumroad.com/) 作为销售方（Merchant of Record）处理。

## ❓ 常见问题

**Specola 是网络服务吗？**
不是。Specola 完全运行在你的电脑上，不包含任何服务器、IP 地址或带宽，只会把流量转发到你自己配置的网关。

**支持哪些平台？**
目前支持 Windows，macOS 与 Linux 即将推出。最新要求请查看 [使用手册](https://jetpooh.com/docs/zh/manual/)。

**Specola 会收集哪些数据？**
连接历史、DNS 与日志都只保存在你的电脑上。Specola 不收集、不出售你的浏览或流量数据，详见 [隐私政策](https://jetpooh.com/legal/privacy.html)。

## 📮 相关链接

- 官网：[jetpooh.com](https://jetpooh.com)
- 文档：[使用手册](https://jetpooh.com/docs/zh/manual/) · [知识库](https://jetpooh.com/docs/zh/knowledge-base/)
- Clash 配置转换工具：[jetpooh.com/tools/clash-converter.html](https://jetpooh.com/tools/clash-converter.html)
- 下载与问题反馈：[github.com/jetpooh-software/specola](https://github.com/jetpooh-software/specola)
- 联系我们：[support@jetpooh.com](mailto:support@jetpooh.com)

---

<div align="center">
<sub>Specola 为闭源商业软件。© 2026 Jetpooh Software 保留所有权利。 · <a href="https://jetpooh.com/legal/terms.html">服务条款</a> · <a href="https://jetpooh.com/legal/refund.html">退款政策</a></sub>
</div>
