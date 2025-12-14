# n8n ERP & Business Systems Integrations

Curated n8n workflows demonstrating ERP-adjacent integrations (order-to-cash, finance/accounting sync, CRM import, and ops notifications).

## How to use
1. Import a workflow JSON into n8n: **Workflows → Import from File**.
2. Configure credentials for each node (Shopify, Odoo, QuickBooks, HubSpot, Salesforce, etc.).
3. Review mappings and identifiers (customer matching keys, SKU/item mapping, PO/invoice linkage) before enabling.

## Repository structure
- `workflows/erp/` — ERP-facing workflows (Business Central, Odoo, NetSuite, ERPNext)
- `workflows/finance/` — payment → accounting and finance notifications (Stripe, QuickBooks, HubSpot)
- `workflows/crm/` — CRM imports/sync (Excel → Salesforce)
- `workflows/ops/` — operational notifications/last-mile hooks (WooCommerce, Onfleet)

## Contact
- LinkedIn: https://www.linkedin.com/in/saidtunc/
- GitHub: https://github.com/saidtuncc
