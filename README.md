<div align="center">

<img src="https://jetpooh.com/specola.png" width="120" alt="Specola logo" />

# Specola

**Every connection on your machine, in plain sight.**

A native desktop network toolkit with a C++20 core and a Qt Quick UI: live connections by process,
searchable connection history, route maps, DNS logs and rule-based routing from one TOML file.
Available for Windows; macOS and Linux coming soon.

English · [简体中文](Readme.zh-CN.md)

[![Website](https://img.shields.io/badge/website-jetpooh.com-ff5a1f)](https://jetpooh.com)
[![Docs](https://img.shields.io/badge/docs-manual-2a2a2f)](https://jetpooh.com/docs/manual/)
![Platforms](https://img.shields.io/badge/platform-Windows-lightgrey)
![License](https://img.shields.io/badge/license-commercial-blue)
[![Releases](https://img.shields.io/github/v/release/jetpooh-software/specola?include_prereleases&label=release)](https://github.com/jetpooh-software/specola/releases)

**[Buy a license — $20](https://jetpooh.com/#pricing)** · [Download](https://github.com/jetpooh-software/specola/releases) · [Documentation](https://jetpooh.com/docs/manual/) · [Report an issue](https://github.com/jetpooh-software/specola/issues)

</div>

---

See which process opened each connection, where it went and which rule sent it there — live, and for weeks afterwards. When you want a different path, write a rule.

Specola is a local application. It observes your own machine's connections and routes them by your rules, only through gateways **you already operate or are authorized to use**.

## ✨ Features

| | |
| --- | --- |
| ⚡ **Native and light** | C++20 core on Asio coroutines. No runtime, no GC, low memory and fast startup. |
| 🔍 **Live connections** | Every connection with its process, destination, matched rule, route and throughput. Turn any connection into a rule in one click. |
| 🕘 **Connection history** | Search 24 hours up to 90 days: heatmaps, app-to-destination flows, why each connection ended, CSV export. |
| 🗺️ **Route map** | Each route drawn from your machine through relay hops to its destination, with per-hop latency. |
| 🛡️ **Enhanced Mode** | Captures every app system-wide — including tools that ignore network environment variables. |
| 🎯 **Rules that make sense** | First-match rules on domain, IP-CIDR, GeoIP, port and process name. Direct / Global / Rule modes. |
| 🔀 **Gateway groups** | `select`, `url-test`, `fallback` and `load-balance` with health checks, so a dead upstream never blocks your build. |
| 🌐 **DNS inspector** | Per-domain resolvers, fallback, hosts and Fake-IP, with every query and answer in the log. |
| 🔌 **One local port** | Mixed HTTP / SOCKS5 listener on `127.0.0.1`. Enhanced Mode for system-wide capture. |
| 📝 **Config as code** | One readable TOML profile you can keep with your dotfiles in Git. |
| 🖥️ **Desktop UI or headless** | Qt Quick UI with connection, history, route map, DNS and log views. The core also runs headless as a background service. |

## 🧑‍💻 Made for developers

- Find out what a build, an installer or a background service actually connects to.
- Test a service behind a specific gateway.
- See exactly which rule each connection matched and where it went — and look it up again days later.
- Send package managers and CI tools through a company gateway while everything else stays direct.
- Switch routing mode from the tray or a keyboard shortcut.

## 🚀 Get started

1. **[Buy a license](https://jetpooh.com/#pricing)**. The license key is emailed to you after checkout.
2. **[Download](https://github.com/jetpooh-software/specola/releases)** the installer for your platform.
3. Open Specola, paste the key, and follow the **[Quick start](https://jetpooh.com/docs/manual/quick-start)**.

Specola starts in Direct mode, so nothing changes until you add a server or rule.

## 💳 Pricing

| Specola Personal License | **$20 USD, one-time** |
| --- | --- |
| License | Lifetime license for Specola 1.x |
| Devices | Activation on one device (transfers on request) |
| Updates | All 1.x updates and bug fixes |
| Support | Email support at [support@jetpooh.com](mailto:support@jetpooh.com) |
| Refund | 14-day full refund, no questions asked |

No subscription and no automatic renewal. Checkout by [Gumroad](https://gumroad.com/), our Merchant of Record.

## ❓ FAQ

**Is Specola a network service?**
No. Specola runs entirely on your computer and includes no servers, IP addresses or bandwidth. It only forwards traffic to gateways you configure yourself.

**Which platforms are supported?**
Windows today. macOS and Linux are coming soon. Check the [manual](https://jetpooh.com/docs/manual/) for current requirements.

**What data does Specola collect?**
Connection history, DNS and logs stay on your computer. Specola does not collect or sell your browsing or traffic data. See the [Privacy Policy](https://jetpooh.com/legal/privacy.html).

## 📮 Links

- Website: [jetpooh.com](https://jetpooh.com)
- Documentation: [Manual](https://jetpooh.com/docs/manual/) · [Knowledge Base](https://jetpooh.com/docs/knowledge-base/)
- Clash profile converter: [jetpooh.com/tools/clash-converter.html](https://jetpooh.com/tools/clash-converter.html)
- Downloads and bug reports: [github.com/jetpooh-software/specola](https://github.com/jetpooh-software/specola)
- Contact: [support@jetpooh.com](mailto:support@jetpooh.com)

---

<div align="center">
<sub>Specola is proprietary software. © 2026 Jetpooh Software. All rights reserved. · <a href="https://jetpooh.com/legal/terms.html">Terms</a> · <a href="https://jetpooh.com/legal/refund.html">Refund Policy</a></sub>
</div>
