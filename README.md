"AI agents need cryptographic identity before they can safely transact."

**Permanent cryptographic identity for humans, AI agents, devices, and organizations.**

Secured by ML-DSA Post-Quantum Cryptography • Enforced by x402 Economic Authorization

## 🌍 Language / Idioma

- **[English](README.md)**  
- **[Español](README.es.md)**  
- **[Português](README.pt.md)** 
- **[中文](README.zh.md)**  
- **[Deutsch](README.de.md)**  
- **[Français](README.fr.md)**
- **[Italiano](README.it.md)**
- **[日本語](README.ja.md)**
- **[русский](README.ru.md)**


---

## Documentation

Public Documentation:

https://ucii.sportgen-ai.com/docs/

Developer API:

https://api.ucii.sportgen-ai.com/docs

OpenAPI Schema:

https://api.ucii.sportgen-ai.com/openapi.json

Machine Discovery:

https://api.ucii.sportgen-ai.com/metadata

x402 Discovery:

https://api.ucii.sportgen-ai.com/v1/x402/info

# UCII

## Universal Cryptographic Identity Infrastructure

**Identity is the primitive. Authentication is just an application.**

Production-ready cryptographic identity infrastructure secured with Post-Quantum Cryptography and protected by x402 economic authorization.

---

## Overview

UCII (Universal Cryptographic Identity Infrastructure) is a production-grade identity infrastructure designed for the next generation of the Internet.

Rather than treating authentication as the foundation of a system, UCII treats **identity** as the permanent cryptographic primitive. Authentication, authorization, credentials, payment, and application-specific trust become services built on top of identity rather than defining it.

Every protected operation is secured using modern Post-Quantum Cryptography and economically enforced through the x402 payment protocol.

UCII is designed to provide a secure foundation for humans, AI agents, autonomous systems, organizations, services, and connected devices.


---

## Designed For

UCII provides identity infrastructure for:

- AI agents requiring autonomous cryptographic identity
- Applications requiring verifiable identity primitives
- Organizations requiring trusted infrastructure identities
- Devices and robots requiring machine identity
- Developers building identity-aware systems

---

## Why UCII?

Traditional identity systems revolve around usernames, passwords, OAuth providers, and authentication sessions.

UCII takes a different approach.

An identity should exist independently of how it authenticates.

Passwords expire.

OAuth providers change.

Certificates rotate.

Authentication methods evolve.

Identity should remain permanent.

UCII establishes cryptographic identity as the root object and allows authentication methods, credentials, and authorization mechanisms to evolve without replacing the underlying identity.

---

## Core Features

* Universal Cryptographic Identity Infrastructure
* Native support for multiple identity classes

  * Human
  * AI Agent
  * Device
  * Robot
  * Organization
  * Service
* ML-DSA Post-Quantum cryptographic credentials
* Multiple active signing keys
* Secure credential rotation
* Cryptographic credential verification
* Production REST API
* x402 payment enforcement
* Settlement verification
* Settlement receipt persistence
* Replay attack protection
* Production-ready FastAPI deployment


---

## Quick Start

Discover UCII capabilities:

https://api.ucii.sportgen-ai.com/metadata

Review available x402 operations:

https://api.ucii.sportgen-ai.com/v1/x402/info

Explore the API schema:

https://api.ucii.sportgen-ai.com/openapi.json

Developer documentation:

https://ucii.sportgen-ai.com/docs/

Integrate UCII through the production API:

https://api.ucii.sportgen-ai.com

---

## Architecture

```
                Applications
                      │
              Authentication
                      │
              Authorization
                      │
             Credentials
                      │
        Universal Identity
                      │
        Post-Quantum Cryptography
```

Identity is permanent.

Everything else builds on top of it.

---

## Economic Authorization (x402)

UCII integrates the x402 protocol to provide native economic authorization for infrastructure services.

Every protected endpoint publishes its required payment.

Clients submit a payment proof.

UCII verifies settlement.

A settlement receipt is permanently recorded.

Replay attempts are rejected.

Only then is the protected operation executed.

Economic authorization becomes part of the infrastructure rather than an external billing system.

---

## x402 Machine Discovery

UCII exposes machine-readable service information through standard HTTP responses.

When a client requests a protected infrastructure operation without payment authorization, UCII returns an HTTP `402 Payment Required` response.

This response provides the information required for autonomous clients to understand:

- what service is being accessed
- what capability is being requested
- which payment protocol is required
- what network settlement occurs on
- where payment should be submitted

Example:

Request:

