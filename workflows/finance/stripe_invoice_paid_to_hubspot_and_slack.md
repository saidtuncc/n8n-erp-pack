# On new Stripe Invoice Payment update Hubspot and notify the team in Slack

## What it does
When a Stripe invoice is paid, finds and updates the related HubSpot deal, and notifies the team in Slack; includes handling for missing PO/deal.

## Trigger
- When Invoice Paid (stripeTrigger)

## Systems / Nodes
- HubSpot
- Slack
- Stripe

## Setup
- Configure Stripe Trigger credentials.
- Configure HubSpot credentials and confirm the property used for PO/deal matching.
- Configure Slack credentials/channel.

## Notes
- Make the matching key explicit (PO number, invoice ID, subscription ID) and document it in the repo README.
- Consider dedupe for repeated Stripe events (webhook retries).

