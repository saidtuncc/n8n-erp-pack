# Erpnext Ai Candidate Shortlisting Webhook

## What it does
Receives applicant data via webhook, extracts resume content, uses an LLM (Gemini) for evaluation, and updates ERPNext applicant status; supports notifications via Outlook/WhatsApp.

## Trigger
- Webhook (webhook)

## Systems / Nodes
- ERPNext
- Google Gemini (LLM)
- HTTP Request (REST)
- Microsoft Outlook
- WhatsApp

## Setup
- Configure ERPNext credentials and base URL in ERPNext nodes.
- Configure LLM credentials (Google Gemini) and ensure prompts are aligned with your hiring rubric.
- Configure Webhook payload format (applicant fields + resume attachment) and Outlook/WhatsApp credentials if used.

## Notes
- Do not store sensitive applicant data longer than necessary; prefer minimal retention.
- In production, add guardrails: prompt injection protection, redaction, and human review for borderline cases.

