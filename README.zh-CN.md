# AI Gene Capsule

<p align="center">
  <img src="assets/gene_capsule_logo.png" alt="AI Gene Capsule" width="320" />
</p>

<p align="center"><b>别再折腾配置了，直接用。</b></p>

<p align="center">
  <a href="https://github.com/kamiimeteor/AI-Gene-Capsule/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/kamiimeteor/AI-Gene-Capsule?display_name=tag"></a>
  <a href="https://github.com/kamiimeteor/AI-Gene-Capsule/releases"><img alt="Total downloads" src="https://img.shields.io/github/downloads/kamiimeteor/AI-Gene-Capsule/total"></a>
  <img alt="Platform" src="https://img.shields.io/badge/platform-macOS%20arm64-111827">
  <img alt="License" src="https://img.shields.io/badge/license-Proprietary-b91c1c">
</p>

<p align="center">
  <a href="README.md">English</a> · <b>简体中文</b>
</p>

---

你知道自己需要什么工具，但不想花几个小时看教程、敲命令行、调配置文件。

**AI Gene Capsule** 把多工具联合配置变成一个引导式流程。它检查你的系统、安装缺失的依赖、把所有东西连起来 — 全程不需要写一行代码。

## 痛点

本地配置 AI 工具通常意味着：

- 看 5 个工具的 5 份文档
- 复制粘贴一堆你不完全理解的终端命令
- 遇到报错，自己根本没法排查
- 折腾 2 个小时以上，东西还不一定能跑起来

这还是一切顺利的情况。

## 解决方案

AI Gene Capsule 把整个配置流程打包成**胶囊**（Capsule）— 引导式工作流，帮你：

1. **检查**你的系统，看哪些已经装好，哪些还缺
2. **安装**缺失的依赖，根据你的机器自动适配
3. **连接**各个工具，自动写好配置
4. **验证**一切正常，发一条确认消息
5. **生成回执**，让你知道到底改了什么

整个过程：回答几个问题，等 10 分钟，搞定。

## 下载

| 平台 | 架构 | 下载 |
|------|------|------|
| macOS | Apple Silicon (arm64) | [**下载 v0.1.1**](https://github.com/kamiimeteor/AI-Gene-Capsule/releases/latest) |

> Intel macOS、Windows、Linux 即将推出。

### 安装步骤

1. 从 [Releases](https://github.com/kamiimeteor/AI-Gene-Capsule/releases) 页面下载 `.dmg`
2. 打开后将 **AI Gene Capsule** 拖到「应用程序」文件夹
3. 启动 — 如果 macOS 阻止打开，去 **系统设置 > 隐私与安全性 > 仍要打开**

## 当前可用 (v0.1.1)

第一个胶囊：**OpenClaw + Telegram**

| 步骤 | 做什么 |
|------|--------|
| 环境检查 | 扫描你的 Mac，告诉你缺什么 |
| OpenClaw 安装 | 自动安装或验证 OpenClaw，不用开终端 |
| Telegram 桥接 | 引导你连接 Telegram 机器人（粘贴 Token 就行） |
| 回执 | 展示所有安装和配置的详细记录 |

### 截图

<p align="center">
  <img src="assets/screenshots/01-openclaw-home.png" alt="主页" width="700" />
</p>
<p align="center"><i>Quick Start 引导你完成全部设置</i></p>

<p align="center">
  <img src="assets/screenshots/02-telegram-setup.png" alt="Telegram 桥接" width="700" />
</p>
<p align="center"><i>粘贴 Bot Token 就能连接 Telegram，不用手动改配置文件</i></p>

<p align="center">
  <img src="assets/screenshots/03-setup-complete.png" alt="设置完成" width="700" />
</p>
<p align="center"><i>验证通过，附带完整操作回执</i></p>

## 工作原理

```
┌─────────────────────────────────────────────────┐
│                 AI Gene Capsule                  │
│                                                  │
│   ┌──────────┐  ┌──────────┐  ┌──────────┐     │
│   │  检查    │→ │  安装    │→ │  连接    │     │
│   │  你的    │  │  缺失的  │  │  各个    │     │
│   │  系统    │  │  依赖    │  │  工具    │     │
│   └──────────┘  └──────────┘  └──────────┘     │
│         ↓                            ↓          │
│   ┌──────────┐              ┌──────────┐       │
│   │  诊断    │              │  验证 &  │       │
│   │  & 修复  │              │  回执    │       │
│   └──────────┘              └──────────┘       │
│                                                  │
└─────────────────────────────────────────────────┘
```

每个胶囊都会感知你的本地环境和操作系统，检测你已有的工具，适配你的配置，只安装真正需要的东西。

## 适合谁用

- 你**知道自己要什么结果**，但不想学命令行
- 你愿意**花钱买工具和 API**，但不想花时间调试安装报错
- 你想要**在自己电脑上跑的东西**，不是又一个云订阅
- 你装过一些 AI 工具，但**从来没真正配好用过**

## 即将推出

| 胶囊 | 一键配好什么 |
|------|-------------|
| **本地 AI 全家桶** | Ollama + Open WebUI + 本地模型 — 完全私有，不走云端 |
| **Discord 桥接** | 把 AI 接入你的 Discord 服务器 |
| **飞书桥接** | 把 AI 接入飞书工作区 |
| **团队开发环境** | Git hooks + 代码规范 + 格式化 — 团队一键统一 |

目标：一个胶囊库，把「我要 X」变成一个能跑的本地环境，不用看任何教程。

## 免费与付费

桌面应用**永久免费**。

未来可能收费的部分在本地应用之上：
- 托管胶囊中心 + 自动更新推送
- 托管桥接服务（保持连接在线）
- 团队协作功能
- 云端监控和审计日志
- 商业支持

## 系统要求

- macOS 14+，Apple Silicon (arm64)
- 设置过程需要联网
- Telegram 桥接需要一个 Bot Token（从 [@BotFather](https://t.me/BotFather) 获取）

高级用户如需校验下载文件完整性，可查看 [SHA256SUMS.txt](SHA256SUMS.txt)。

## 常见问题

| 问题 | 解决 |
|------|------|
| macOS 提示无法打开 | **系统设置 > 隐私与安全性 > 仍要打开**（v0.1.1 尚未公证） |
| Telegram 没发出首条消息 | 在 Telegram 里打开 Bot，点 **Start**，再重试 |
| Token 被拒绝 | 确保粘贴了完整 Token，包括数字前缀和冒号 |
| Intel Mac 不支持 | 目前仅 arm64，Intel 版即将推出 |

## 相关链接

- [更新日志](CHANGELOG.md)
- [安全政策](SECURITY.md)
- [隐私政策](PRIVACY.md)
- [参与贡献](CONTRIBUTING.md)
- [行为准则](CODE_OF_CONDUCT.md)

## 反馈

发现 Bug？需要新的胶囊？[提交 Issue](https://github.com/kamiimeteor/AI-Gene-Capsule/issues)。

## 许可证

专有软件 — 免费下载使用。详见 [LICENSE](LICENSE)。
