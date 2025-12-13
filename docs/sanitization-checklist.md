# Sanitization checklist (before pushing to GitHub)

Scan each workflow JSON for:
- Webhook URLs/paths and secrets
- API base URLs pointing to real tenants
- Email addresses, phone numbers, customer names
- Order/invoice numbers, internal IDs
- Sample payloads (PII)

Recommended approach:
- Replace sensitive values with placeholders (e.g., `{TENANT_URL}`, `{API_KEY}`).
- Keep the workflow logic intact; only sanitize parameters and sample data.
- If you discover a secret was committed, rotate it immediately and rewrite git history (e.g., `git filter-repo`).
