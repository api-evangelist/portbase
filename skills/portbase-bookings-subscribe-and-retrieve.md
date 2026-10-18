---
name: portbase-bookings-subscribe-and-retrieve
description: Subscribe to a booking and retrieve the booking dossier by subscription ID.
api: openapi/portbase-cargo-controller-export-openapi.yml
operations:
- subscribe
- getBySubscriptionId
generated: '2026-10-18'
method: generated
generator: extract-docs-artifacts.py skills (deepseek)
source: openapi/portbase-cargo-controller-export-openapi.yml ; every operationId checked against the contract
---

# portbase-bookings-subscribe-and-retrieve

Subscribe to a booking and retrieve the booking dossier by subscription ID.

## Steps

1. 1. Call `subscribe` POST /v1/bookings with booking subscription data to create a new booking subscription
2. 2. Call `getBySubscriptionId` GET /v1/bookings/{subscriptionId} with the subscriptionId from the subscribe response to retrieve the booking dossier

## Rules

- Use ${authorizer-name} apiKey header authorizer for authentication
- Use subscriptionId from subscribe response as path parameter for getBySubscriptionId
