# [n8n] - Shopify Orders to D365 Business Central Sales Orders / Sales Invoices

## What it does
Pulls new/updated Shopify orders, maps customer + line items, and creates/updates Sales Orders and Sales Invoices in Microsoft Dynamics 365 Business Central via REST.

## Trigger
- Schedule Trigger (scheduleTrigger)

## Systems / Nodes
- HTTP Request (REST)
- Shopify

## Setup
- Configure Shopify credentials (API key/app) in the Shopify node.
- Set Business Central environment/company settings in the `D365 BC Environment Settings` node (or equivalent).
- Provide BC OAuth2 credentials / access token configuration for HTTP Request nodes.
- Review mapping nodes (`Sales Order Mapping`, `Set Lines Invoice`) and align SKUs, taxes, and currency rules.

## Notes
- This workflow contains cleanup nodes (DELETE Sales Order / Sales Invoice). Keep them disabled unless you intentionally need destructive operations.
- Consider idempotency: use Shopify order ID as an external reference in Business Central to avoid duplicates.
- Business Central and Shopify APIs are rate-limited; batch/schedule frequency should be tuned for your volume.

