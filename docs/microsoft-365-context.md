# Microsoft 365 Phishing Context

## Purpose

This section explains how the phishing workflow maps to a Microsoft 365 environment without claiming ownership of a live enterprise security program.

## User Reporting Flow

A realistic Microsoft 365 reporting flow may include:

- User reports suspicious email from Outlook.
- IT or security receives the report.
- Analyst reviews the message details.
- Analyst checks whether the message reached other mailboxes.
- Analyst recommends containment based on user interaction and indicators.

## Microsoft 365 Areas To Understand

| Area | What To Review |
|---|---|
| Outlook report | User-submitted suspicious email |
| Message headers | SPF, DKIM, DMARC, routing, sender details |
| Exchange message trace | Delivery status and recipient scope, if available |
| Microsoft Defender portal | Email entity, URL, attachment, and threat details, if available |
| Entra ID sign-in logs | Suspicious sign-ins after credential exposure |
| User sessions | Session revocation if credentials may be compromised |

## Common Microsoft 365 Response Ideas

- Search for other recipients.
- Quarantine similar messages if available.
- Block malicious sender/domain/URL after validation.
- Reset password if credentials were entered.
- Revoke active sessions if account compromise is possible.
- Review recent sign-ins for the affected account.
- Check inbox rules if compromise is suspected.
- Document the finding and escalation decision.

## Junior Analyst Boundary

A junior analyst may support the investigation by collecting evidence, reviewing indicators, documenting findings, and escalating clearly. Final tenant-wide actions may require approval from a senior analyst, administrator, or security owner.
