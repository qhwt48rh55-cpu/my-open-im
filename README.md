<p align="center">
    <a href="#">
        <img src="./assets/logo-gif/openim-logo.gif" width="60%" height="30%"/>
    </a>
</p>

<div align="center">

[![License](https://img.shields.io/badge/license-Apache--2.0-green?style=for-the-badge)](./LICENSE)
[![Language](https://img.shields.io/badge/Language-Go-blue.svg?style=for-the-badge&logo=go&logoColor=white)](https://golang.org/)
[![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20Windows%20%7C%20Mac-orange?style=for-the-badge)](配置您的服务器)

<p align="center">
  <strong>专业的私有化部署即时通讯解决方案</strong>
</p>

<p align="center">
  <a href="./README_zh_CN.md">中文文档</a> · 
  <a href="./README.md">English</a>
</p>

</div>

---

## Ⓜ️ 关于 SmartIM (智联通讯)

**SmartIM** 是一套专为企业级用户打造的开源即时通讯（IM）解决方案。与 Telegram 或 Rocket.Chat 等单一应用不同，SmartIM 提供了一整套底层的通讯能力，旨在帮助开发者和企业快速将聊天、音视频通话、群组管理等功能集成到自己的现有业务系统中。

通过私有化部署，您可以确保所有聊天数据完全存储在自己的服务器上，彻底解决数据隐私和安全合规问题。

![系统架构图](./docs/images/oepnim-design.png)

## 🚀 核心组件介绍

### 1. SmartIM-SDK (客户端核心)
专门为移动端（iOS/Android）、Web 端及桌面端打造的通讯 SDK，支持：
- 🌟 **主要功能**：
  - 📦 本地数据加密存储
  - 🔔 实时消息回执与通知
  - 🛡️ 安全稳定的 API 封装
  - 🌐 高并发连接管理

### 2. SmartIM-Server (服务端核心)
基于 Golang 开发的高性能后端，支持：
- 🌐 **微服务架构**：支持集群模式，可轻松应对千万级用户并发。
- 🚀 **灵活部署**：支持宝塔面板 Docker 一键部署、Kubernetes 集群部署。
- **海量支撑**：支持百万级超级群组，具备秒级消息送达能力。

---

## 💎 商业增强功能

- **REST API**：提供丰富的后端接口，支持从您的业务后台直接创建群组、推送系统通知。
- **Webhooks 回调**：支持消息前置/后置过滤，方便对接您的自动审核系统或机器人。
- **多端同步**：消息在手机、电脑、网页端实时同步，无缝切换。

---

## :rocket: 快速开始 (服务器部署)

为了方便快速交付，我们推荐使用 **Docker** 进行一键部署。

1. **环境要求**：Linux 服务器 (推荐使用宝塔面板安装 Docker)。
2. **部署脚本**：
   ```bash
   # 进入部署目录
   cd deployments
   # 启动服务
   docker-compose up -d
