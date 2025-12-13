# Sync New Shopify Customers to Odoo Contacts

## What it does
On each new Shopify customer event, searches for an existing Odoo contact; creates one if missing.

## Trigger
- Shopify Trigger (shopifyTrigger)

## Systems / Nodes
- Odoo
- Shopify

## Setup
- Configure Shopify credentials (Shopify Trigger).
- Configure Odoo credentials (URL, database, username/API key) in the Odoo nodes.
- Review the `Code` node to match your contact field mapping (email, phone, VAT, address).

## Notes
- Use email as the primary matching key if possible; add secondary matching rules if your data is messy.
- If you operate multi-company in Odoo, ensure the correct company/context is set.

