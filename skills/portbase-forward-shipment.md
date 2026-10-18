---
name: portbase-forward-shipment
description: Process and forward shipments through the cargo controller system.
api: openapi/portbase-hinterland-container-notification-openapi.yml
operations:
- _01_processShipments
- _03_forwardShipment
- _03b_cancelShipmentForwarding
generated: '2026-10-18'
method: generated
generator: extract-docs-artifacts.py skills (deepseek)
source: openapi/portbase-hinterland-container-notification-openapi.yml ; every operationId checked against the contract
---

# portbase-forward-shipment

Process and forward shipments through the cargo controller system.

## Steps

1. 1. Declare shipments using `_01_processShipments` with shipment data in the request body
2. 2. Forward a shipment using `_03_forwardShipment` with forwarding details in the request body
3. 3. Cancel shipment forwarding if needed using `_03b_cancelShipmentForwarding` with cancellation details in the request body

## Rules

- Authentication requires the ${authorizer-name} API key in the header
- Use the appropriate server endpoint based on environment (PCS or KT)
- Operations are performed sequentially: declare shipments first, then forward them
