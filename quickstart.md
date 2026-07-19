# UCII Developer Quickstart

## Universal Cryptographic Identity Infrastructure

> Identity is the primitive. Authentication is an application.

UCII provides permanent cryptographic identity for:

- HUMAN
- AI_AGENT
- ROBOT
- DEVICE
- SERVICE
- ORGANIZATION

## Integration Flow

1. Create Identity
2. Register Credential
3. Verify Credential
4. Access Protected Services
5. Authorize via x402

## Discovery Endpoints

Metadata:
https://api.ucii.sportgen-ai.com/metadata

OpenAPI:
https://api.ucii.sportgen-ai.com/openapi.json

API Docs:
https://api.ucii.sportgen-ai.com/docs

x402 Discovery:
https://api.ucii.sportgen-ai.com/v1/x402/info

## x402 Authorization

Protected operations return:

HTTP 402 Payment Required

Clients provide payment authorization.

UCII verifies settlement.

Authorized requests are executed.

## Documentation

- docs/identity-model.md
- docs/cryptographic-architecture.md
- docs/security-model.md
- docs/api-reference.md
- docs/x402-integration.md
