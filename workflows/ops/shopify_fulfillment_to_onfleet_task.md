# Creating an Onfleet Task for a new Shopify Fulfillment

## What it does
On Shopify fulfillment events, creates a delivery task in Onfleet.

## Trigger
- Shopify Trigger (shopifyTrigger)

## Systems / Nodes
- Onfleet
- Shopify

## Setup
- Configure Shopify Trigger credentials and event type (fulfillment).
- Configure Onfleet credentials and mapping (recipient, address, notes, time window).

## Notes
- Normalize addresses (especially country/region formats) before task creation to reduce dispatch errors.