```http
POST /v1/identity
Content-Type: application/json

{
  "type": "AI_AGENT"
}
```
Response:

```http
HTTP/1.1 402 Payment Required
Content-Type: application/json

{
  "error": "payment_required",
  "service": {
    "name": "Universal Cryptographic Identity Infrastructure",
    "short_name": "UCII",
    "category": "identity-infrastructure",
    "capabilities": [
      "cryptographic_identity_creation",
      "post_quantum_credentials",
      "machine_identity"
    ]
  },
  "payment": {
    "protocol": "x402",
    "amount": "0.50",
    "currency": "USDC",
    "network": "Solana",
    "payTo": "UCII_PAYMENT_ADDRESS"
  },
  "endpoint": "/v1/identity",
  "method": "POST"
}
```
The payment destination is provided dynamically by the UCII service and may vary by deployment.

---

## x402 Discovery Compatibility

UCII exposes machine-readable service information through its `/v1/x402/info` discovery endpoint.

This endpoint provides UCII-specific service metadata and operation information while remaining compatible with the standard x402 payment flow.

UCII does not define a replacement discovery protocol. The endpoint is intended as a service-level discovery interface while payment authorization continues to follow the x402 HTTP 402 payment lifecycle.

Payment requirements are communicated through HTTP `402 Payment Required` responses and validated through the x402 payment authorization flow.

---

## Production Status

### UCII V1 Production Infrastructure

✅ Universal Identity Infrastructure

✅ ML-DSA Credential Framework

✅ Credential Verification

✅ Settlement Verification

✅ Settlement Receipt Persistence

✅ Replay Protection

✅ Production Boundary Testing

✅ Environment Separation

✅ x402 Economic Authorization

✅ Public REST API

✅ Production x402 economic authorization is active.

---

## Public API

### Create Identity

```
POST /v1/identity
```

Creates a new Universal Cryptographic Identity.

**Price:** 0.50 USDC

---

### Register Credential

```
POST /v1/credentials/register
```

Registers a cryptographic credential.

**Price:** 0.75 USDC

---

### Verify Credential

```
POST /v1/credentials/verify
```

Verifies a registered credential.

**Price:** 0.10 USDC

---

Additional endpoints are documented through the OpenAPI specification.

## Service Discovery

UCII exposes machine-readable discovery surfaces:

- `/` — service identity and capability summary
- `/metadata` — machine-readable service metadata
- `/health` — operational health status
- `/v1/x402/info` — x402 service discovery and pricing

API documentation:

- `/openapi.json` — OpenAPI schema
- `/docs` — interactive API documentation
- `/redoc` — alternative API documentation interface

---

## Alignment with Post-Quantum Security

UCII is built around modern Post-Quantum Cryptography using NIST-standardized algorithms including ML-DSA and ML-KEM.

The project aligns with the broader industry transition toward quantum-resistant infrastructure and is intended to help organizations adopt production-ready cryptographic identity systems well before post-quantum migration deadlines.

---

## Roadmap

### Completed

* Universal Cryptographic Identity
* Post-Quantum Credentials
* x402 Economic Authorization
* Settlement Verification
* Replay Protection
* Production API

### Planned

* JavaScript SDK
* Python SDK
* Go SDK
* Rust SDK
* Hosted UCII Platform
* Additional settlement adapters
* Expanded identity services

---

## Project Vision

UCII is building infrastructure rather than an application.

Identity should be universal.

Cryptography should be quantum-safe.

Authorization should be economically enforceable.

Developers should be able to build applications on top of identity instead of rebuilding identity for every application.

UCII exists to provide that foundation.

---

Technical Documentation
- **[TechOverview](docs/ucii-overview.md)**
- **[Identity](docs/identity-model.md)**
- **[Architecture](docs/architecture.md)**
- **[CryptoArch](docs/cryptographic-architecture.md)**
- **[x402Integ](docs/x402-integration.md)**
- **[Security](docs/security-model.md)**
- **[API](docs/api-reference.md)**
- **[Roadmap](docs/roadmap.md)**

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

**🛡️ Aligned with White House Executive Orders — June 22, 2026**

On **June 22, 2026**, President Donald J. Trump signed two landmark Executive Orders:

- **EO 14412**: *"Securing the Nation Against Advanced Cryptographic Attacks"*
- **EO 14413**: *"Ushering in the Next Frontier of Quantum Innovation"*

These orders accelerate America's transition to Post-Quantum Cryptography with aggressive deadlines:
- High-value assets and key establishment → **by December 31, 2030**
- Digital signatures and authentication → **by December 31, 2031**

---

