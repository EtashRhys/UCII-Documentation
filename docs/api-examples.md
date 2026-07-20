# UCII API Examples

## Overview

Universal Cryptographic Identity Infrastructure (UCII) provides cryptographic identity primitives that applications and services can integrate with.

This guide demonstrates the basic UCII integration flow:

1. Create an identity
2. Register a cryptographic credential
3. Verify credential ownership
4. Authorize access through applications and services

Identity is the primitive.

Authentication is an application.

---

## Base URL

https://api.ucii.sportgen-ai.com/

---


# 1. Create an Identity

An identity represents the permanent cryptographic subject in UCII.

Endpoint:

POST /v1/identity


Example request:

```json
{
  "identity_type": "SERVICE",
  "name": "Example Service",
  "description": "A UCII-enabled service"
}
```


Example response:

```json
{
  "id": "identity-id",
  "identity_type": "SERVICE",
  "name": "Example Service",
  "is_active": true
}
```

---

# 2. Register a Cryptographic Credential

Credentials provide cryptographic proof mechanisms associated with an identity.

Endpoint:

POST /v1/credentials/register

Example request:

```json
{
  "identity_id": "identity-id",
  "credential_type": "ML_DSA_SIGNING_KEY",
  "algorithm": "ML-DSA-65",
  "public_key": "public-key-material",
  "fingerprint": "credential-fingerprint",
  "key_version": "1"
}
```


Example response:

```json
{
  "id": "credential-id",
  "identity_id": "identity-id",
  "credential_type": "ML_DSA_SIGNING_KEY",
  "algorithm": "ML-DSA-65",
  "fingerprint": "credential-fingerprint",
  "status": "ACTIVE"
}
```


---

# 3. Verify Credential Ownership

Credential verification proves control of a registered cryptographic credential.

Endpoint:

POST /v1/credentials/verify

Example request:

```json
{
  "fingerprint": "credential-fingerprint",
  "message": "verification-message",
  "signature": "credential-signature"
}
```


Example response:

```json
{
  "verified": true,
  "fingerprint": "credential-fingerprint",
  "identity_id": "identity-id",
  "status": "ACTIVE",
  "reason": null
}
```


---

# 4. Credential Lifecycle

Credentials have independent lifecycle states.

Supported states:

- ACTIVE
- PENDING
- REPLACED
- REVOKED
- EXPIRED

REPLACED indicates intentional migration to a newer credential.

REVOKED indicates the credential should no longer be trusted.


---

# 5. Compatibility Authentication

UCII provides authentication compatibility endpoints for systems migrating toward cryptographic identity.

Endpoints:

/v1/auth/*

These endpoints allow existing application authentication flows to operate while identity-based infrastructure is adopted.

Authentication remains an application layer built on top of identity.

---

# Summary

UCII separates:

- identity
- credentials
- authentication

Identity is the primitive.

Authentication is an application.

