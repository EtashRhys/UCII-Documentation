# UCII Identity Lifecycle

## Overview

Universal Cryptographic Identity Infrastructure (UCII) treats identity as the root primitive.

An identity represents a permanent cryptographic subject independent from authentication credentials.

Authentication mechanisms may be built on top of identity, but they are not the identity itself.

UCII supports the following identity classes:

- HUMAN
- AI_AGENT
- ROBOT
- DEVICE
- SERVICE
- ORGANIZATION

---

# Identity Lifecycle

A UCII identity lifecycle consists of:

1. Create Identity
2. Register Cryptographic Credential
3. Verify Credential Ownership
4. Maintain Credential Lifecycle
5. Authorize Access Through Applications and Services

The lifecycle relationship:

```text
Identity
 |
 +-- Credential
       |
       +-- Verification
```


---

# 1. Create Identity

An identity is created through the identity endpoint.

Endpoint:

POST /v1/identity

Example request:

{
  "identity_type": "SERVICE",
  "name": "Example Service",
  "description": "A UCII-enabled service"
}


---

# 2. Register Cryptographic Credential

Credentials provide cryptographic proof mechanisms associated with an identity.

Endpoint:

POST /v1/credentials/register

Supported credential types:

- ML_DSA_SIGNING_KEY
- DEVICE_KEY
- SERVICE_KEY
- CERTIFICATE
- ATTESTATION_KEY

Credentials represent proof mechanisms, not identity itself.


---

# 3. Verify Credential Ownership

Credential verification proves control of a registered cryptographic credential.

Endpoint:

POST /v1/credentials/verify

Verification confirms:

- credential exists
- credential belongs to an identity
- signature validates
- credential status is valid

A successful verification establishes that the presented cryptographic proof corresponds to the registered credential.


---

# 4. Credential Lifecycle

Credentials have independent lifecycle states:

- ACTIVE
- PENDING
- REPLACED
- REVOKED
- EXPIRED

REPLACED indicates intentional migration to a newer credential.

REVOKED indicates the credential should no longer be trusted.

---

# 5. Compatibility Authentication

UCII includes compatibility authentication endpoints:

/v1/auth/*

These endpoints support existing systems migrating toward cryptographic identity.

Authentication remains an application layer built on top of identity.

---

# Summary

UCII separates:

- identity
- credentials
- authentication

Identity is the primitive.

Authentication is an application.
