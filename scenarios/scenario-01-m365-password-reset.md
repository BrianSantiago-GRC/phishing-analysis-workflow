# Scenario 01: Microsoft 365 Password Reset Phish

> Scenario note: This is a sanitized training scenario. It does not contain real user, employer, tenant, or customer information.

## Scenario

A user reports an email claiming their Microsoft 365 password will expire today. The email asks the user to verify their account through a link.

## Observed Details

| Field | Scenario Value |
|---|---|
| Display name | Microsoft 365 Security |
| Sender | `security-alert@example-training.com` |
| Reply-to | `support@example-training.com` |
| Subject | `Action Required: Password Expiration Notice` |
| Link text | `Verify Account` |
| Destination | `hxxps://m365-verify.example[.]com/login` |
| Attachment | None |
| User action | User reported before entering credentials |

## Suspicious Indicators

- Microsoft branding used with non-Microsoft sender domain.
- Urgency language: password expiration today.
- Link destination does not match Microsoft domain.
- Account verification request.
- Reply-to does not match the claimed sender.

## Initial Classification

Medium risk.

Reason: Credible phishing indicators are present, but no credential entry or attachment execution was confirmed.

## Recommended Action

- Advise user not to click.
- Preserve message and headers.
- Search for additional recipients.
- Block sender/domain/URL if confirmed malicious.
- Escalate if any user entered credentials.
