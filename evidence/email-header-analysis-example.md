# Email Header Analysis Example

> Sanitized example for portfolio documentation. Values are placeholders.

## Sample Header Snippet

```text
From: Microsoft 365 Security <security-alert@example-training.com>
Reply-To: support@example-training.com
To: user@example.com
Subject: Action Required: Password Expiration Notice
Authentication-Results: spf=fail; dkim=none; dmarc=fail
Received: from mail.example-training.com (203.0.113.10)
```

## Review

| Header Item | Observation | Analyst Meaning |
|---|---|---|
| From | Claims Microsoft 365 Security | Display name may be impersonating Microsoft |
| Sender domain | `example-training.com` | Does not match Microsoft |
| Reply-to | `support@example-training.com` | Reply-to does not support the claimed identity |
| SPF | Fail | Sending source not authorized in this sample |
| DKIM | None | No valid signing observed in this sample |
| DMARC | Fail | Domain alignment failed in this sample |
| Received IP | `203.0.113.10` | Documentation IP reserved for examples |

## Analyst Summary

The sample header supports a phishing classification because the sender identity, reply-to address, and authentication results do not align with the claimed Microsoft 365 brand.

## Boundary

Header findings support the investigation, but the final decision should also consider links, attachments, user action, recipient scope, and reputation results.
