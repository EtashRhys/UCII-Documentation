# UCII

## 通用加密身份基础设施

**身份是原生基础。身份验证只是其中一种应用。**

采用后量子密码学保护，并通过 x402 经济授权机制保障的生产级加密身份基础设施。

---

## 概述

UCII（Universal Cryptographic Identity Infrastructure，通用加密身份基础设施）是一套为下一代互联网设计的生产级身份基础设施。

UCII 不将身份验证视为系统的基础，而是将 **身份（Identity）** 视为永久性的加密原语。身份验证、授权、凭证、支付以及应用级信任，都成为构建于身份之上的服务，而不是定义身份本身的核心。

每一个受保护的操作均使用现代后量子密码学进行保护，并通过 x402 支付协议进行经济强制执行。

UCII 旨在为人类、AI 智能体、自主系统、组织、服务以及连接设备提供安全基础。

---

## 为什么选择 UCII？

传统身份系统围绕用户名、密码、OAuth 提供商以及身份验证会话构建。

UCII 采用不同的方法。

身份应当独立于其身份验证方式而存在。

密码会过期。

OAuth 提供商会变化。

证书会轮换。

身份验证方式会不断演进。

身份应该保持永久。

UCII 将加密身份确立为根对象，使身份验证方式、凭证以及授权机制能够不断演进，而无需替换底层身份。

---

## 核心功能

* 通用加密身份基础设施
* 原生支持多种身份类别

  * 人类
  * AI 智能体
  * 设备
  * 机器人
  * 组织
  * 服务
* ML-DSA 后量子加密凭证
* 多个活动签名密钥
* 安全凭证轮换
* 加密凭证验证
* 生产级 REST API
* x402 支付强制执行
* 结算验证
* 结算收据持久化存储
* 防重放攻击保护
* 生产级 FastAPI 部署

---

## 架构

```
                应用程序
                      │
              身份验证
                      │
                授权
                      │
                凭证
                      │
              通用身份
                      │
          后量子密码学
```

身份是永久的。

其他所有能力都建立于其之上。

---

## 经济授权（x402）

UCII 集成 x402 协议，为基础设施服务提供原生经济授权能力。

每个受保护端点都会公开所需支付金额。

客户端提交支付证明。

UCII 验证结算状态。

结算收据被永久记录。

重放尝试将被拒绝。

只有通过验证后，受保护操作才会执行。

经济授权成为基础设施的一部分，而不是外部计费系统。

---

## 生产状态

### Phase 2.5 生产强化版本

✅ 通用身份基础设施

✅ ML-DSA 凭证框架

✅ 凭证验证

✅ 结算验证

✅ 结算收据持久化

✅ 重放保护

✅ 生产边界测试

✅ 环境隔离

✅ x402 经济授权

✅ 公共 REST API

已准备进行 x402 集成。

---

## 公共 API

### 创建身份

```
POST /v1/identity
```

创建新的通用加密身份。

**价格：0.50 USDC**

---

### 注册凭证

```
POST /v1/credentials/register
```

注册加密凭证。

**价格：0.75 USDC**

---

### 验证凭证

```
POST /v1/credentials/verify
```

验证已注册的凭证。

**价格：0.10 USDC**

---

其他端点通过 OpenAPI 规范进行文档说明。

---

## 与后量子安全的结合

UCII 基于现代后量子密码学构建，采用包括 ML-DSA 和 ML-KEM 在内的 NIST 标准化算法。

该项目符合全球行业向抗量子基础设施转型的发展趋势，旨在帮助组织在后量子迁移截止日期之前，采用可投入生产使用的加密身份系统。

---

## 路线图

### 已完成

* 通用加密身份
* 后量子凭证
* x402 经济授权
* 结算验证
* 重放保护
* 生产级 API

### 计划中

* JavaScript SDK
* Python SDK
* Go SDK
* Rust SDK
* 托管式 UCII 平台
* 更多结算适配器
* 扩展身份服务

---

## 项目愿景

UCII 正在构建基础设施，而不是单一应用。

身份应该是通用的。

密码学应该具备量子安全能力。

授权应该能够通过经济机制进行强制执行。

开发者应该能够在身份基础设施之上构建应用，而不是为每个应用重新创建身份系统。

UCII 的存在，就是为了提供这一基础。

---

<img width="1200" height="800" alt="17827196299747102586194974612432" src="https://github.com/user-attachments/assets/612b45fc-8b78-4931-a3c9-7d27a1bad07f" />

<p align="center">
  <a href="https://www.whitehouse.gov/gallery/president-donald-j-trump-signs-executive-orders-on-quantum-in-the-oval-office/">
    <img src="https://img.shields.io/badge/White_House-Gallery-0A2540?style=for-the-badge" alt="Gallery">
  </a>
  <a href="https://www.whitehouse.gov/videos/president-trump-signs-executive-orders-jun-22-2026/">
    <img src="https://img.shields.io/badge/Watch-Video-red?style=for-the-badge" alt="Video">
  </a>
  <a href="https://www.youtube.com/live/HNipoXNANAs?si=zfwh6OOjdR42zwA6">
    <img src="https://img.shields.io/badge/YouTube-Live-red?style=for-the-badge&logo=youtube" alt="YouTube">
  </a>
</p>

[![Python](https://img.shields.io/badge/Python-3.11+-blue)](https://www.python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.115+-green)](https://fastapi.tiangolo.com)

---

**🛡️ 与白宫行政命令保持一致 — 2026年6月22日**

2026年6月22日，美国总统唐纳德·J·特朗普签署了两项具有里程碑意义的行政命令：

* **EO 14412**：*《保护国家免受高级密码攻击》*
* **EO 14413**：*《开启量子创新的新前沿》*

这些行政命令加速美国向后量子密码学转型，并设定了严格期限：

* 高价值资产和密钥建立 → **截至2030年12月31日**
* 数字签名和身份验证 → **截至2031年12月31日**

---
