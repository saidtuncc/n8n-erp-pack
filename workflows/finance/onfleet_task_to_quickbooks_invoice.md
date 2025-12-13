# Create a QuickBooks invoice on a new Onfleet Task creation

## What it does
Creates a QuickBooks invoice when a new Onfleet Task is created (operational event → accounting document).

## Trigger
- Onfleet Trigger (onfleetTrigger)

## Systems / Nodes
- Onfleet
- QuickBooks Online

## Setup
- Configure Onfleet Trigger credentials and select the task event you care about.
- Configure QuickBooks Online credentials and invoice defaults (customer, item, account).

## Notes
- If Onfleet tasks can be edited/cancelled, add update/cancellation logic to keep accounting consistent.

