# Stripe Payments To Quickbooks Sales Receipt

## What it does
On Stripe payment events, fetches the Stripe customer, ensures a matching QuickBooks customer exists, then posts a Sales Receipt via QuickBooks.

## Trigger
- New Payment (stripeTrigger)

## Systems / Nodes
- HTTP Request (REST)
- QuickBooks Online
- Stripe

## Setup
- Configure Stripe credentials (Stripe Trigger + Stripe node).
- Configure QuickBooks Online credentials in the QuickBooks node(s).
- Review the `POST Sales Receipt` / HTTP Request mapping (tax, currency, item/service, account mapping).

## Notes
- Decide your matching rule: Stripe customer email vs external ID; keep it consistent to prevent duplicate customers.
- Handle partial payments/refunds explicitly (separate workflows or branching).

