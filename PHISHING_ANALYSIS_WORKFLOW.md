# Phishing Analysis Workflow - Project Status

Date started: 2026-05-15
Status: completed portfolio documentation; screenshot evidence polish pending

GitHub: https://github.com/BrianSantiago-GRC/phishing-analysis-workflow

Note: Brian confirmed the project was completed, but the original local files were lost. This local workspace now contains a rebuilt, completed portfolio-quality documentation project. Screenshots still need to be added from recovered or newly sanitized evidence.

## Main Files

- `README.md`
- `docs/investigation-workflow.md`
- `docs/microsoft-365-context.md`
- `docs/analyst-timeline-walkthrough.md`
- `docs/remediation-recommendations.md`
- `docs/lessons-learned.md`
- `scenarios/scenario-01-m365-password-reset.md`
- `scenarios/scenario-02-invoice-attachment.md`
- `evidence/ioc-extraction-example.md`
- `evidence/email-header-analysis-example.md`
- `evidence/link-and-attachment-review.md`
- `incident_notes/completed-incident-notes.md`
- `incident_notes/escalation-summary.md`
- `templates/ioc-checklist.md`
- `templates/incident-notes-template.md`
- `templates/user-report-intake-template.md`
- `screenshots/README.md`
- `linkedin/LINKEDIN_PROJECT_SUMMARY.md`

## Screenshot Gap

No real screenshots are currently included. Add sanitized screenshots to `screenshots/` before treating the project as screenshot-backed.

## Purpose

Document a realistic phishing triage process that shows operational security judgment, clear evidence handling, and escalation discipline.

## Scenario

A user reports a suspicious email that appears to impersonate a known service and asks the user to click a link or open an attachment.

## Triage Workflow

1. Confirm report details.
   - Who reported it?
   - When was it received?
   - Did the user click, download, reply, or enter credentials?

2. Preserve evidence.
   - Save the email or screenshot.
   - Capture sender address, subject, timestamp, URLs, attachments, and headers if available.

3. Review sender and header indicators.
   - Display name mismatch.
   - Sender domain mismatch.
   - Reply-to mismatch.
   - SPF/DKIM/DMARC failures.
   - Unusual originating IP or relay path.

4. Review content indicators.
   - Urgency or fear language.
   - Credential request.
   - Payment or gift card request.
   - Unexpected attachment.
   - Link text does not match destination.
   - Brand impersonation.

5. Extract indicators of compromise.
   - Sender email.
   - Reply-to email.
   - URLs.
   - Domains.
   - IP addresses.
   - Attachment filenames.
   - Hashes if available.

6. Check reputation safely.
   - Use URL/domain reputation tools.
   - Do not open suspicious links directly.
   - Use safe preview or reputation services.
   - Record results and timestamps.

7. Classify risk.
   - Low: suspicious but no click and no clear malicious payload.
   - Medium: credible phishing attempt, no user interaction confirmed.
   - High: user clicked, entered credentials, opened attachment, or multiple users received it.

8. Escalate if needed.
   - Credential entry.
   - Attachment opened.
   - Malware indicators.
   - Multiple recipients.
   - Executive, finance, HR, or privileged user targeted.

9. Response action.
   - Advise user not to interact.
   - Reset password if credentials were entered.
   - Revoke sessions if applicable.
   - Block sender/domain/URL if confirmed malicious.
   - Search for other recipients.
   - Document incident notes.

10. Lessons learned.
   - What indicator mattered most?
   - What control would reduce recurrence?
   - What user education point applies?

## IOC Checklist

| Indicator | Value | Notes |
|---|---|---|
| Sender email |  |  |
| Reply-to |  |  |
| Subject |  |  |
| URL/domain |  |  |
| Attachment |  |  |
| IP address |  |  |
| Hash |  |  |

## Incident Notes Template

| Field | Entry |
|---|---|
| Date/time reported |  |
| Reporter |  |
| User action taken |  |
| Initial classification |  |
| Evidence reviewed |  |
| IOCs found |  |
| Reputation check result |  |
| Escalation needed |  |
| Containment action |  |
| Final status |  |
| Lessons learned |  |

## LinkedIn Draft

I started documenting a practical phishing analysis workflow from an operations perspective.

The useful part is not just spotting a suspicious sender. It is building a repeatable decision path: preserve evidence, review headers, extract indicators, check reputation safely, classify risk, and know when to escalate.

That is the security operations skill I am focused on building: clear triage, strong documentation, and practical judgment.

## Next Milestone

Add recovered or newly sanitized screenshots to the GitHub repo.
