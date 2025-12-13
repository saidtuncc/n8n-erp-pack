# Sync New Shopify Products to Odoo Product

## What it does
On each new Shopify product event, filters/normalizes product data and syncs it into Odoo product records.

## Trigger
- Shopify Trigger (shopifyTrigger)

## Systems / Nodes
- Odoo
- Shopify

## Setup
- Configure Shopify credentials (Shopify Trigger).
- Configure Odoo credentials in Odoo nodes.
- Adjust SKU/variant mapping in the `Code` node based on your catalog structure.

## Notes
- If you have variants, decide whether you create separate Odoo products or handle variants via attributes.
- Plan for incremental updates (price/stock/title changes) to avoid overwriting hand-edited fields in Odoo.

