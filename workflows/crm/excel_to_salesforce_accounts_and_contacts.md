# Excel To Salesforce Accounts And Contacts

## What it does
Reads companies/contacts from an Excel file, deduplicates, searches existing Salesforce Accounts, creates missing Accounts, and creates related Contacts.

## Trigger
- On clicking 'execute' (manualTrigger)

## Systems / Nodes
- Microsoft Excel
- Salesforce

## Setup
- Configure Microsoft Excel node to read your workbook and sheet.
- Configure Salesforce credentials (connected app / OAuth).
- Confirm dedupe keys (company name/domain, contact email) and adjust `Remove duplicate companies` if needed.

## Notes
- For large files, prefer batching and add a checkpoint mechanism (last row processed) to resume safely.
- Log rejects (validation failures) to a separate sheet or queue for review.

