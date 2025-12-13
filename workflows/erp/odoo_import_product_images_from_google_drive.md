# Import Odoo Product Images from Google Drive

## What it does
Scheduled import of product images from Google Drive into Odoo product templates; moves/organizes images after processing.

## Trigger
- Schedule Trigger (scheduleTrigger); Click Manual (manualTrigger)

## Systems / Nodes
- Google Drive
- Odoo

## Setup
- Configure Google Drive credentials (Find/Download/Move nodes).
- Configure Odoo credentials for the product template lookup/update steps.
- Define the Drive folder structure and naming convention used to match images to Odoo products.

## Notes
- Keep an audit trail: write processed file IDs somewhere (Sheet/DB) to avoid re-importing the same image.
- Large images may increase runtime; consider resizing/compressing upstream.

