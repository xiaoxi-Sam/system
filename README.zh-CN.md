# 中小企业（个人环境）内部通信与数据管理系统
这个项目主要是基于私有云环境的实现、利用和探索。 
This project is based on the implementation, utilization and exploration of a private cloud environment.

> [English Version](./README.md)

# 📙 README.zh-CN.md （中文版）

```markdown
# 基于 Proxmox 的中小企业内部通信与数据管理系统

本项目基于 **Proxmox VE** 虚拟化平台，整合 **Mailcow** 邮件系统与 **飞牛 NAS（FeiniuNAS）** 数据存储系统，构建一个面向中小型企业的私有通信与数据管理平台，实现**低成本、高可靠性、高可维护性**的企业级内部服务。

---

## 🧩 项目简介

该系统为企业提供了一个虚拟化的内部服务环境，结合虚拟化技术与容器化应用，实现邮件通信与数据共享的集中化管理与安全隔离。

---

## 🏗️ 系统架构

- **Proxmox VE**：虚拟化与资源调度平台  
- **Mailcow**：企业内部邮件系统  
- **FeiniuNAS**：NAS 文件共享与备份系统  
- **Ubuntu Server**：运行环境基础系统  

![系统架构](./docs/architecture.png)

---

## 🚀 功能特性

- 虚拟化部署，灵活分配资源  
- 内部邮件系统与用户集中管理  
- 数据共享与备份机制  
- 集成防火墙与 SSL/TLS 安全配置  

---

## ⚙️ 部署步骤

```bash
# 1. 安装 Proxmox VE
apt update && apt install proxmox-ve

# 2. 在 PVE 创建 Ubuntu 虚拟机并部署 Mailcow
bash src/install_mailcow.sh

# 3. 使用 Docker 部署 FeiniuNAS
docker-compose up -d


##项目介绍

