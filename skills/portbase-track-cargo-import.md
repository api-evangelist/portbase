---
name: portbase-track-cargo-import
description: Create a tracking request and retrieve tracked bills of lading for cargo import operations.
api: openapi/portbase-cargo-controller-import-openapi.yml
operations:
- track_1
- trackedBls_1
generated: '2026-10-18'
method: generated
generator: extract-docs-artifacts.py skills (deepseek)
source: openapi/portbase-cargo-controller-import-openapi.yml ; every operationId checked against the contract
---

# portbase-track-cargo-import

Create a tracking request and retrieve tracked bills of lading for cargo import operations.

## Steps

1. 1. Submit a tracking request using `track_1` operation with required tracking parameters in the request body
2. 2. Retrieve tracked bills of lading using `trackedBls_1` operation with appropriate query parameters

## Rules

- Authentication requires ${authorizer-name} API key in the header
- Use appropriate server endpoint based on environment (PCS or KT)
